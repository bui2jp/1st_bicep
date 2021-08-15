# はじめてのBicep

https://docs.microsoft.com/ja-jp/azure/azure-resource-manager/bicep/quickstart-create-bicep-use-visual-studio-code?tabs=CLI

## リソース作成
```
az group create --name exampleRG --location eastus
```

## Bicepをデプロイ
```
az deployment group create --resource-group exampleRG --template-file main.bicep --parameters storageName={your-unique-name}
```
storageNameは小文字と数字で。

## リソース削除
```
az group delete --name exampleRG
```
