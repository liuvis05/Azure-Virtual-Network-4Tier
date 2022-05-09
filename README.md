# Azure-Virtual-Network-4Tier
Design 4-Tier Azure Virtual Network using Terraform

Azure Virtual Network Design

We are going to design the 4-Tier Azure Virtual Network here
Azure Virtual Network
WebTier Subnet + WebTier Network Security Group (Ports 80, 443)
AppTier Subnet + AppTier Network Security Group (Ports 8080, 80, 443)
DBTier Subnet + DBTier Network Security Group (Ports 3306, 1433, 5432)
Bastion Subnet + Bastion Network Security Group (Ports 80, 3389)
Terraform for_each Meta-Argument
Azure Resources created

azurerm_resource_group
azurerm_virtual_network
azurerm_subnet
azurerm_network_security_group
azurerm_subnet_network_security_group_association
azurerm_network_security_rule

Step-08: Execute Terraform Commands

# Terraform Initialize
terraform init

# Terraform Validate
terraform validate

# Terraform Plan
terraform plan

# Terraform Apply
terraform apply -auto-approve
Step-09: Verify Resources

# Verify Resources - Virtual Network
1. Azure Resource Group
2. Azure Virtual Network
3. Azure Subnets (Web, App, DB, Bastion)
4. Azure Network Security Groups (Web, App, DB, Bastion)
5. View the topology
6. Verify Terraform Outputs in Terraform CLI
Step-10: Delete Resources

# Delete Resources
terraform destroy 
terraform apply -destroy

# Clean-Up Files
rm -rf .terraform* 
rm -rf terraform.tfstate*
