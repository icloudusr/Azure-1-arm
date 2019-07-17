
1-Arm VM-Series Configuration Skillet

This skillet configures a VM-Series firewall on Azure in a 1-arm configuration.

The config snippets include security policies, NAT policies, routing Policies, routing configuration and network configuration.

The following diagram shows a generic topology using a single firewall pair between a set of load balancers: a public and an internal load balancer. The public facing load balancer (standard SKU) load balances traffic through the VM-series untrust interface while the internal load balancer does it through the dmz interfaces. The dmz interfaces support direct traffic from om-prem and azure VNETs.  

![alt_text](https://github.com/icloudusr/azure-1-arm/blob/master/single_pair/1-armgen.png)

The following diagram shows a more detailed topology which incudes specific IP addresses used to bring up a testing topology and to validate the working of the 1-arm mode environment. Note that the VM-series include public IP addresses both on the mgmt and untrust interfaces.

![alt_text](https://github.com/icloudusr/azure-1-arm/blob/master/single_pair/1-armdet.png)

The documentation include a guide that walks through he details of the Azure environemnt and the 1-ram VM-Series configuration. The guide could is found here: https://github.com/icloudusr/azure-1-arm/blob/master/documentation/azure-1-arm%20guide.pdf

There is an additional document that provide additional reference details about the environment, the test details and the test results looking at traffic logs: https://github.com/icloudusr/azure-1-arm/blob/master/documentation/skillet%20azure-1-arm.pdf  