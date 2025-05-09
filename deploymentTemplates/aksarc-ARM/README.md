# ARM template to deploy an AKS Arc Kubernetes cluster

This template deploys an AKS Arc Kubernetes cluster with workload identity federation enabled.

## Instructions

Update azuredeploy.parameters.json with provisioned cluster name, ssh public key, and ARM IDs of vnet and custom location.

## Deploy

You can use the following command to deploy the template

```CLI
az deployment group create -g $resourceGroup --template-file azuredeploy.json -p azuredeploy.parameters.json
```
for more details please look through [Arm template deployment with Powershell](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/deploy-powershell) 
and 
[ARM template documentation](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/)
