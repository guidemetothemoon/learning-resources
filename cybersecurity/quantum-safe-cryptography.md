# Quantum-Safe Cryptography

With acceleration of development of quantum computers it has become clear that current cryptographic techniques and cryptographic algorithms will face great challenges once quantum computers become publicly available. Current data protection mechanisms heavily rely on a collection of well-proven and well-known cryptographic algorithms. These cryptographic algorithms were built so that they can't be broken with computing power that is currently available. With advancement and public availability of quantum computers such implementations will become pretty easy and straightforward to solve which makes establishment and standardization of quantum-safe cryptography critically important.

What makes the whole situation even scarier is the fact that a malicious actor can steal data that's safely encrypted now and keep it stored until a quantum computer with enough computing power becomes available. Once it's available, all encrypted data can potentially be easily decrypted. This means that **all data that has ever been in-transit or at-rest will become vulnerable to disclosure**.

Not all cryptographic algorithms are currently confirmed to be vulnerable to quantum attacks but this may change with time and more research. Symmetric encryption algorithms like AES can still be quantum-safe by increasing the key size. Most of the asymmetric encryption algorithms are not quantum-safe due to the fact that they're based upon Integer Factoring and Discrete Logarithms complexities which can be resolved with quantum computing. For example, security protocols like **TLS, SSH, S/MIME and IKE** will be affected by quantum vulnerabilities and will need to be upgraded to be quantum-safe.

It has also become clear that many security protocols are lacking **cryptographic agility** which means that it makes it extremely hard to extend and improve them in order to make them quantum-safe.

These are some of the factors that make quantum-safe cryptography a complex task to complete. All the existing security protocols and encryption algorithms have been tested, researched and standardized for years. Historically, **it has taken almost two decades to deploy our modern public key cryptography infrastructure** so you can imagine that creating a new standard for quantum-safe cryptography under current time constraints and the level of urgency is far from an easy task. 

Back in 2016 NIST has started a process for discovering and creating post-quantum cryptography standards and in 2020 they announced Round 3 finalists which is a list of 7 most promising general-purpose algorithms for public-key encryption/KEM and digital signature schemes. A list of 8 alternate algorithms has also been announced which may potentially be standardized by NIST as well, just not as part of Round 3. Current status is that NIST plans to publish standardization documents in **2024** but this may be subject to change depending on further development in quantum computing domain.

If you're interested in open-source projects that contribute to building quantum-resistant cryptography you can check out **The Open Quantum Safe (OQS) Project** - it's an open-source project that is also supported by companies like Microsoft, Amazon and IBM. Another cool thing that Microsoft did was that as part of the **Project Natick** experiment (underwater datacenter in the North Sea, off the Scottish coast) they built an encrypted network tunnel between the underwater datacenter and Microsoft Research Headquarters in Redmond, Washington, USA. This tunnel was protected with quantum-safe cryptography using a post-quantum cryptography-enabled Virtual Private Network (VPN) application based on OpenVPN. The experiment was quite successful which also contributes to a promissing near future of post-quantum cryptography.

**Lastly, what are the current recommendations for preparing and migrating to quantum-safe standards?**

ETSI (European Telecommunications Standards Institute) has created a framework that suggests a staged approach to migration:

1. **Inventory compilation** - in order to understand the impact and get an overall picture of how much you will need to migrate, you need to identify the set of cryptographic assets and processes in the system, including hardware and software. This stage also includes identification of impacted supply chain resources.
2. **Preparation of the migration plan** - once the affected assets have been identified you can start with creating a plan for migration, including the cost and timeline. Detailed planning is dependent upon knowledge of the inventory of cryptographic assets and their dependencies across the system supply chain, therefore Stage 1 is a pre-requisite for the migration plan preparation stage. Dependency testing must be an important part of the migration plan preparation.
3. **Migration execution** - this stage includes migration management with tasks like tracking the progress and the migration budget; another part of the migration execution stage is mitigation management where the plan must be in place for how to handle issues that may occur during migration and how these issues may affect the overall budget and timing constraints.


Stage 1 is an activity that anyone can start working on already now. Getting an overall picture of the assets that an organization has, including supply chain, will not only be valuable for planning for migration to quantum-safe state but it will also be useful for threat modeling and strengthening security of the organization and the ecosystem it owns and maintains.

More details on everything summarized here can be found in the recommended resources section below - reach out if you want to have a chat about quantum-safe cryptography!😸

## Recommended Resources

😼 [ETSI Whitepaper: Quantum Safe Cryptography and Security - An introduction, benefits, enablers and challenges](https://www.etsi.org/images/files/ETSIWhitePapers/QuantumSafeWhitepaper.pdf)

😼 [ETSI Technical Report: Migration strategies and recommendations to Quantum Safe schemes](https://www.etsi.org/deliver/etsi_tr/103600_103699/103619/01.01.01_60/tr_103619v010101p.pdf)

😼 [NIST Webinar: Virtual Workshop on Considerations in Migrating to Post-Quantum Cryptographic Algorithms](https://www.nccoe.nist.gov/get-involved/attend-events/virtual-workshop-considerations-migrating-post-quantum-cryptographic/post-workshop-materials)

😼 [NIST Cybersecurity Whitepaper: Getting Ready for Post-Quantum Cryptography: Exploring Challenges Associated with Adopting and Using Post-Quantum Cryptographic Algorithms](https://nvlpubs.nist.gov/nistpubs/CSWP/NIST.CSWP.04282021.pdf)

😼 [The Open Quantum Safe (OQS) project](https://openquantumsafe.org/)

😼 [Microsoft Article: Post-Quantum Crypto Tunnel to the Underwater Datacenter](https://www.microsoft.com/en-us/research/project/post-quantum-crypto-tunnel-to-the-underwater-datacenter/)

😼 [Microsoft Research: Quantum-safe cryptography: Securing today’s data against tomorrow’s computers](https://youtu.be/IiEdJ5IjH_U)

😼 [Microsoft - Post Quantum Cryptography](https://www.microsoft.com/en-us/research/project/post-quantum-cryptography/)
