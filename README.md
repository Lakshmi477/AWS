# AWS Networking and IP Addressing

## **Introduction to IP Address**
An **IP Address (Internet Protocol Address)** identifies devices on a network. There are two types of IP addresses:
1. **IPv4**
2. **IPv6**

### **IPv4**
- Represented in **4 decimal numbers** separated by `.` (e.g., `192.168.1.1`).
- Uses **32-bit addresses**, allowing approximately **4 billion unique addresses**.
- Divided into classes based on the address range:
  - **Class A**: `1.0.0.0` to `126.0.0.0` (Large networks with multiple devices).
  - **Class B**: `128.0.0.0` to `191.255.0.0` (Medium-sized networks).
  - **Class C**: `192.0.0.0` to `223.255.255.0` (Small networks).
  - **Class D**: `224.0.0.0` to `239.255.255.255` (Multicast groups).
  - **Class E**: `240.0.0.0` to `255.255.255.255` (Experimental/future use).
- Supports both **manual configuration** and **dynamic configuration** using **DHCP** (Dynamic Host Configuration Protocol).

### **IPv6**
- Represented in **8 hexadecimal numbers** separated by `:` (e.g., `2001:0db8:85a3:0000:0000:8a2e:0370:7334`).
- Supports **auto-configuration** and **renumbering**.
- Does not use address classes.
- Devices can use both **IPv4** and **IPv6** simultaneously.

---

## **NAT (Network Address Translation)**
- Allows devices on a private network to access the internet using a single public IP.
- **Private IPs** are translated to **Public IPs** to provide internet access to local hosts.

---

## **Amazon VPC (Virtual Private Cloud)**
A **Virtual Private Cloud (VPC)** enables you to launch AWS resources in a logically isolated virtual network.

### **Key Features**
1. **Subnets**: 
   - A range of IP addresses within your VPC.
   - Can add one subnet in each **Availability Zone**.
   
2. **IP Addressing**:
   - Support for **IPv4** and **IPv6**.

3. **Route Tables**:
   - Define how network traffic is directed within your VPC.

4. **Gateways**:
   - Connect your VPC to other networks or the internet.
   - Example: **Internet Gateway**.

5. **VPC Peering**:
   - Allows routing traffic between resources in two VPCs.

---

## **AWS Services Using Public IPv4**
AWS services that require or support public IPv4 include:
- **Amazon AppStream 2.0**
- **AWS Client VPN**
- **AWS Database Migration Services**
- **Amazon EC2**
- **Amazon Elastic Container Service (ECS)**
- **Amazon EKS**
- **Amazon ECR**
- **Amazon GameLift**
- **AWS Global Accelerator**
- **AWS Mainframe Modernization**
- **Amazon Managed Service for Apache Kafka**
- **Amazon Redshift**
- **Amazon RDS**
- **Amazon MQ**
- **AWS Site-to-Site VPN**
- **Amazon VPC NAT Gateway**
- **Amazon Workspaces**
- **AWS ELB**

---

## **Key Concepts Summary**
1. **NAT**: Enables private networks to communicate with the internet via public IPs.
2. **Subnets**: Logical divisions of a VPC, each with its own range of IP addresses.
3. **Gateways**: Bridge your VPC to the internet or other networks.
4. **Route Tables**: Manage network traffic direction.
5. **IPv4 vs IPv6**:
   - IPv4: 32-bit, class-based.
   - IPv6: 128-bit, no classes, written in hexadecimal.

---
## **How to View IP Addresses**
- Use the `ipconfig` command on the command prompt to view both IPv4 and IPv6 addresses.

--- 
## **Conclusion**
Amazon VPC and AWS networking services provide flexibility to build secure and scalable cloud networks, utilizing both IPv4 and IPv6 addressing to meet modern requirements.

VPC Endpoints:
Vpc endpoints enables to customer to connect privately to the AWS servives and VPC endpoint services with AWS private link.
VPC doesn't require public IP
They are 2 types of endpoints
1.Interface endpoints
2.gateway endpoints
Interface endpoints:
It enables private acess to services provided by AWS without travsing the public network.They are used in Elastic Network interface(ENI) in VPC.
gateway endpoints:
It Provides the route table entry to route traffic to s3 over private networks.
It supoorts only S3 and DynamoDB

