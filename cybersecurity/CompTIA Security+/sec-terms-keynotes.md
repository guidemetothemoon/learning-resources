> These notes contain important properties, key words and examples related to crucial cybersecurity terms that I have collected and aggregated from multiple learning resources that have come in handy both during Sec+ certification but also as a cheat sheet later on. Hope you can benefit from these notes as well! :)

> Important note: this list is more useful for those who already have the foundational knowledge in place. Check out my book recommendations and core definition notes for more detailed foundational knowledge material.

### 7 data wipes are recommended

### 802.1x
Is used to prevent rogue access point to be plugged into network by authenticating user and device.

### Active Directory Federation Services (AD FS)
Software component for Windows that provides users with SSO access to systems & applications across organization boundaries or between partner organizations. Uses claims-based access control authorization model to maintain application security & implement federated identity. Is part of AD services.

### Access Control List (ACL)
- Used by router and firewall to block traffic by port, protocol or IP address.

### Ad-Hoc Mode
Devices connect in a mesh network as group of peers.

### Advanced Persistent Threat (APT)
Sophisticated attacks over a long period of time, often sponsored by state governments.

### Anti-spoofing
Checks source IP of external traffic coming into network and verifies if it matches IP range of internal network - if not, it's considered to be spoofed -> drop packet.

### Application proxy server
Is often used when client and server are incompatible for direct connection.

### ARP Poisoning - example
An email was sent but was never received by the intended recipient.

### Authentication
Validates credentials after those are provided.

### Basel III
Framework for banking industry security.

### Birthday attack
Exploits probability of hash collision.

### Block cipher - pros & cons
Disadvantage - encryption speed & error propagation.
Advantage - high diffusion & tampering immunity.

### Blue screen of death
Windows stop error, attributed to hardware problems.

### Bridge
- Segments networks into collision domains. Has less ports than switches (1 port == 1 collision domain).
- Optimize network usage by remembering which network segments MAC addresses are connected to.

### Certificate pinning
Prevents server from attacker updating the certificate.

### Certificate stapling
Used by web server to provide certificate validity.

### Certificate trust errors
Check if certificate is valid and is added to trusted root CA store on the local machine. Deleting local cache will remove certificate from trusted root CAs.

### CPU Throttling
Used to slow down processing -> reduces power consumption and heat.

### Data labeling
- Data owners decide how the data is labeled (top secret, public, etc.).

### DDoS mitigation
- Perimeter devices.
- Identify network traffic patterns.
- Filtering: connection tracking, IP reputation lists, deep packet inspection, blacklisting/whitelisting, rate limiting.
- Pass traffic for potential target network through high-capacity networks with "traffic scrubbing filters".

### Deprovision an app
First, remove access -> then backup data.

### DIAMETER
- Uses TCP, doesn't encrypt the message.

### Digital signature
Created with sender's private key and is verified with sender's public key.

### DNS server replication traffic
Uses TCP port 53.

### DNS user queries
Uses UDP port 53.

### Domain Name System Security Extensions (DNSSEC)
Uses digital signature based on public key cryptography: DNS data signed by owner of DNS zone with private key -> public key published for anyone to use -> when recursive resolver looks up data it uses public key to validate authenticity of DNS data (to prevent DNS response spoofing) -> results in data origin authentication & integrity.

### Download of unauthorized software
Reduces available bandwidth & amount of free disk space.

### Download third-party mobile application
- iOS: jailbreaking + sideloading
- Android: rooting (equivalent of jailbreaking for Android) + sideloading

### Due care
Taking steps to address a security problem like ensuring client data is confidential.

### Due diligence
Act of understanding security risks.

### Due process
Actions taken as a result of due care policy violation.

### Dynamic ARP inspection
Validates ARP packets in a network - discards those with invalid MAC to IP binding. Used against ARP poisoning (Man-in-the-Middle (MiTM) attack variation where MAC addresses are spoofed).

### FedRAMP
Federal risk & authorization management program, non-regulatory framework for providing recommendations on security best practices.

### File Transfer Protocols (FTPS, SFTP, SCP)
- FTPS: uses digital certificates to secure transfer.
- SFTP: uses SSH to secure transfer.
- SCP: secure copy, uses SSH to secure transfer.


### Firewall
- Often acts as VPN concentrator.
- Can be stateful, stateless, network-based, host-based, application-aware (next generation firewall).

### FISMA
Framework for protection of government data & assets against disastrous threats.

### Flow logs
Track outbound data from network interfaces of the server.

### Full-scale exercise
Near-real disaster incident, is expensive to execute.

### Functional excercise
Simulate disaster incident at more realistic level.

### Gray hat hacker
Discovers security flaws & makes these public - not for personal gain.

### Hardware Security Module (HSM)
Cryptographic processor that is used for securing cryptographic keys and provisioning encryption, decryption, authentication and digital signing services. Used in PKI, database encryption, SSL/TLS for web servers. Can generate and protect keys.

### Host Based Intrusion Detection/Protection System (HIDS/HIPS)
- Provides IP addresses and ports of both sender & receiver and protocol.

### HTTP response splitting
Leads to cross-site scripting attacks (XSS).

### IEEE 802.1x
Port-based network access protocol, can integrate with RADIUS and uses digital certificates to authenticate clients.

### Implicit deny
Any new access account will by default be denied all access. When a request is made for specific privileges for that account, those are explicitly applied.

### In-vehicle communication
Ad-hoc mesh network between vehicles, communication in plaintext, no firewall. Protocols used (CAN bus, FlexRay) ensure data integrity & availability but not authentication & confidentiality -> vulnerable to wireless jamming & spoofing.

### Incremental backup
Takes less time to backup but longer to restore.

### Infrastructure mode
Controlled by administrator, all traffic goes through Access Point (AP).

### Internet Key Exchange (IKE)
Used in setting up security associations in IPsec.

### Internet Protocol Security (IPsec)
- Authentication Header (AH) - provides authentication & integrity check, added to packet header (MD5, SHA-1, SHA-2).
- Encapsulating Security Payload (ESP) - provides encryption services, adds header + trailer + integrity check value (MD5, SHA-1, SHA-2, 3DES, AES).

### IoT devices
- Unable to update embedded firmware.

### Integrity checker (MS System File Checker)
Can determine if dll-s were tampered with.

### IP Spoofing defense
Packet filtering, encryption, key-based authentication.

### Kerberos
Protected against replay & eavesdropping, builds on symmetric key cryptography and requires trusted third-party. Uses UDP port 88.

### Layer 2 switches
Multiple collision domains, one broadcast domain.

### Layer 2 Tunneling Protocol (L2TP)
Protocol for VPN, could be used for site-to-site or remote access VPNs.

### Lightweight Directory Access Protocol (LDAP)
Protocol to communicate with directory services (like Active Directory (AD)). Has two authentication types:
- Simple authentication: anonymous/unauthenticated (logging only) or with password (insecure).
- Simple authentication and security (SASL): binds LDAP to authentication mechanism (like Kerberos). Uses TLS to keep username & password safe from network sniffers and alike.

### MAC (Message Authentication Code)
Provides message integrity, will reveal any data tampering.

### Mail protocols (IMAP, SMTP, PGP, S/MIME)
- IMAP (Internet Message Access Protocol) - used for receiving e-mails.
- SMTP (Simple Mail Transfer Protocol) - used for sending e-mails.
- PGP (Pretty Good Privacy) - used to encrypt e-mails, uses self-signed certificates.
- S/MIME (Secure/Multipurpose Internet Mail Extensions) - used to encrypt e-mails, uses X.509 certificates that are created & authenticated by a trusted third-party.

### MANET
Mobile ad-hoc network used for on-the-fly communication - every devices acts as a router.

### Mobile download manager
States how many connections are allowed and bandwidt amount that they're allowed to use.

### Mobile security
Least functionality on mobile - disable what's not in use.

### Near-field communication (NFC)
Maximum distance - 10 meters, two-way communication.

### NetBIOS (Network Basic Input / Output System)
Not routable network protocol, goes over TCP/IP (NBT). Microsoft protocol used long ago for file and print sharing, uses TCP port 139.

### Network Access Control (NAC)
Checks if device is fully patched (no viruses) before allowing it into the network.

### Network Based Intrusion Detection/Protection System (NIDS/NIPS)
- Passive monitoring -> examine traffic copy.
- Inline monitoring -> all traffic goes through IDS/IPS - allow/deny traffic in real-time.
- Out-of-band response -> if malicious traffic identified, IPS sends TCP RST (reset) frames, remote monitoring of device.
- In-band response -> local monitoring.
- Available system types: signature-based, anomaly-based, behaviour-based, heuristic-based.
- NIDS should be put in front of and behind firewall.
- Provides IP addresses and ports of both sender & receiver and protocol.

### NTLM (Windows NT LAN Manager)
negotiate_msg from client -> challenge_msg from server -> authenticate_msg from client. 128 bits password hashes - two of them (DES or MD4). Used mainly for compatibility with older systems.

### Non-repudiation
Presents the denial from someone/something of having sent a transmission or making a change to data.

### OAuth
Provides access delegation, token-based. Is more an authorization protocol.

### OpenID
Authentication protocol, uses single set of user credentials to access multiple sites.

### OpenID Connect
Identity layer on top of OAuth 2.0 that allows computer clients to verify identity of end-user based on authentication performed by authorized server and obtain basic profile information about end-user in a RESTful manner.

### Operations-based excercise
Validates plans identified after table-top exercise, in an environment that simulates real-life incident.

### OSI (Open Systems Interconnect) Model - layers
- L1: Physical layer, deals with physical transmission mediums like physical connectors.
- L2: Data link layer, deals with MAC addresses.
- L3: Network layer, deals with IP addresses.
- L4: Transport layer, dealts with port addresses.
- L5: Session layer, deals with connections (sessions) between local and remote applications.
- L6: Presentation layer, formats data to be sent across network.
- L7: Application layer, closest to the user, interact directly with software application.


### PKI (Public Key Infrastructure)
- User 1 encrypts with public key of user 2 -> user 2 decrypts with private key of user 2.
- User 2 encrypts with public key of user 1 -> user 1 decrypts with private key of user 1.

### Port forwarding
Technique that is often used in terms of Network Address Translation (NAT) - it redirects communication request from one address & port number combination to another while packets are traversing network gateway.

### Port security
Prevents from someone plugging laptop into network.

### Private cloud
Self-service & virtualization.

### Radio Frequency Identification (RFID)
Maximum distance - 3 meters, one-way communication. Uses encoded memory chip - RFID reader.

### RADIUS
- Uses UDP.

### RAID
Implemented for performance & data redundancy.

### Reverse brute-force - mitigation
Establish password policy that disallows common passwords.

### Reverse engineering
Man-made object is de-constructed to reveal it's designs, architecture, code, etc.

### Robocalling
Places unsolicited telemarketing calls.

### Root Certificate Authority (CA) name and public key
Only included in root certificate, not in end-user certificate.

### Root of Trust (RoT)
Source that can always be relied on within a cryptographic system.

### Router
Results in multiple broadcast domains -> broadcast transmissions don't traverse routers. Forwards traffic between subnets.

### Security misconfiguration - example
Assigned permissions that shouldn't be assigned in the first place.

### Security templates
Standardization of security settings.

### Self-encrypting drive (SED)
Provides automatic encryption & decryption.

### Server affinity (Load Balancer)
Ability of Load Balancer or router to send a user's request to the same server where their session was initiated.

### Shunning
Ignore attack (f.ex., when it is not relevant/applicable).

### Sideloading
Transfers data between two devices. Is associated with installing applications to Android from other places than Google Play (f.ex., USB).

### SIEM
- SIEM correlation - Helps compare events from different logs to link them together.
- Monitors wrong attacks (false positives) -> reason for that may be wrong input filters.

### Simple Service Discovery Protocol (SSDP)
Self-managing network service discovery standard.

### Single hub
One collision and one broadcast domain.

### Single Sign-On (SSO) common configurations
- Kerberos-based
- Smart card-based
- Integrated Windows Authentication
- SAML (Security Assertion Markup Language)

### Smartcard
Is 2FA (two-factor authentication) - something you know and something you have.

### Smurf attack
Distributed Denial of Service (DDoS) attack where large numbers of Internet Control Message Protocol (ICMP) packets with intended victim's spoofed source IP are broadcasted to computer network.

### Software-defined networking (SDN) - layers
Application Layer (Business apps) -(API)-> Control Layer (Network services) -> Infrastructure layer.

### Sparse infector virus
Only infects files when certain conditions are met (f.ex., only on 10th execution or only 128kB files). Uses conditions to infect less often.

### SSL Offload (Load Balancer)
Moves out complex calculations for encryption/decryption of secured data from web/app servers.

### Stateful Packet Inspection (SPI)
Looks at entire context of conversation, used against TCP SYN flood.

### Storage segmentation
Applies through mobile device management (MDM), helps to impose different access controls on specific types of data.

### Switch
- Optimize network usage by remembering which network segments MAC addresses are connected to.
- Assigning specific MAC addresses to specific switch ports enables control of which stations can connect to which switch ports.

### Subnet
- Formula to determine size of subnet based in CIDR: (2^(32-N))-2, where N=(/nr).

### TACACS+
- Uses TCP.

### TCP Offload (Load Balancer)
Reduces overhead with opening/closing TCP sockets, reduces total number of connections needed without impacting application's capacity.

### Tethering
When laptop get internet connection from the phone.

### To discover disable SSID (Service Set Identifier)
Use wireless packet sniffer or perform SSID de-cloak.

### Transport mode
Internal, doesnt encrypt header -> between servers.

### Trivial File Transfer Protocol (TFTP)
Allows file storage without requiring username & password.

### Tunnel mode
If data leaves the network -> over the Internet.

### Unified Threat Management (UTM)
Single device that combines security devices like anti-virus, HIDS (Host-based Intrusion Detection System), log monitoring, firewall, etc.

### USB OTG (On-The-Go)
Use of portable devices as USB.

### Virtual IP Load Balancing
Doesn't take load of each interface into account & assumes that all loads are similar.

### VM Shielding
Security mechanism used to prevent hypervisor administrators from accessing VM content while having the ability to manage the VM itself.

### Voice over Internet Protocol (VOIP) protocols (RTP, SIP)
- RTP (Real-time Transport Protocol): protocol for transmitting VOIP.
- SIP (Session Initiation Protocol): protocol to initiate a VOIP call.

### War dialing
Dialing numbers hoping a computer modem answers.

### Weighted Round Robin
Assigns weighs to each server based on criteria like traffic-handling capacity.

### WiFi Direct
Communication without Access Point (AP), authentication with PIN.

### Windows Integrated Authentication
For use in intranets where all clients are on single domain. Current Windows user information on client PC is supplied by web browser through cryptographic exchange -> hashing with web server. If it fails -> use username & password.

### WINS (Windows Internet Name Service) server
Resolves NetBIOS computer names to IP addresses.

### Wireless Access Point (WAP)
- Fat: has all needed functionality, ability to traffic between wired interfaces like L2/L3 vswitch & MAC filtering -> no other servers or devices are required.
- Thin: requires some server or device to offload some functionality to.

### Wireless Packet Sniffer
Used to diagnose wireless access point (AP) problems.

### WPA (Wi-Fi Protected Access)
- Uses TKIP (Temporal Key Integrity Protocol).

### WYOD (Wear Your Own Device)
Wearable tech like smart watch or Google glasses.