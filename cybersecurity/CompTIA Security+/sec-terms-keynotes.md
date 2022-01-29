> These notes contain important properties, key words and examples related to crucial cybersecurity terms that I have collected and aggregated from multiple learning resources that have come in handy both during Sec+ certification but also as a cheat sheet later on. Hope you can benefit from these notes as well! :)

### Tunnel mode
If data leaves the network -> over the Internet

### Transport mode
Internal, doesnt encrypt header -> between servers

### PKI (Public Key Infrastructure)
- User 1 encrypts with public key of user 2 -> user 2 decrypts with private key of user 2
- User 2 encrypts with public key of user 1 -> user 1 decrypts with private key of user 1

### Deprovision an app
First, remove access -> then backup data

### Block cipher - pros & cons
Disadvantage - encryption speed & error propagation
Advantage - high diffusion & tampering immunity

### HTTP response splitting
Leads to cross-site scripting attacks (XSS)

### Security misconfiguration - example
Assigned permissions that shouldn't be assigned in the first place

### WiFi Direct
Communication without Access Point (AP), authentication with PIN

### Infrastructure mode
Controlled by administrator, all traffic goes through Access Point (AP)

### Ad-Hoc Mode
Devices connect in a mesh network as group of peers

### MANET
Mobile ad-hoc network used for on-the-fly communication - every devices acts as a router

### Incremental backup
Takes less time to backup but longer to restore

### Security templates
Standardization of security settings

### ARP Poisoning - example
An email was sent but was never received by the intended recipient

### Flow logs
Track outbound data from network interfaces of the server

### Software-defined networking (SDN) - layers
Application Layer (Business apps) -(API)-> Control Layer (Network services) -> Infrastructure layer

### Private cloud
Self-service & virtualization

### Reverse brute-force - mitigation
Establish password policy that disallows common passwords

### In-vehicle communication
Ad-hoc mesh network between vehicles, communication in plaintext, no firewall. Protocols used (CAN bus, FlexRay) ensure data integrity & availability but not authentication & confidentiality -> vulnerable to wireless jamming & spoofing

### RAID
Implemented for performance & data redundancy

### IP Spoofing defense
Packet filtering, encryption, key-based authentication

### Storage segmentation
Applies through mobile device management (MDM), helps to impose different access controls on specific types of data

### SIEM correlation
Helps compare events from different logs to link them together

### Certificate pinning
Prevents server from attacker updating the certificate

### Certificate stapling
Used by web server to provide certificate validity

## Root Certificate Authority (CA) name and public key
Only included in root certificate, not in end-user certificate 