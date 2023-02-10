# Script
using PowerShell/Python/Whatever, that will install "av-software.exe" on a virtual machine. 
The script will be deployed via GPO to all machines where it will be installed. 
Feel free to use Google or any other resource to aid in writing the script.
This script first defines the location of the installer package, then checks if the software is already installed on the virtual machine using the WMI class Win32_Product. 
If the software is not already installed, the script will use Start-Process to run the installer with the "/quiet" argument for a silent installation. 
The script will wait for the installer to complete before moving on. Finally, the script will confirm that the software is installed by running the check again and will give the output if the software is installed or not.
This script can be deployed via GPO (Group Policy Object) to all virtual machines that you want to install the AV software on.

