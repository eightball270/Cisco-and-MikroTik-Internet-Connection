# Cisco and MikroTik Internet Connection
This simulation demonstrates how to configure a router to connect to an ISP (Internet Service Provider) so that some clients can access the internet. In this simulation, the host (the actual user's PC connected to the internet) acts as the ISP.

## Technology Used
- GNS3

## Requirements
1. A router and a switch
2. Client PCs
3. NAT cloud as ISP

## Configuration Completed
1. VLANs on router and switch
2. DHCP client on the router interface that connects to the ISP
3. NAT configuration on the router
4. DHCP server on the router or static IP configuration for each client (choose one)

## Internet Connection

### Cisco
To allow certain clients internet access, the Cisco configuration uses the Access Control List (ACL) method. The purpose of an ACL is to filter traffic based on the source address, destination address, port, and protocol. In this configuration, internet access is granted to all clients based on their network address.

![Internet Connection (Cisco).png](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/Cisco/Internet%20Connection%20(Cisco).png)

Project File Link : [Part1](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/Cisco/Internet%20Connection%20(Cisco).gns3project.part1.rar) and [Part2](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/Cisco/Internet%20Connection%20(Cisco).gns3project.part2.rar) (extract the separate archives into a single project file)

Internet connection test from PC1:

![Internet Connection (Cisco) (1).png](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/Cisco/Internet%20Connection%20(Cisco)%20(1).png)
![Internet Connection (Cisco) (2).png](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/Cisco/Internet%20Connection%20(Cisco)%20(2).png)

Internet connection test from PC4:

![Internet Connection (Cisco) (3).png](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/Cisco/Internet%20Connection%20(Cisco)%20(3).png)
![Internet Connection (Cisco) (4).png](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/Cisco/Internet%20Connection%20(Cisco)%20(4).png)

### MikroTik
In the MikroTik configuration, a firewall NAT rule is created to filter traffic, functioning similarly to an ACL in Cisco.

![Internet Connection (MikroTik).png](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/MikroTik/Internet%20Connection%20(MikroTik).png)

[Project File Link](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/MikroTik/Internet%20Connection%20(MikroTik).gns3project.7z) (extract the file first)

Internet connection test from PC1:

![Internet Connection (MikroTik) (1).png](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/MikroTik/Internet%20Connection%20(MikroTik)%20(1).png)
![Internet Connection (MikroTik) (2).png](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/MikroTik/Internet%20Connection%20(MikroTik)%20(2).png)

Internet connection test from PC3:

![Internet Connection (MikroTik) (3).png](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/MikroTik/Internet%20Connection%20(MikroTik)%20(3).png)
![Internet Connection (MikroTik) (4).png](https://github.com/eightball270/Cisco-and-MikroTik-Internet-Connection/blob/main/MikroTik/Internet%20Connection%20(MikroTik)%20(4).png)
