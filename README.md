# datacom


# Dit zijn allemaal voorbelden.
- Show spanning-tree: met dit commando kun je zien welke vlan’s er root zijn op de switch waar je nu op zit. Je kunt deze link gebruiken voor hulp (Link)
 
- Show vlan br: dit commando laat zien welke vlan’s er op het apparaat staan, waar je bent ingelogd.
 
- Spanning-tree vlan 1 root primary: dit is het commando om een vlan op root te zetten op het apparaat waar je bent ingelogd. (vlan 1 is een voorbeeld het kan anders zijn)
 
- Ip dhcp excluded-address 192.168.12.1 – 192.168.12.60: Dit is hoe je een exclusion aan maakt voor een DHCP. (het ip address is een voorbeeld)
 
- VTP Domain (Naam Domain): hiermee kun je de naam van een domain maken.
 
- VTP Mode Server/Client: met dit commando kun je instellen of het een server word of client.
 
- ssh -l "user"  "ip van het apparaat"

In het aparaat komen
 
- password: cisco
 
- password class
 
- show cdp neighbors

Laat zien welke devices gekoppeld zijn
 
- cdp entry device naam

Informatie zien van apparaat
 
Show inter trunk: om te zien welke poorten in trunk zitten
 
Show vtp status: status van vtp zien
 
in de interface van vlan(name naamvlan): om naam van de vlan te wijzigen
 
show interface gig 0/0/1: Informatie over een poort zien
 
Show MAC adress table: gebruik dit op de switch om het MAC-adres van de PC te achterhalen
 
Ping eerst met de twee PC's zodat de switches kennis maakt met de PC's

Dan kan je zien aan welke poorten de MAC-Adres zit
 
Standby ip 192.168.10.1(voorbeeld ip): dit commando voer je uit in de interface van de vlan om een ip als standby in te stellen
 
standby priority 255

standby preempt(dit doe je ook in de interface van de vlan)
 
 
 
Multi layer switch
 
Int range gig 1/0/2 -5
 
Swmode acces trunk
 
VTP Domain guus
 
VTP mode server
 
Int vlan 10
 
Ip add 192.168.10.1
 
Ip dhcp pool v10
 
Network 192.168.10.0 255.255.255.0
 
Default router 192.168.10.1
 
dns 68.98.54.1(voorbeeld ip)
 
 
Switch
 
Vtp domain
 
Vtp mode client
 
Int range fa0/1 -5
 
Swport mode acces
 
Swport acces vlan 10
 
Int range fa0/6 -10
 
Swport mode acces
 
Swport acces vlan 20
 
Int range fa0/11 -15
 
Swport mode acces
 
Swport acces vlan 30
 
Int range fa0/16 - 20
 
Swport mode acces
 
Swport acces vlan 40
 
Int range fa0/21 - 24
 
Swport mode acces
 
Swport acces vlan 50
