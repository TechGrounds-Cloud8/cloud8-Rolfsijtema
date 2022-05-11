# [Subnetting]
When 2 or more divices are connected we call it a Local Area Network (LAN), every host(device) has its own adres in this range. A Subnet Mask helps to (prefix) all this adresses, how many "bits" of the networkadres are reserved for the host/devices. A subnet is a smaller network within a bigger network. the subnet has a larger prefix than the larger network it is connected to. Subnet logically isolates the devices/host. 

## Key terminology
CIDR notation: 
(Classless Inter-Domain Routing) is an alternate method of representing a subnet mask. It is simply a count of the number of network bits (bits that are set to 1) in the subnet mask.

Subnet:
A subnet mask is a 32-bit number created by setting host bits to all 0s and setting network bits to all 1s. In this way, the subnet mask separates the IP address into the network and host addresses
![subnet](../00_includes/subnet%20mask.png)

Prefix:
Prefix is a measurement to quantify large number. In networking, prefix is used to quantify large number of hosts/networks - 10.0.0.0/8 and 10.0.0.0/24 is a prefix. My definition of BGP Prefix is a large number of networks learned via BGP Routing Protocol.

Bits:
Image result for bits in networking
The terms bits and bytes in computer networking refer to standard units of digital data transmitted over network connections. There are 8 bits for every 1 byte.



## Exercise

### Sources
[List your sources you used for solving the exercise]

### Overcome challanges
[Give a short description of your challanges you encountered, and how you solved them.]

### Results
Maak een netwerkarchitectuur die voldoet aan de volgende eisen:
1 private subnet dat alleen van binnen het LAN bereikbaar is. Dit subnet moet minimaal 15 hosts kunnen plaatsen.
1 private subnet dat internet toegang heeft via een NAT gateway. Dit subnet moet minimaal 30 hosts kunnen plaatsen (de 30 hosts is exclusief de NAT gateway).
1 public subnet met een internet gateway. Dit subnet moet minimaal 5 hosts kunnen plaatsen (de 5 hosts is exclusief de internet gateway).
Plaats de architectuur die je hebt gemaakt inclusief een korte uitleg in de Github repository die je met de learning coach hebt gedeeld.
