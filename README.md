# Azure-quickstart-windows-3tier
Azure Resource Manager Template with MGMT, WEB, DATA tiered Sub nets with access rules

# Step 1 Create Resource Group

E.g. azure group create demo1 westus
E.g. New-AzureRmResourceGroup -Name "RG01" -Location "South Central US"


# Step 2 Deploy Network Subnets
azure.network.json – sets up the network and NSGs between the subnets.

Azure CLI: azure group deployment create --template-uri https://github.com/manojvas/Azure-quickstart-windows-3tier/master/azure-network.json  demo1

Powershell: New-AzureRmResourceGroupDeployment -ResourceGroupName demo1 -TemplateUri https://github.com/manojvas/Azure-quickstart-windows-3tier/master/azure-network.json  demo1

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmanojvas%2Fazure-quickstart-windows-3tier%2Fmaster%2Fazure-network.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>

</a>
