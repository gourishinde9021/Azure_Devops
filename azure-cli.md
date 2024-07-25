# Steps to deploy storage account arm template

### Create resource group
```
az group create --name vscode --location centralindia
```


### Create the storage account
Switch to the folder where you have the `azure-storage.json` or similar file

```
az deployment group create --resource-group vscode --template-file azure-storage.json
```