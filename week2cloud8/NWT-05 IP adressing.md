# [IP adressen]
How are IPadresses created. How did they excisted, are there enough? IPV6 or NAT inside IPV4 

## Key terminology

IP adressen
IPv4 en IPv6
Public en Private IPs
NAT
Statische en dynamische adressen

## Exercise
See results 
IP adressen: 
is a logic adres that can be connected to a networkdivices such as a PC or Router 192.168.0.1
IPv4: ip4 has 32bits but options are ended. so they invented ipv6
IPv6: IPV6 had 128bits has more options than we need on this planet. 

Public IP:  Public IP is an adres accesable from the internet.
Private IPs is an adres within the router/network. 

NAT:The NAT router checks the routing table to see if it has an entry for the destination address. If it does, the NAT router then translates the packet and creates an entry for it in the address translation table. If the destination address is not in the routing table, the packet is dropped.

Statische adresses or dynamische adressen: 
What is the difference between a dynamic and static IP address? When a device is assigned a static IP address, the address does not change. Most devices use dynamic IP addresses, which are assigned by the network when they connect and change over time.

Er zijn 3 IP adres bereiken gereserveerd voor privé netwerken.
192.168.0.0 - 192.168.255.255
172.16.0.0 - 172.31.255.255
10.0.0.0 - 10.255.255.255

Important note: In AWS you need to turn-on the ipv6 option!!! otherwise it only works with IPV4 adresses

### Sources
Therms searched via Google and [www.quora.com]

Change ip computer to phone. 
[https://www.google.com/search?q=what+happends+when+you+change+your+ip+adress+of+your+phone+to+the+computers+one&oq=what+happends+when+you+change+your+ip+adress+of+your+phone+to+the+computers+one+&aqs=chrome..69i57.35111j0j4&sourceid=chrome&ie=UTF-8]

Private adres changing on mobile phone
[https://www.quora.com/Does-your-IP-address-change-using-a-mobile-phone-with-data]


### Overcome challanges
difficult to change IP inside router enviroment. 

### Results
1 Ontdek wat je publieke IP adres is van je laptop en mobiel op wifi.
Mobile:     192.168.x.xx   Internal IPadres, only public true the router. 
Computer:   192.168.x.xxx  Pulic adres

2 Zijn de adressen hetzelfde of niet? Leg uit waarom.
No, they are diffirent because they are personal to each device.
Mobile IP is internal from the router.
Computer is public IP.

3 Verander het privé IP adres van je mobiel naar dat van je laptop. Wat gebeurt er dan?

4 When you change the IP adres of ur phone the internetconnection stops, when you connect to your WIFInetwork the router will change it back and so it makes the connection again. 

Does changing IP address affect anything?
Keep in mind, changing your IP address will temporarily disrupt whatever internet-connected services or programs you're using on your device. There's no harm done, but it's going to have the same effect as if you'd momentarily lost your Wi-Fi.

5 Probeer het privé IP adres van je mobiel te veranderen naar een adres buiten je netwerk. Wat gebeurt er dan?

your IP address changes on any network you're using either being mobile or Wi-Fi.
Your cellular carrier will assign a temporary IP address to your device whenever you begin a new data session, or periodically refresh the IP address assigned if your device connects continuously.
The IP address ‘lease’ time is fairly short (typically 48 hours). A complete record of the IP addressed assigned to a device is retained for a considerable length of time (months or years), and in many cases permanently. This allows forensic investigators to determine which device participated in any given data exchange.
