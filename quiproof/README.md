# Quiproof: ZK National Identity & Verifiable Credentials Platform

A sovereign, privacy-preserving digital identity bridge for national ID systems.

---

## 👥 Team
- **Team/Individual Name:** Alex Padilla  
- **GitHub Handles:** [@padimaster](https://github.com/padimaster)  
- **Devfolio Handles:** [@padimasterec](https://devfolio.co/@padimasterec)

---

## 📖 Project Description

### The Problem  
Most national identity systems depend on centralized, high-friction verification processes.
To prove a single fact — such as being over 18 — users must disclose their full personal information (name, birthdate, ID number, etc.), creating what’s known as the “over-sharing paradox.”

This approach not only undermines user privacy but also exposes citizens to identity theft, data leaks, and regulatory non-compliance (e.g., GDPR, eIDAS 2.0).

Meanwhile, governments have already deployed ICAO 9303-compliant ID cards and e-passports, embedding cryptographically secure chips (NFC). However, there is still no trust bridge between these verified physical identities and decentralized digital ecosystems.

### The Solution — **Quiproof**  
**Quiproof** enables citizens to convert their government-issued IDs into Zero-Knowledge Verifiable Credentials (ZK-VCs) that they fully control from their personal wallet — no intermediaries, no data exposure.

#### Core Capabilities:
- **Trust Ingestion (MRZ → VC):** Scan a national ID via camera and NFC to unlock the chip (BAC), verify authenticity (Passive Authentication), and issue a W3C Verifiable Credential.
- **Selective Disclosure (ZKPs):** Generate Zero-Knowledge Proofs to privately verify facts such as “I am over 18” or “I am a citizen of X,” without revealing underlying personal data.
- **Scalable Verification (Layer 2):** Anchor DID states and revocation registries on a ZK-Rollup (zkSync Era) for cost-efficient, tamper-proof, and globally verifiable identity proofs.

#### Why It Matters  
Quiproof establishes a privacy-first national identity layer in **Ecuador** that preserves sovereignty while ensuring interoperability with Web3 and e-governance frameworks.

It allows:
- Governments to digitally extend their existing ID infrastructure without replacing it.
- Citizens to prove identity attributes securely and privately.
- Developers and institutions to verify trust cryptographically, not bureaucratically.

---

## Tech Stack

- **Core Cryptography:** ZK-SNARKs (Groth16)
- **Smart Contracts:** Arbitrum Stylus (Arbitrum Mainnet)
- **Identity Standards:** ICAO 9303 eMRTD + W3C Verifiable Credentials
- **Mobile Wallet:** React Native + Kotlin (NFC Integration)
- **ZK Circuits:** SP1 (Succinct Parallel Prover)
- **Backend & APIs:** Rust + PostgreSQL / IPFS metadata registry

---

## Objectives

By the end of ARG25, **Quiproof** will:

**1. Establish a national identity research baseline**
| - Analyze the Ecuadorian ID Card cryptographic design, ICAO 9303 compliance, and data standards.
| - Define the legal, technical, and interoperability framework for self-sovereign identity adoption in Ecuador.

**2. Design a complete decentralized identity architecture**
| - Develop the end-to-end Quiproof architecture, integrating MRZ → NFC → VC issuance.
| - Define the data model, credential lifecycle, and revocation mechanism aligned with W3C VC and DID standards.

**3. Deliver an operational MVP and live demo**
| - Implement a working Trust Ingestion prototype capable of scanning, authenticating, and issuing Verifiable Credentials.
| - Integrate ZK proof modules for age and nationality verification.
| - Deploy a verifier contract and present the full system demo at the end of ARG25.

---

## Weekly Progress

### Week 1 (ends Oct 31)
**Goals**
- Analyze the Ecuadorian ID Card system: data structure, embedded chip type, and regulatory context.
- Study ICAO 9303 standards for passports and ID cards.
- Review international SSI and ZKP implementations (QuarkID, ZK Passport) to inform design choices.
- Define initial cryptographic model for MRZ → NFC → VC issuance.

**Progress Summary**
- Completed literature and standard review on Ecuadorian ID architecture.
- Identified compatible ICAO 9303 fields and chip protocols (BAC, PA).
- Outlined trust-ingestion cryptographic sequence.

---

### Week 2 (ends Nov 7)
**Goals**
- Design the end-to-end system architecture, including wallet, smart-contract layer, and verifier modules.
- Define VC data model aligned with W3C standards and Ecuadorian ID schema.
- Map user flows and UX journeys for onboarding and proof generation.

**Progress Summary**
- Produced system architecture diagram and component interfaces.
- Drafted UI wireframes and user journeys. 

---

### Week 3 (ends Nov 14)
**Goals**
- Develop the MVP with MRZ scan, NFC read, and VC issuance flow.
- Integrate ZK proof circuits for age and nationality verification.
- Deploy verifier contract on zkSync testnet and prepare final demo presentation.

**Progress Summary**
_(to be updated)_

---

## 🧩 Final Wrap-Up

- **Main Repository:** [Frontend](https://github.com/Quiproof/app)
- **Validation Repository:** [Backend + Circuits + Contracts](https://github.com/padimaster/quiproof-validation)
- **Slides / Presentation:** ARG25 final deck (in progress)

---

## 🧾 Learnings

- Implemented the **MRZ → NFC → VC pipeline** for trust ingestion.  
- Explored **ZK-Rollups as identity layers** for scalability.  
- Identified UX barriers and key-recovery trade-offs in SSI systems.  
- Understood how to bridge government trust anchors with decentralized verification.

---

## 🚀 Next Steps

- Expand to multi-country ICAO document support.  
- Integrate social / cloud key-recovery safeguards for usability.  
- Collaborate with public institutions to pilot ZK identity issuance in LatAm.  
- Launch **Quiproof DAO** for open governance and standardization efforts. (First pilot in Ecuador)
