# What is Azure Portal ¿?

Azure Portal is the Graphic Unit Interface (GUI) that allow manage all the resources in a unified console.

# What is Azure Cloud Shell ¿?

Is a browser-accesible shell for managing Azure resources, based on Bash or Powershell.

For more information about Azure Cloud Shell, follow this link: https://docs.microsoft.com/en-us/azure/cloud-shell/overview

# What is Azure PowerShell ¿?

Azure Powershell is a module that can be install in Windows Powershell or Powershell Core to manage de Azure resource(s) and subcription(s).

You can use Azure Powershell through:
- Azure Cloud Shell
- Local Installation (Windows, MacOS or Linux)

# What is Azure CLI ¿?

Azure CLI is a cross-platform command line program to manage the Azure resource(s) and subscription(s).

You can use Azure Powershell through:
- Azure Cloud Shell
- Local Installation (Windows, MacOS or Linux)

# What is Azure Resource Manager (ARM) ¿?

Is the service that Azure uses to deploy and manage the resources, through a management layer that allows to create, update, and delete resources.

<p align=center>
<img src="../assets/arm.png" alt="ARM" title="ARM"> </p>

# Azure Resource Manager (ARM) Templates ¿?

Is a block/piece of code based on JSON (JavaScript Object Notation) that define the infrastructure resources and configuration for a proyect or deployment.

The ARM Templates file contains various key-value pairs in the JSON format. For example, below, you can see a format of an ARM Templates.

<p>{</p>
<p>"$schema": "https://schema.management.azure.com/schemas/2015-01-01/deploymentTemplate.json#",</p>
<p>"contentVersion": "1.0.0",</p>
<p>"parameters":{},</p>
<p>"variables":{},</p>
<p>"functions":[],</p>
<p>"resources": [],</p>
<p>"outputs":{}</p>
<p>}</p>

For more information about ARM Templates, follow the next link:
https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/overview