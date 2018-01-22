# Multi VM deployment from managed disk custom image

[![Deploy to Azure](http://azuredeploy.net/deploybutton.svg)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsnobu%2Fmulti-vm-from-template%2Fmaster%2Fazuredeploy.json)


For MS Internal Portal (**ms**.portal.azure.com), use this one:

[![Deploy to Azure](http://azuredeploy.net/deploybutton.svg)](https://ms.portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsnobu%2Fmulti-vm-from-template%2Fmaster%2Fazuredeploy.json)


<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fsnobu%2Fmulti-vm-from-template%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

This template allows you to deploy one or more VMs using a managed disk custom image as source.

## Usage:

1. Create resource group "X"
2. Create Virtual Network in resource group "X"
3. Create Subnet in Virtual Network in resource group "X"
4. Deploy template, use values from steps `1`, `2`, `3`, and use full resourceId URI as `imageId` (for example: `/subscriptions/{SUBSCRIPTION_ID}/resourceGroups/{RESOURCE_GROUP}/providers/Microsoft.Compute/images/{IMAGE_NAME}`)