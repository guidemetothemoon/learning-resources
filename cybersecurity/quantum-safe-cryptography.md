# Quantum-Safe Cryptography

With acceleration of development of quantum computers it has become clear that current cryptographic techniques and cryptographic algorithms will face great challenges once quantum computers become publicly available. Current data protection mechanisms heavily rely on a collection of well-proven and well-known cryptographic algorithms. These cryptographic algorithms were built so that they can't be broken with computing power that is currently available. With advancement and public availability of quantum computers such implementations will become pretty easy and straightforward to solve which makes establishment and standardization of quantum-safe cryptography critically important.

What makes the whole situation even scarier is the fact that a malicious actor can steal data that's safely encrypted now and keep it stored until a quantum computer with enough computing power becomes available. Once it's available, all encrypted data can potentially be easily decrypted. This means that **all data that has ever been in-transit or at-rest will become vulnerable to disclosure**.

Not all cryptographic algorithms are currently confirmed to be vulnerable to quantum attacks but this may change with time and more research. Symmetric encryption algorithms like AES can still be quantum-safe by increasing the key size. Most of the asymmetric encryption algorithms are not quantum-safe due to the fact that they're based upon Integer Factoring and Discrete Logarithms complexities which can be resolved with quantum computing. For example, security protocols like TLS, SSH, S/MIME and IKE will be affected by quantum vulnerabilities and will need to be upgraded to be quantum-safe.

It has also become clear that many security protocols are lacking cryptographic agility which means that it makes it extremely hard to extend and improve them in order to make them quantum-safe.

These are some of the factors that make quantum-safe cryptography a complex task to complete. All the existing security protocols and encryption algorithms have been tested, researched and standardized for years. Historically, it has taken almost two decades to deploy our modern public key cryptography infrastructure so you can imagine that creating a new standard for quantum-safe cryptography under current time constraints and the level of urgency is far from an easy task. 

Back in 2016 NIST has started a process for discovering and creating post-quantum cryptography standards and in 2020 they announced Round 3 finalists which is a list of 7 most promising general-purpose algorithms for public-key encryption/KEM and digital signature schemes. A list of 8 alternate algorithms has also been announced which may potentially be standardized by NIST as well, just not as part of Round 3. Current status is that NIST plans to publish standardization documents in 2024 but this may be subject to change depending on further development in quantum computing domain.

If you're interested in open-source projects that contribute to building quantum-resistant cryptography you can check out The Open Quantum Safe (OQS) Project - it's an open-source project that is also supported by companies like Microsoft, Amazon and IBM. Another cool thing that Microsoft did was that as part of the Project Natick experiment (underwater datacenter in the North Sea, off the Scottish coast) they built an encrypted network tunnel between the underwater datacenter and Microsoft Research Headquarters in Redmond, Washington, USA. This tunnel was protected with quantum-safe cryptography using a post-quantum cryptography-enabled Virtual Private Network (VPN) application based on OpenVPN. The experiment was quite successful which also contributes to a promissing near future of post-quantum cryptography.

## Recommended Resources

😼 [ETSI Whitepaper: Quantum Safe Cryptography and Security - An introduction, benefits, enablers and challenges](https://www.etsi.org/images/files/ETSIWhitePapers/QuantumSafeWhitepaper.pdf)

😼 [ETSI Technical Report: Migration strategies and recommendations to Quantum Safe schemes](https://www.etsi.org/deliver/etsi_tr/103600_103699/103619/01.01.01_60/tr_103619v010101p.pdf)

😼 [NIST Webinar: Virtual Workshop on Considerations in Migrating to Post-Quantum Cryptographic Algorithms](https://www.nccoe.nist.gov/get-involved/attend-events/virtual-workshop-considerations-migrating-post-quantum-cryptographic/post-workshop-materials)

😼 [NIST Cybersecurity Whitepaper: Getting Ready for Post-Quantum Cryptography: Exploring Challenges Associated with Adopting and Using Post-Quantum Cryptographic Algorithms](https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.04282021.pdf)

😼 [The Open Quantum Safe (OQS) project](https://openquantumsafe.org/)

😼 [Microsoft Article: Post-Quantum Crypto Tunnel to the Underwater Datacenter](https://www.microsoft.com/en-us/research/project/post-quantum-crypto-tunnel-to-the-underwater-datacenter/)

😼 [Microsoft Research: Quantum-safe cryptography: Securing today’s data against tomorrow’s computers](https://youtu.be/IiEdJ5IjH_U)

😼 [Microsoft - Post Quantum Cryptography](https://www.microsoft.com/en-us/research/project/post-quantum-cryptography/)
