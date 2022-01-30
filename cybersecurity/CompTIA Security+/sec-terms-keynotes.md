> These notes contain important properties, key words and examples related to crucial cybersecurity terms that I have collected and aggregated from multiple learning resources that have come in handy both during Sec+ certification but also as a cheat sheet later on. Hope you can benefit from these notes as well! :)

### Ad-Hoc Mode
Devices connect in a mesh network as group of peers

### Advanced Persistent Threat (APT)
Sophisticated attacks over a long period of time, often sponsored by state governments

### Application proxy server
Is often used when client and server are incompatible for direct connection

### ARP Poisoning - example
An email was sent but was never received by the intended recipient

### Basel III
Framework for banking industry security

### Birthday attack
Exploits probability of hash collision

### Block cipher - pros & cons
Disadvantage - encryption speed & error propagation
Advantage - high diffusion & tampering immunity

### Certificate pinning
Prevents server from attacker updating the certificate

### Certificate stapling
Used by web server to provide certificate validity

### DDoS mitigation
- Perimeter devices
- Identify network traffic patterns
- Filtering: connection tracking, IP reputation lists, deep packet inspection, blacklisting/whitelisting, rate limiting
- Pass traffic for potential target network through high-capacity networks with "traffic scrubbing filters"

### Deprovision an app
First, remove access -> then backup data

### Domain Name System Security Extensions (DNSSEC)
Uses digital signature based on public key cryptography: DNS data signed by owner of DNS zone with private key -> public key published for anyone to use -> when recursive resolver looks up data it uses public key to validate authenticity of DNS data (to prevent DNS response spoofing) -> results in data origin authentication & integrity

### Dynamic ARP inspection
Validates ARP packets in a network - discards those with invalid MAC to IP binding. Used against ARP poisoning (Man-in-the-Middle (MiTM) attack variation where MAC addresses are spoofed)

### FedRAMP
Federal risk & authorization management program, non-regulatory framework for providing recommendations on security best practices

### File Transfer Protocols (FTPS, SFTP, SCP)
- FTPS: uses digital certificates to secure transfer
- SFTP: uses SSH to secure transfer
- SCP: secure copy, uses SSH to secure transfer


### Firewall
- Often acts as VPN concentrator
- Can be stateful, stateless, network-based, host-based, application-aware (next generation firewall)

### FISMA
Framework for protection of government data & assets against disastrous threats

### Flow logs
Track outbound data from network interfaces of the server

### Full-scale exercise
Near-real disaster incident, is expensive to execute

### Functional excercise
Simulate disaster incident at more realistic level

### Hardware Security Module (HSM)
Cryptographic processor that is used for securing cryptographic keys and provisioning encryption, decryption, authentication and digital signing services. Used in PKI, database encryption, SSL/TLS for web servers. Can generate and protect keys

### Host Based Intrusion Detection/Protection System (HIDS/HIPS)
- Provides IP addresses and ports of both sender & receiver and protocol

### HTTP response splitting
Leads to cross-site scripting attacks (XSS)

### Implicit deny
Any new access account will by default be denied all access. When a request is made for specific privileges for that account, those are explicitly applied

### In-vehicle communication
Ad-hoc mesh network between vehicles, communication in plaintext, no firewall. Protocols used (CAN bus, FlexRay) ensure data integrity & availability but not authentication & confidentiality -> vulnerable to wireless jamming & spoofing

### Incremental backup
Takes less time to backup but longer to restore

### Infrastructure mode
Controlled by administrator, all traffic goes through Access Point (AP)

### Internet Key Exchange (IKE)
Used in setting up security associations in IPsec

### Internet Protocol Security (IPsec)
- Authentication Header (AH) - provides authentication & integrity check, added to packet header (MD5, SHA-1, SHA-2)
- Encapsulating Security Payload (ESP) - provides encryption services, adds header + trailer + integrity check value (MD5, SHA-1, SHA-2, 3DES, AES)

### IP Spoofing defense
Packet filtering, encryption, key-based authentication

### Layer 2 Tunneling Protocol (L2TP)
Protocol for VPN, could be used for site-to-site or remote access VPNs

### Lightweight Directory Access Protocol (LDAP)
Protocol to communicate with directory services (like Active Directory (AD)). Has two authentication types:
- Simple authentication: anonymous/unauthenticated (logging only) or with password (insecure)
- Simple authentication and security (SASL): binds LDAP to authentication mechanism (like Kerberos). Uses TLS to keep username & password safe from network sniffers and alike 

### Mail protocols (IMAP, SMTP, PGP, S/MIME)
- IMAP (Internet Message Access Protocol) - used for receiving e-mails
- SMTP (Simple Mail Transfer Protocol) - used for sending e-mails
- PGP (Pretty Good Privacy) - used to encrypt e-mails, uses self-signed certificates
- S/MIME (Secure/Multipurpose Internet Mail Extensions) - used to encrypt e-mails, uses X.509 certificates that are created & authenticated by a trusted third-party

### MANET
Mobile ad-hoc network used for on-the-fly communication - every devices acts as a router

### Mobile security
Least functionality on mobile - disable what's not in use

### Near-field communication (NFC)
Maximum distance - 10 meters, two-way communication

### Network Based Intrusion Detection/Protection System (NIDS/NIPS)
- Passive monitoring -> examine traffic copy
- Inline monitoring -> all traffic goes through IDS/IPS - allow/deny traffic in real-time
- Out-of-band response -> if malicious traffic identified, IPS sends TCP RST (reset) frames, remote monitoring of device
- In-band response -> local monitoring
- Available system types: signature-based, anomaly-based, behaviour-based, heuristic-based
- NIDS should be put in front of and behind firewall
- Provides IP addresses and ports of both sender & receiver and protocol

### Operations-based excercise
Validates plans identified after table-top exercise, in an environment that simulates real-life incident

### PKI (Public Key Infrastructure)
- User 1 encrypts with public key of user 2 -> user 2 decrypts with private key of user 2
- User 2 encrypts with public key of user 1 -> user 1 decrypts with private key of user 1

### Port forwarding
Technique that is often used in terms of Network Address Translation (NAT) - it redirects communication request from one address & port number combination to another while packets are traversing network gateway

### Private cloud
Self-service & virtualization

### Radio Frequency Identification (RFID)
Maximum distance - 3 meters, one-way communication. Uses encoded memory chip - RFID reader

### RAID
Implemented for performance & data redundancy

### Reverse brute-force - mitigation
Establish password policy that disallows common passwords

### Reverse engineering
Man-made object is de-constructed to reveal it's designs, architecture, code, etc.

### Robocalling
Places unsolicited telemarketing calls

### Root Certificate Authority (CA) name and public key
Only included in root certificate, not in end-user certificate

### Root of Trust (RoT)
Source that can always be relied on within a cryptographic system

### Security misconfiguration - example
Assigned permissions that shouldn't be assigned in the first place

### Security templates
Standardization of security settings

### Server affinity (Load Balancer)
Ability of Load Balancer or router to send a user's request to the same server where their session was initiated

### Shunning
Ignore attack (f.ex., when it is not relevant/applicable)

### SIEM correlation
Helps compare events from different logs to link them together

### Single Sign-On (SSO) common configurations
- Kerberos-based
- Smart card-based
- Integrated Windows Authentication
- SAML (Security Assertion Markup Language)

### Smurf attack
Distributed Denial of Service (DDoS) attack where large numbers of Internet Control Message Protocol (ICMP) packets with intended victim's spoofed source IP are broadcasted to computer network

### Software-defined networking (SDN) - layers
Application Layer (Business apps) -(API)-> Control Layer (Network services) -> Infrastructure layer

### Sparse infector virus
Only infects files when certain conditions are met (f.ex., only on 10th execution or only 128kB files). Uses conditions to infect less often

### SSL Offload (Load Balancer)
Moves out complex calculations for encryption/decryption of secured data from web/app servers

### Stateful Packet Inspection (SPI)
Looks at entire context of conversation, used against TCP SYN flood

### Storage segmentation
Applies through mobile device management (MDM), helps to impose different access controls on specific types of data

### TCP Offload (Load Balancer)
Reduces overhead with opening/closing TCP sockets, reduces total number of connections needed without impacting application's capacity

### Transport mode
Internal, doesnt encrypt header -> between servers

### Tunnel mode
If data leaves the network -> over the Internet

### Unified Threat Management (UTM)
Single device that combines security devices like anti-virus, HIDS (Host-based Intrusion Detection System), log monitoring, firewall, etc.

### Virtual IP Load Balancing
Doesn't take load of each interface into account & assumes that all loads are similar

### Voice over Internet Protocol (VOIP) protocols (RTP, SIP)
- RTP (Real-time Transport Protocol): protocol for transmitting VOIP
- SIP (Session Initiation Protocol): protocol to initiate a VOIP call 

### War dialing
Dialing numbers hoping a computer modem answers

### Weighted Round Robin
Assigns weighs to each server based on criteria like traffic-handling capacity

### WiFi Direct
Communication without Access Point (AP), authentication with PIN

### Wireless Access Point (WAP)
- Fat: has all needed functionality, ability to traffic between wired interfaces like L2/L3 vswitch & MAC filtering -> no other servers or devices are required
- Thin: requires some server or device to offload some functionality to