# The Future Pillars of Cyber Security: Post-Quantum Cryptography and Zero Trust Architecture

[![Read PDF](https://img.shields.io/badge/PDF-Download%20Full%20Report-red?style=for-the-badge&logo=adobeacrobatreader)](./Post_Quantum_Zero_Trust_Analysis.pdf)

## I. Executive Summary
> **Abstract:** This report compares two new technologies in cyber security: Post-Quantum Cryptography (PQC) and Zero Trust Architecture (ZTA). PQC is a mathematical algorithm designed to protect global data privacy against the fast-approaching threat of quantum computers. ZTA, on the other hand, is a big-picture security structure that deals with current risks caused by traditional network boundaries disappearing due to cloud use and remote work.

The analysis finds that PQC and ZTA work together and need each other. While PQC solves the future encryption problem, ZTA provides the necessary setup, clear view, and continuous management required to successfully put PQC algorithms into place across complicated business networks. Organisations aiming for strong, long-term security must include PQC migration planning in their ZTA strategies, viewing both as essential, company-wide change programs rather than small technical projects.

---

## II. Introduction to Emerging Cyber Security Technologies

### A. Contextualising the Modern Threat Landscape
The traditional security models, like the “castle and moat” model that rely on trusting users and devices inside the company network, no longer work effectively because of modern operations. The wide use of cloud computing, many Internet of Things (IoT) devices and the rise of remote work have broken down old network boundaries. This change means security must move closer to the data and users, no matter where they are.

At the same time, a new serious threat is facing the core of digital security: **The potential arrival of powerful quantum computers.** These devices are expected to be able to run programs that could easily break the standard public-key encryption (like RSA and ECC) that protects almost all digital information today. This risk is made worse by the **"Harvest Now, Decrypt Later" (HNDL)** attack. Here, attackers collect huge amounts of currently encrypted data, storing it in the hope that a quantum computer will be able to decrypt it later.

### B. Selection Rationale: PQC and ZTA
To handle these two problems, this report focuses on:
* **Post-Quantum Cryptography (PQC):** Changing fast, shown by the finalisation of its main standards by the U.S. National Institute of Standards and Technology (NIST) in 2024.
* **Zero Trust Architecture (ZTA):** Explained in documents like NIST Special Publication 800-207, it offers a smart way to achieve immediate operational strength.

---

## III. Post-Quantum Cryptography (PQC): A Foundational Layer

### A. Overview of the Technology: What is PQC?
PQC, also called quantum-resistant cryptography, involves new mathematical algorithms designed to be safe from attacks by both regular computers and future quantum computers. It uses regular computer hardware to run new, hard maths problems (mostly using structured lattices).

In 2024, NIST released the final versions of the first three PQC standards:
* **ML-KEM (Kyber):** Meant to replace public-key systems like RSA/ECC for creating security keys. It has small keys and runs fast.
* **ML-DSA (Dilithium):** The main standardised algorithm for digital signatures.
* **SLH-DSA (Sphincs+):** A hash-based maths approach. It is an important backup method.

### B. Current State of Development and Adoption
The NIST standards mark a key moment, turning PQC from a theory into a required step for security. Governments and security leaders around the world are treating the HNDL threat seriously. Large internet companies, like Cloudflare, have already reached goals where most user-based traffic is protected by post-quantum encryption.

### C. Applications in Cyber Security
The main use of PQC is to protect data for the long term against HNDL attacks. PQC is vital for securing critical parts of the internet, including:
* Public Key Infrastructure (PKI)
* TLS/SSL protocols
* Virtual Private Networks (VPNs)
* Fully Homomorphic Encryption (FHE)

### D. Advantages and Limitations
**Advantages:** Evidently quantum resistant and offers long-term security. Speed tests show codes like Kyber are noticeably faster than older types in key exchange speed.

**Limitations:**
* **Complexity:** Often called one of the most complex change programs in decades.
* **Bandwidth:** Keys and signatures are much larger than ECC's, requiring more bandwidth.
* **Vendor Maturity:** The market is immature; HSMs and database tools do not yet fully support PQC.

### E. Security Implications and Challenges
The biggest challenge is not the maths, but the **lack of organisational management and clear visibility of encryption**. Without a centralised inventory of cryptographic assets, finding and replacing vulnerable algorithms is a "near-impossible task." Furthermore, there is a global shortage of engineers with experience in lattice-based cryptography.

---

## IV. Zero Trust Architecture (ZTA): A Strategic Framework

### A. Overview of the Technology: What is ZTA?
Zero Trust Architecture is a strategic security model built on the basic rule of **"never trust, always verify"**. It requires strict and continuous identity checks for every access request.

**The 3 Main Ideas (NIST):**
1.  **Continuously Verify:** Access is never given automatically.
2.  **Limit the Blast Radius:** Using micro-segmentation to stop lateral movement.
3.  **Assume Breach:** Operates on the assumption that the system is already compromised.

### B. Applications in Cyber Security
ZTA is the required security structure for today's decentralised business. It mitigates:
* **Ransomware:** Limits the spread of bad code.
* **Supply Chain Attacks:** Enforces strict device health checks.
* **Insider Threats:** Constant monitoring of user behaviour.
* **Compliance:** Fits with GDPR, HIPAA, and PCI-DSS.

### C. Advantages and Limitations
**Advantages:** Better security by making the system harder to attack and limiting damage. Can lead to less complexity over time.

**Limitations:** High initial setup costs. It requires a full, clear view of all data and resources to work correctly. Strict checks can cause operational friction.

### D. Security Implications and Challenges
A key risk is the **Policy Engine (PE)** becoming a Single Point of Failure (SPOF). If the centralized PE is compromised, it could grant access everywhere. Additionally, ZTA implementation often reveals existing poor asset management practices.

---

## V. Comparative Analysis: ZTA and PQC

### A. Fundamental Differences
* **PQC** is a basic encryption standard (the mathematical heart).
* **ZTA** is a strategic security plan (the rules and structure).

### B. Comparison Matrix

| Criteria | Post-Quantum Cryptography (PQC) | Zero Trust Architecture (ZTA) |
| :--- | :--- | :--- |
| **Primary Objective** | Long-term data privacy and integrity against quantum computers (HNDL threat). | Limiting the area an attack can affect and the damage inside current decentralised networks. |
| **Core Mechanism** | Mathematical complexity (lattice problems). | Continuous identity verification, micro-segmentation, and minimum access rights. |
| **Implementation Scope** | Deep technical layer (Cryptography, Protocols, HSMs). | Company-wide rules, identity management, and network segmentation. |
| **Timeline Urgency** | Strategic, long-term preparation (years of change required before Q-day). | Immediate need driven by current cloud and remote work threats. |
| **Required Agility** | **Cryptographic Agility** (ability to rapidly swap encryption codes). | **Policy Agility** (ability to rapidly adjust access controls based on context). |

### C. Synergies and Conflicts
**Synergies:**
1.  **ZTA Helps PQC Happen:** ZTA forces organisations to create the asset inventory needed for PQC migration.
2.  **PQC Makes ZTA Stronger:** PQC strengthens the encryption that ZTA relies on to protect data in transit and at rest.

**Conflicts:**
* **Speed:** ZTA's checks plus PQC's larger key sizes can create latency issues.

---

## VI. Conclusion and Recommendations

### A. Synthesis of Findings
Post-Quantum Cryptography and Zero Trust Architecture are essential improvements for the future of cybersecurity. PQC addresses the future quantum threat, while ZTA addresses immediate structural threats.

### B. Recommendations for Integration
1.  **Focus on Encryption Inventory:** Include the work of finding all encryption use directly in the ZTA planning stage.
2.  **Make Crypto Agility a ZTA Policy Rule:** The system must support hybrid encryption during the transition.
3.  **Manage Speed Trade-offs:** Closely test how PQC codes affect speed in resource-limited parts of the ZTA network.
4.  **Reduce Single Points of Failure:** Segment the network around the Policy Engine.
5.  **Keep Regulatory Alignment:** Follow NIST SP 800-207 and NIST FIPS 204/205.

---

### 📚 Works Cited
1. NIST. "New Draft White Paper | PQC Migration." 2025.
2. CrowdStrike. "What is Zero Trust?" 2025.
3. Akitra. "Zero Trust Architecture vs. Traditional Perimeter Security." 2025.
4. NIST. "What Is Post-Quantum Cryptography?" 2025.
5. GDIT. "Zero Trust and PQC Build a Stronger Security Foundation." 2025.
6. NIST. "NIST Releases First 3 Finalized Post-Quantum Encryption Standards." 2024.
7. Zscaler. "Adopting Zero Trust Principles with CISA's Maturity Model." 2025.
8. Forrester. "Zero Trust Security: The Business Benefits." 2025.
9. EC-Council. "Emerging Cybersecurity Trends & Technologies." 2025.
10. Google Cloud. "Post-quantum cryptography (PQC)." 2025.
11. Palo Alto Networks. "What Is Post-Quantum Cryptography (PQC)?" 2025.
12. Cryptomathic. "PQC Migration Challenges & Compliance Risks." 2025.
13. The Stack. "Eight firms blessed by the NCSC for PQC migration." 2025.
14. techUK. "NCSC shares update on PQC pilot scheme." 2025.
15. Cloudflare. "State of the post-quantum Internet in 2025." 2025.
16. ArXiv. "Performance Analysis and Industry Deployment of PQC Algorithms." 2025.
17. ArXiv. "Comparative Study of Classical and Post-Quantum Algorithms." 2025.
18. ISARA. "Lattice-Based Cryptography." 2025.
19. Fortinet. "What Is Zero Trust Architecture?" 2025.
20. Terranova Security. "The Limitations of Zero Trust Architecture." 2025.
21. Palo Alto Networks. "What Is Zero Trust Architecture?" 2025.
22. Verified Market Research. "Zero-Trust Security Market." 2025.
23. Zscaler. "What Is Zero Trust?" 2025.
24. ArXiv. "Zero Trust Architecture: A Systematic Literature Review." 2025.
25. PMC. "Theory and Application of Zero Trust Security." 2025.
26. F5. "Zero Trust Architecture for Government." 2025.
27. Microsoft Azure. "Architecture strategies for encryption." 2025.
28. TechTarget. "Security Models and Architecture." 2025.
29. SandboxAQ. "Bridging Post-Quantum Cryptography and Zero Trust." 2025.
30. IJIRT. "Beyond Passwords: Evaluating PQC in Zero Trust Architectures." 2025.

---
_Report uploaded by Harrison Ennis
