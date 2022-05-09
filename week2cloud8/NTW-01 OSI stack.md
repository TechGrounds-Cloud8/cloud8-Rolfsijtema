# [Subject]
leer wat OSI model inhoud en TCP/IP

## Key terminology
OSI  Open Systems Internetconnection Model, bestaad uit 7 lagen, bijvoorbeeld laag 1 gaat over het controleren van kabels/hardware of alles werkt en correct is aangesloten. 

TCP/IP is alternatief, is meer opgebouwd zoals het internet is gebouwd.  1 op 1 benadering.

## Exercise
The OSI model and its uses. 
7 layers of OSI

7 Application:  network HTTP Internet, interactive applications de programma's
alle Internet explorers, outlook/office, zoom, skype,  

6 presentation: 
Syntax processing: converting data voorbeeld: Shopping:converting --> encrypting. 
data tussen de webshop naar de achterliggende afdelingen/bezorgdienst/betaling. 

5 Session:
het tot stand komen van een verbinding. 
Dit gaat over meerdere typen verbindingen, controlleer ook authentications als er een verbinding verbroken is en opnieuw tot stand komt.

4 Transport: 
Dit heet TCP (transmission Controlled Protocol,  of UDP: User Datagram Protocol.
Gaat letterlijk over het vervoeren/verzenden van de data over het netwerk. Controleert de verbinding tussen alle applicatie's, zorgt ook voor controle en veilighgeid.   error recovery, data re-transmission. het zorgt voor een betrouwbare verbinding, en lost het automatisch op als de informatie niet goed of onvolledig is doorgekomen. 
 
 
3 network
ZOrgt voor het correct routen van de te verzenden data, het controlleerd tevens of de data is aangekomen, denk aan emailadres wat niet klopt, je krijgt een melding in jou inbox.  ARP: Adres Resolution Protocol. kan IP adressen zijn of bijv; een printer. 

2 Data Link
Dit is de laag waar alle verbindingen worden gemanaged. Wifi, ethernet. De verbindingen / apparaten hebben een MAC adres, denk aan je printer. 
Mac-adres: Media Acces Control 
LLC: Logical Link Control  
![screenshot](../00_includes/Datalink%20layer.png)

1 Physical 
Hier worden de electrische verbindingen gemaakt, dus letterlijk de data via de kabel naar de printer/glasvezel/wifi/usb/thunderbolt. Wifi 802.11
electrical Mechanical Radiosignals.   Er zijn standaard protocols hiervoor bij het ontwerpen van een nieuw apparaat. "waar moeten ze aan voldoen om te kunnen communiceren"
![screenshot](../00_includes/Electrical%20divices.png)

Onderwerp: 
The TCP/IP model and its uses.

TCP  Transmission Control Protocol
Ip: Internet Protocol
TCP/IP een model om het internet en alles er omheen te standariseren. 
![screenshot](../00_includes/TCP%3AIP%20Layers.png)

 TCP/IP model is geupdate: er is 1 laag bijgekomen 
 [Screenshot](../00_includes/TCP%3AIP%20Layers.png)

Alle lagen met hun hun protocols:
![screenshot](../00_includes/Layers%20met%20protocols.png)

Layers/protocols: 

5: Application Layer: programma's om de data aan te maken welke verzonden dient te worden. 

4:Transport layer: TCP Data: data transportlayer waar de verzending klaargemaakt wordt.

3 Network Link Layer: Beheert het transport van data pakkage: IP TCP Data  "Packet" is klaar voor verzending er wordt een verbinding gemaakt met een IP adres. IP-protocol en TCP protocol maken samen de verbinding, TCP is de technology in jou computer/telefoon die het mogelijk maakt om de verbinding te maken. adressing/routing/en pakkage. 

2 Data Link Layer: IP TCP Data Ethernet: maakt de verbinding tussen de data en de fysiek.  Het omzetten van een file naar de printer bijvoorbeeld. 

1 Link Layer  kabels/wifi/enz.. hardware verbindingen maken. 
 


 
### Sources
OSI model: https://www.youtube.com/watch?v=Ilk7UXzV_Qc

TCP/IP   https://www.youtube.com/watch?v=tnAW02zvFhU

### Overcome challanges
verschil begrijpen tussen OSI TCP/IP

### Results
zie bovenstaande info als uitwerking opdracht. 