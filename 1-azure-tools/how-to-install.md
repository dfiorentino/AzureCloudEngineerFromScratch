# How to use Azure Cloud Shell

You can access to this option by two ways:

- Using a direct link to https://shell.azure.com
- Using the option Cloud Shell from the Azure Portal

Once you're in the shell you need to select <strong>Bash</strong> or <strong>Powershell</strong> as a cmdlets interpreter.

# How to install Azure CLI

For Linux on Ubuntu/Debian use apt-get, on RedHat/Fedora/CentOs use yum and zypper for OpenSUSE.

More information for Linux installation: https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-linux?pivots=apt

For MacOS use Homebrew

More information for MacOS installation: https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-macos

For Windows we need to download and execute a MSI file.

To download Azure CLI for Windows, click here: https://aka.ms/installazurecliwindows and follow the instructions.

Run az --version after the installation process to see if works.

# How to install Azure PowerShell

In this section we are only cover the Windows installation.

Before the installation is recommended to update your version of Powershell to 7.1.3, PowerShell 7.0.6 LTS or higher.

Run this command to validate the PS version:
$PSVersionTable.PSVersion

To install the module: Install-Module -Name Az -Verbose -Force

Another method to install this module is the Offline Installation by downloading the MSI file: https://docs.microsoft.com/en-us/powershell/azure/install-az-ps-msi?view=azps-7.4.0

Run Connect-AzAccount to see if the installation works.