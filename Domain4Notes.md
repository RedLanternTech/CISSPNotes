# Note:  Not going to lie, I blew this domain off because its my strongest domain.  I will gladly take anyones suggestions.  

# OSI Model
**All People Seem To Need Data Processing**

- 7: Application:  HTTP, FTP, Telnet
- 6:  Presentation:  ASCII, Jpg, GIF, Midi
- 5:  Session:  NFS, SQL, RPC, Simplex, Duplex, 
- 4:  Transport:  TCP, UDP, SPX, SSL/TLS
- 3:  Network:  ICMP, RIP, IP, IPSec, NAT, Border Gateway Protocol
- 2:  Data Link:  PPP, ARP, l2f, L2TP, ISDN
- 1:  Physical:  EIA/TIA 232 and 449, X.21, .v25

## Attack vectors
- Layer 1:  passive sniffing, electrical interference, cutting wire, 
- Layer 2:  ARP Spoofing/MAC Address forging
- Layer 3:  Man-in-the-Middle Attacks, Spoofing or Forging IP addresses, Denial of Service Attacks
- Layer 4:  SYN Flood, Session hijacking
- Layer 5:  Depreciated SSL protocol, less secure versions of TLS, attacks on NETBIOS and NFS
- Layer 6:  Attacks on the encryption schemes themselves.
- Layer 7:  **Most Security breaches happen here**, Hitting weaknesss in protocols (HTTP, FTP, SMTP, SNMP), SQL Injections, 

## TCP/IP Model
- Application:  DNS, DHCP, SMTP, POP/IMAP, X-Windows
- Transport:  TCP, UDP
- Internet:  IP, ARP, IGMP, ICMP
- Link:  Ethernet

RFC 2828 defines IKE as an Internet, IPSec, key establishing protocol that is intended for putting in place authentication keying material for use with ISAKMP

As a note, NIST strong discourages BYOD.  It is best from a security standpoint to provide Employees devices the company controls.

## Firewalls 
- Static Pack Filtering Firewalls:  Straddles between Layer 3(network) and Layer 4 (Transport).  Simple, also called a screening router.  easiest to bypass/least secure
- Application level Firewalls:  Layer 7 (application).  Slow, complex, very secure.  Refered to as Gateway/Proxies.   
- Stateful inspection firewalls:  Layer 3 and 4.  Maintaines a record of what comes in and out.  Fast, harder to bypass, doesn't see data.  
- circuit-level firewalls:  Live on Layer 5.  No data inspection, operates like a stateful inspection firewall.  
- Next-Gen Firewalls:  IDS/IPS, Can operate at all/different levels of the OSI model.  Serve at application level firewalls.  UTM would fit here.

Multihomed Firewall:  Has more than one interface.  Everything runs though a single box (or cluster).  

Bastion Host/Screened Host:  AKA a Jump Box.  

Screened Subnet:  Two separate Firewalls.  Enterprise Lan -> First Firewall -> DMZ Network/Screen Network -> Firewall Two -> Internet.  Adds complexity.  

AWS "Security Groups" and Firewall as a service (FWaaS)

## Dumb Network items
Repeaters, Concentratos, and Amplifiers:  Operate at layer 1, a hub is a multiport repeater, **A Hub is a security risk**  

Bridges and Switches:  Does same as hub, Operates at Layer 2, filters traffic based on Mac address.  Spanning Tree Algorithm (STA):  blocks forwarding on redunant links.  Where colision domain gets broken down.  

Vlans.  We tag specific ports to be on vlans.  Switches can't route between vlans.  They are layer 2.  For the exam, switches don't do routing.  Routers do routing.  

**When you hear colision domain, think layer 2, When you hear broadcast domain, think layer 3.**

You may see BGP, OSPF and RIP on the exam.  BGP would be external, OSPF for areas, RIP is just listening to neighbors.  All happens at layer 3

Gateway's operate at all 7 layers of the osi model.  

Proxies Do not translate protocols like Gateways.  Operate at all 7 layers

Lan Extender:  Extends beyond 100M (328ft).  Work at Layer 2.  Temporary.  

## Ethernet 
- IEEE 802:3
- Most Common
- Usually star or Busch
- two-way full duplex
- Layer 2 technology
- PDU is the frame
- Carrier Senses multiple access - Collision detection

## Network Access Control .`
- Deny netwokr access to noncompliant devices
- yo have to lay out how to plan it, think before you buy.  Plan out policies.  
- pre-adminission:  evaluates access attemps and only allows entry to authorized devices and users
- post-admission:  reauthenticates users trying to enter a different part of the network .  also restricts lateral movment to limit the damage from cyber attacks.  
- Capative Portals.  There are 1000s of ways to do NAC 

## VPN
- PPTP:  Layer 2, oldest, not recommended.  Uses same protocols as PPP.  
- SSTP:  uses SSL
- Frame Relay:  emulates a switched network, operates at layer 1 and 2, typically used on WANs.  
- ATM:  used by IsPs on their private networks.  no routing, ATM cells are 53 bytes.  CBR, VBR, ABR, UBR.  
