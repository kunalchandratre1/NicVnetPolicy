# NicVnetPolicy
This repo has code related to Azure policy to identify Azure resources which are not deployed in approved VNETs.

Virtual machines should be connected to an approved virtual network - Thise default Azure policy is fantastic. This policy checks if a VM is part of approved VNET; else it shows compliance message. 
However it only offers VMs to be checked against single VNET name. In reality, we have flood of Azure VNETs across multiple Azure subscriptions.
So we need a policy that can check all Azure VMs against “multiple azure Virtual Networks”.
This policy code creates a policy that allows to provision Azure VMs inside only allowed list of VNETs, precisely MULTIPLE VNETs.. 

Refer to the link for more details - 
