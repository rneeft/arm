# StorageAccount
Creates a storage account.

## How to use
Add the following code section into the ARM template:
``` json
{
    "apiVersion": "2019-10-01",
    "name": "nestedTemplate",
    "type": "Microsoft.Resources/deployments",
    "properties": {
        "mode": "incremental",
        "templateLink": {
            "uri": "https://raw.githubusercontent.com/rneeft/arm/master/templates/StorageAccounts/2019-06-01/v1/azuredeploy.json",
            "contentVersion": "1.0.0.0"
        },
        "parameters": {
            "stage": {
                "value": "[parameters('stage')]"
            },
            "product": {
                "value": "[parameters('product')]"
            }
        }
    }
}
```
## Parameters
The template uses the following parameters:
| Name          | Required  | DefaultValue
| ------------- | :--------: | ------------: 
| stage         | Yes       | -
| product       | Yes       | -
| location | No | `[resourceGroup().location]`
| locationSmall | No        | `WE`
| kind | No | `StorageV2`
| skuName | No | `Standard_RAGRS`
| accessTier | No | `Hot`

### Output

| Name | Type |
| ---- | ---- |
| storageAccountName | string