# Teil 3 Realisieren

> Back [Page](https://github.com/lauradubach/Semesterarbeit1/blob/main/Sites/Teil%202%20Vorbereitung.md)
>
> Next [Page](https://github.com/lauradubach/Semesterarbeit1/blob/main/Sites/Teil%204%20Abschluss.md)


- [Teil 3 Realisieren](#teil-3-realisieren)
- [Umsetzung](#umsetzung)
  - [Implementierungsplan](#implementierungsplan)
  - [CLI](#cli)
  - [Probleme](#probleme)
  - [Endprodukt](#endprodukt)
  - [Fallbacksolution](#fallbacksolution)
- [Kontrollieren](#kontrollieren)
  - [Testing](#testing)
  - [Schulung Kunde](#schulung-kunde)


# Umsetzung

## Implementierungsplan

![Implementierungsplan](../Pictures/Implementierungsplan.png)

## CLI
```bash
#!/bin/bash

if ! az account show > /dev/null 2>&1; then
  echo "Bitte melde dich bei der Azure CLI an..."
  az login
fi

# Variablen setzen
RESOURCE_GROUP="sa1blobresource"
LOCATION="switzerlandnorth"
STORAGE_ACCOUNT_NAME="sa1blobstorage"
CONTAINER_NAME="sa1blobcontainer"
FILES_TO_UPLOAD="C:\Users\laura\Documents\Test.txt"
EXPIRY_DATE=$(date -u -d "1 day" '+%Y-%m-%dT%H:%MZ')

# Azure Resource Group erstellen
az group create --name $RESOURCE_GROUP --location $LOCATION

# Azure Storage Account erstellen
az storage account create --name $STORAGE_ACCOUNT_NAME --resource-group $RESOURCE_GROUP --location $LOCATION --sku Standard_LRS --kind StorageV2

# Blob-Container erstellen
az storage container create --account-name $STORAGE_ACCOUNT_NAME --name $CONTAINER_NAME

#Account key erstellen
ACCOUNT_KEY=$(az storage account keys list --account-name $STORAGE_ACCOUNT_NAME --query "[?keyName=='key2'].value" --output tsv --output tsv)

# SAS-Token generieren
SAS_TOKEN=$(az storage container generate-sas --name $CONTAINER_NAME --account-name $STORAGE_ACCOUNT_NAME \
    --permissions rwdl --expiry $EXPIRY_DATE --auth-mode key \
    --account-key $ACCOUNT_KEY)

# Vollständige SAS-URL
SAS_URL="https://${STORAGE_ACCOUNT_NAME}.blob.core.windows.net/${CONTAINER_NAME}?${SAS_TOKEN}"

echo $SAS_TOKEN
echo $SAS_URL

# Dateien hochladen mit az storage blob upload-batch
az storage blob upload --account-name $STORAGE_ACCOUNT_NAME --account-key $ACCOUNT_KEY --container-name $CONTAINER_NAME --file $FILES_TO_UPLOAD --name myblob

echo "Dateien erfolgreich hochgeladen."
```

## Probleme

Folgenden Error habe ich erhalten:

``ERROR: incorrect usage: specify '--auth-mode login' when as-user is enabled``

Er hatte ein Problem mit dem Key erstellen, den Code musste ich dann anpassen:

```bash
#Account key erstellen
ACCOUNT_KEY=$(az storage account keys list --account-name $STORAGE_ACCOUNT_NAME --query "[?keyName=='key2'].value" --output tsv --output tsv)

#SAS-Token generieren
SAS_TOKEN=$(az storage container generate-sas --name $CONTAINER_NAME --account-name $STORAGE_ACCOUNT_NAME \
    --permissions rwdl --expiry $EXPIRY_DATE --auth-mode key \
    --account-key $ACCOUNT_KEY)
```

Fogendes habe ich effekiv gemacht:

Der code für den Key zu erstellen war zuerst am falschen Platz. Diesen musste ich zuerst erstellen. Dann musste ich im code noch as-user entfernen, da dies nicht gepasst hat und er dies nicht im kontext gekannt hat. Zusätzlich musste ich die Line ``--name $CONTAINER_NAME`` nach oben verschieben.

Danach kam das nächste problem:

``azcopy: command not found``

Ich habe dann az Storage upload verwendet, weil es mit azcopy nicht geklappt hat.

Folgenden Link habe ich verwendet: https://learn.microsoft.com/en-us/cli/azure/storage/blob?view=azure-cli-latest

## Endprodukt
## Fallbacksolution

# Kontrollieren
## Testing
## Schulung Kunde