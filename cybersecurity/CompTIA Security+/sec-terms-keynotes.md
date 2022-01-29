> These notes contain important properties, key words and examples related to crucial cybersecurity terms that I have collected and aggregated from multiple learning resources that have come in handy both during Sec+ certification but also as a cheat sheet later on. Hope you can benefit from these notes as well! :)

### Ad-Hoc Mode
Devices connect in a mesh network as group of peers

### Advanced Persistent Threat (APT)
Sophisticated attacks over a long period of time, often sponsored by state governments

### ARP Poisoning - example
An email was sent but was never received by the intended recipient

### Basel III
Framework for banking industry security

### Block cipher - pros & cons
Disadvantage - encryption speed & error propagation
Advantage - high diffusion & tampering immunity

### Certificate pinning
Prevents server from attacker updating the certificate

### Certificate stapling
Used by web server to provide certificate validity

### Deprovision an app
First, remove access -> then backup data

### Dynamic ARP inspection
Validates ARP packets in a network - discards those with invalid MAC to IP binding. Used against ARP poisoning (Man-in-the-Middle (MiTM) attack variation where MAC addresses are spoofed)

### FedRAMP
Federal risk & authorization management program, non-regulatory framework for providing recommendations on security best practices

### Firewall often acts as VPN concentrator

### FISMA
Framework for protection of government data & assets against disastrous threats

### Flow logs
Track outbound data from network interfaces of the server

### Full-scale exercise
Near-real disaster incident, is expensive to execute

### Functional excercise
Simulate disaster incident at more realistic level

### HTTP response splitting
Leads to cross-site scripting attacks (XSS)

### In-vehicle communication
Ad-hoc mesh network between vehicles, communication in plaintext, no firewall. Protocols used (CAN bus, FlexRay) ensure data integrity & availability but not authentication & confidentiality -> vulnerable to wireless jamming & spoofing

### Incremental backup
Takes less time to backup but longer to restore

### Infrastructure mode
Controlled by administrator, all traffic goes through Access Point (AP)

### Internet Protocol Security (IPsec)
- Authentication Header (AH) - provides authentication & integrity check, added to packet header (MD5, SHA-1, SHA-2)
- Encapsulating Security Payload (ESP) - provides encryption services, adds header + trailer + integrity check value (MD5, SHA-1, SHA-2, 3DES, AES)

### IP Spoofing defense
Packet filtering, encryption, key-based authentication

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

### Operations-based excercise
Validates plans identified after table-top exercise, in an environment that simulates real-life incident

### PKI (Public Key Infrastructure)
- User 1 encrypts with public key of user 2 -> user 2 decrypts with private key of user 2
- User 2 encrypts with public key of user 1 -> user 1 decrypts with private key of user 1

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

### Root Certificate Authority (CA) name and public key
Only included in root certificate, not in end-user certificate

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

### Smurf attack
Distributed Denial of Service (DDoS) attack where large numbers of Internet Control Message Protocol (ICMP) packets with intended victim's spoofed source IP are broadcasted to computer network

### Software-defined networking (SDN) - layers
Application Layer (Business apps) -(API)-> Control Layer (Network services) -> Infrastructure layer

### Sparse infector virus
Only infects files when certain conditions are met (f.ex., only on 10th execution or only 128kB files). Uses conditions to infect less often.

### Storage segmentation
Applies through mobile device management (MDM), helps to impose different access controls on specific types of data

### Transport mode
Internal, doesnt encrypt header -> between servers

### Tunnel mode
If data leaves the network -> over the Internet

### WiFi Direct
Communication without Access Point (AP), authentication with PIN
