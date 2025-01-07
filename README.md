# AWS
IP measn interent protocol address.
 There are 2 types of IP address
   IPV4 and IPV6
   if we want to see the both address just run ipconfig on command promot. It is separted by (.)
   The IPV4 range: 0.0.0.0 to 255.255.255.255. IPV4 is divided into 4 classes Class A,Class B,Class C,Class D.
   class A: The range for Class A is 1.0.0.0 to 126.0.0.0. It is desined for large network with multiple devices.
   Class B: The range for Class B is 128.0.0.0 to 191.255.0.0. It is designed for medium sized networks
   Class C: The range for Class C is 192.0.0.0 to 223.255.255.0. It is desinged for small networks.
   Class D: The range for Class D is 224.0.0.0 to 239.255.255.255 . It is desugned for multicast groups.
   Class E: The range for Class E is 240.0.0.0 to 255.255.255.255. It is designed for Experimental and future usage.
   
It uses 32 bit address. It allows 4 billons unique addresses. IPV4 address are defined in 4 decimal numbers.
It supports both manual configuration of IP and dynamic configuration throught the DHCP(Dynamic host configuration protocol)
The IPV6 It is written in 8 hexadecimals sperated by (:)
Devices can use both IPV4 and IPV6 at a time. It supports auto and renumberng address configuration.IPV6 doesn't have any classes
NAT(Network Address Transalation):
One public Ip is needed to get the internet but we can use Private IP for private networks.It is the process in which one or more local IP address are transalated to one or more global IP and vice versa to provdide the internet access to local hostes.
VPC:Virtual Private cloud
We can lanuch AWS resources locally isolated virtual network.The VPC has a one subnet in each in avaiablity zone in the region.
EC2 instance in each subnet and an network gateway it allows the comminucation between the resources in VPC and internet.
After creating VPC we can add subnets
Subnets measn it is the range of IP address in our VPC.
IP Addressing we can add IPV4 and IPV6 to the vps and subnets.
Using route table to determine the where network traffic from your subnet or gateway directed
A gateway connects your VPC to another newtwork
Using VPC peering connection to route the traffic between the resources from 2 VPC's
AWS services that can use public IPV4
Amazon app stream 2.0
AWS clinet VPN
AWS database migration services
Amazon EC2
Amazon Elastic container services
Amazon EKS
Amazon EKR
Amazon gamelift
AWS global Accelerator
AWS mainframe modernization
Amazon managed for Apche kafka
Amazon redshift
Amazon RDS
amazom MQ
AWS site to site VPN
Amazon VPC NAT gateway
Amazon Workspaces
AWS ELB








   
