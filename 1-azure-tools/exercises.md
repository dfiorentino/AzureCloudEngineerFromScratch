# Azure PowerShell

Connect to Azure:
<p><code>Connect-AzAccount</code></p>

Retrieve a list of all RG:
<p><code>Get-AzResourceGroup | Format-Table</code></p>

Create a Resource Group:
<p><code>New-AzResourceGroup -Name rg-lab-eastus2 -Location EastUs2</code></p>

Create a Virtual Machine with variables:
<p><strong>$rgname:</strong> "rg-lab-eastus"</p>
<p><strong>$vmname:</strong> "vm-lab-eastus"</p>
<p><strong>$location:</strong> "east-us-2"</p>
<p><strong>$image:</strong> "UbuntuLTS"</p>

<p><code>New-AzVm
            -ResourceGroupName $rgname
            -Name $vmname
            -Credential (Get-Credential)
            -Location $location
            -Image $image
</code></p>

Verify all the resources in the subscription:
<p><code>Get-AzResource | Format-Table</code></p>

