
1-Arm VM-Series Configuration Skillet

This skillet configures a VM-Series firewall on Azure to support 1-arm configurations for a single VM-Series pair

The snippets includes security policies, NAT policies, routing Policies, routing configuration and network configuration.

The documentation discusses the Azure environment design pattern and the configuration expected to ensure the VM-series are able to operate in 1-arm mode.

The following diagram shows a generic topology using a single firewall pair between a set of load balancers: a public and an internal load balancer. The public facing load balancer (standard SKU) load balances traffic through the VM-series untrust interface while the internal load balancer does it through the dmz interfaces. The dmz interfaces support direct traffic from om-prem and azure VNETs.  

![alt_text](https://github.com/icloudusr/Azure/blob/master/1-arm/1-armdet.png)

The following diagram shows a more detailed topology which incudes specific IP addresses used to bring up a testing topology and to validate the working of the 1-arm mode environment. Note that the VM-series include public IP addresses both on the mgmt and untrust interfaces.

![alt_text](https://github.com/icloudusr/Azure/blob/master/1-arm/1-armgen.png)