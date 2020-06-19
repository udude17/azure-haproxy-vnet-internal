# azure-haproxy-vnet-internal
Deploy HAPROXY on a standard internal load-balancer on an existing Azure VNET


Original reference:  https://github.com/insidepowershell/azure-quickstart-templates/tree/master/haproxy-redundant-floatingip-ubuntu
- Modified it to use existing VNET and internal load balancer

0) Edit the paramters json file with your values including your subnetrefid 
1) upload the azuredeploy.xx.json files (two) and the .ps1 to the Azure cloud shell. (powershell)  
2) create a new ResGroup.  
3) az account set -s SUBID to ensure targeting the correct subscription.   
4) run the ./deploy-haproxy.ps1. 


Optional: Create an azure storage account of your own in Azure, create an new blob container, upload the .sh scripts, and reference that in the parameters file. Set manage access to public blob.

