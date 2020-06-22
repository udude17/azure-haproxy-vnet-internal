# azure-haproxy-vnet-internal
Deploy HAPROXY on a standard internal load-balancer on an existing Azure VNET

Original reference:  https://github.com/insidepowershell/azure-quickstart-templates/tree/master/haproxy-redundant-floatingip-ubuntu
Adapted to use existing VNET and internal load balancer

Usage Steps:
1) Edit the paramters json file with your values including your subnetrefid 
2) Review and edit the load balancer ports in the variables section in the main azuredeploy template
3) upload the azuredeploy.xx.json files (two) and the .ps1 to the Azure cloud shell. (powershell)  
4) create a new resource group  
5) az account set -s SUBID to ensure targeting the correct subscription.   
6) run the ./deploy-haproxy.ps1 scrips


Optional: Create an azure storage account of your own in Azure, create an new blob container, upload the .sh scripts, and reference that in the parameters file. Set manage access to public blob.


