Create an Azure Resource Manager template to deploy a StorageAccount

Prerequisites

An Azure account with an active subscription. If you don't already have one, you can sign up for a free trial at https://azure.com/free.
Visual Studio Code with the Azure Resource Manager Tools installed.
Azure CLI installed locally

This template depicts the use of parameters while configuring services.

template can be deployed using az CLI 

//Create resource group  (Location could be eastus for example)
az group create --name [RESOURCE-GROUPNAME] --location [LOCATION]

//Create deployment group
az deployment group create --resource-group [RESOURCE-GROUP] --template-file [FILE.JSON] --parameters [FILE.PARAMETERS.JSON]

//validate resource created 
az deployment group list --resource-group [RESOURCE-GROUP]

