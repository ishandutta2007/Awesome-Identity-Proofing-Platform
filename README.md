# Awesome-Identity-Proofing-Platform

## Top Identity Proofing Platforms

A curated list of leading identity proofing and verification platforms for KYC/AML compliance, document authentication, biometric face matching, liveness detection, age assurance, and fraud prevention.  
**Primary focus: open-source software.**

Commercial / hosted platforms are listed separately for completeness. Open-source alternatives and community tools are emphasized throughout.

---

## SaaS / Hosted Platforms

| Platform | Description | Key Focus |
|----------|-------------|-----------|
| **[Persona](https://withpersona.com/)** | Flexible identity verification platform supporting government ID, selfie + liveness, phone, document, and reusable identity flows. Strong for customizable KYC, age verification, and fraud prevention across industries. | Modular identity proofing & reusable identities |
| **[Jumio](https://www.jumio.com/)** | AI-powered identity verification with document authenticity checks, selfie + liveness, biometrics, and continuous identity intelligence. High global ID coverage and deepfake resistance. | Automated ID + biometric verification |
| **[Veriff](https://www.veriff.com/)** | Fast AI-driven identity and document verification supporting 12,500+ documents across 230+ countries. Strong conversion rates and multi-language support. | Global document + identity verification |
| **[Trulioo](https://www.trulioo.com/)** | Global KYC platform with person match, document verification (14,000+ IDs), business verification (KYB), and AML screening across 195+ countries via a single API. | Global person + business identity data |
| **[Incode](https://www.incode.com/)** | Advanced AI identity verification with proprietary facial recognition, multi-modal liveness, document forensics, age estimation, and government-record matching (e.g., DMV). | High-accuracy biometrics & government-grade verification |
| **[Socure](https://www.socure.com/)** | Identity graph-powered verification and risk platform. Strong PII matching, document + biometric checks, and high-assurance proofing (including IAL2-aligned flows). | Data-driven identity graph & risk scoring |
| **[Onfido](https://www.entrust.com/)** (now Entrust Identity Verification) | Document + biometric identity verification with AI analysis, fraud signals, and global coverage. Widely used for digital onboarding and compliance. | Document + face verification |
| **[IDnow](https://www.idnow.io/)** | European-focused identity verification with video identification, document checks, and eID support. Strong regulatory compliance in the EU. | Video ID & regulated market verification |
| **[AU10TIX](https://www.au10tix.com/)** | High-assurance identity proofing with deep document forensics, anti-deepfake biometrics, cross-signal intelligence, and reusable digital ID capabilities (including Microsoft Entra integration). | Border/airline-grade forensics & reusable IDs |
| **[Sumsub](https://sumsub.com/)** | Full-stack KYC/KYB/AML platform with document verification, biometrics, liveness, and case management. Popular for fintech and crypto onboarding. | End-to-end KYC + compliance workflows |

---

## Open-Source Softwares

Fully production-grade, globally certified open-source identity proofing platforms (with the breadth of document coverage, forensic depth, and regulatory certifications of commercial vendors) remain limited. However, strong open-source building blocks exist for face recognition, liveness/anti-spoofing, document OCR/MRZ parsing, and self-hosted verification flows.

### Core Frameworks & Identity / Biometric Platforms

| Project | Description | License | Notes |
|---------|-------------|---------|-------|
| **[OpenBiometrics](https://openbiometrics.dev/)** / **[openbm/openbiometrics](https://github.com/drinkredwine/openbiometrics)** | Open-source biometric platform offering face detection/recognition, passive & active liveness, document processing (OCR + MRZ), and identity verification APIs. Self-hostable. | MIT | Strong modern biometric + document stack |
| **[ID-Verification-OpenKYC](https://github.com/FaceOnLive/ID-Verification-OpenKYC)** (FaceOnLive) | Community open-source eKYC project with face recognition, face liveness (anti-spoofing), and ID document recognition supporting large numbers of document types. | Open source | Practical open eKYC toolkit |
| **[KYC Beacon](https://github.com/bp-ventures/kyc-beacon)** | Early-stage open-source, self-hostable KYC / identity verification platform aiming to provide document verification, face match, liveness, hosted flows, and review dashboards. | Open source | Emerging self-hosted alternative |
| **[biometrical-verify](https://github.com/asalazarvaldiviaocg/biometrical-verify)** | Open-source biometric identity verification engine for face match, liveness, deepfake detection, and signed decision receipts. Designed for self-hosting with zero per-verification fees. | MIT | Privacy-focused biometric verification |
| **[OpenPassport](https://github.com/demonsh/openpassport)** (and related zk projects) | Privacy-preserving identity proofs from government-issued IDs (e.g., passport NFC) using zero-knowledge techniques. Proves attributes (age, nationality, etc.) without revealing full data. | Open source | ZK / privacy-preserving identity |
| **Google Longfellow-ZK / ZKP libraries** | Open-sourced zero-knowledge proof libraries for age assurance and privacy-enhancing digital ID applications. | Open source | Cryptographic age/attribute proofs |

### Specialized Libraries & Related Tools

| Project | Description | Focus Area |
|---------|-------------|---------|
| **Open-source face recognition & liveness models** | InsightFace, ArcFace, MiniFASNet, Silent-FAS, and various CVPR challenge models for face matching and anti-spoofing. | Face match + liveness |
| **Document OCR & MRZ parsers** | Tesseract, EasyOCR, PassportEye, and specialized MRZ (ICAO 9303) parsers for extracting data from passports and IDs. | Document data extraction |
| **Doubango KYC Documents Verif SDK** | Advanced document recognition & verification SDK with support for thousands of formats (commercial SDK with open components/research roots). | High-coverage document verification |
| **Self-hosted verification layers** | Projects such as verifid/vl providing deployable API layers for identity card/passport verification. | Self-hosted verification APIs |
| **OIDC / digital identity tools** | OpenID Connect libraries, verifiable credentials toolkits, and related identity infrastructure. | Digital identity standards |
| **Privacy-preserving proofs** | Additional zk-SNARK and attribute-based credential projects for selective disclosure. | Selective disclosure & privacy |

### Additional Notable Open-Source Tools

- **Computer vision stacks** — OpenCV, MediaPipe, and deep-learning frameworks (PyTorch/TensorFlow) commonly used to assemble custom liveness and matching pipelines.
- **Age estimation models** — Open models for estimating age from faces (useful for age-assurance flows).
- **Audit & case-management UIs** — Custom dashboards built on open frameworks for manual review of verification results.
- **Integration patterns** — Combining open OCR + face models + simple decision engines to approximate basic KYC flows.
- **Research prototypes** — Numerous academic and community projects exploring deepfake detection, document forensics, and passive liveness.

**Note:** Commercial platforms dominate in global document coverage (thousands of ID types), certified liveness (iBeta, etc.), advanced forensic analysis, regulatory compliance tooling, and high-volume reliability. Open-source solutions are strongest as building blocks (face matching, liveness models, OCR, privacy-preserving proofs) or early-stage self-hosted platforms. Production deployments often combine open components with commercial services or significant custom engineering and ongoing model maintenance.

---

## Quick Start Recommendations

| Goal | Recommended Starting Point |
|------|---------------------------|
| Self-hosted biometric + document verification | **OpenBiometrics** or **ID-Verification-OpenKYC** |
| Emerging full self-hosted KYC platform | **KYC Beacon** or **biometrical-verify** |
| Privacy-preserving / ZK identity proofs | **OpenPassport** or Google ZKP libraries |
| Face recognition + liveness building blocks | Open models (InsightFace, MiniFASNet, etc.) + OpenCV |
| Global commercial document + biometric KYC | **Jumio**, **Veriff**, **Persona**, or **Onfido/Entrust** |
| High-assurance / forensic-grade verification | **AU10TIX** or **Incode** |
| Global data + document coverage via API | **Trulioo** |
| Identity graph + risk scoring | **Socure** |
| Full KYC/KYB/AML suite | **Sumsub** |
| EU-regulated / video identification | **IDnow** |

---

## Contributing

Contributions, corrections, and new open-source projects are welcome.  
Please open an issue or pull request.

---

**Last updated:** August 2026  
Emphasizing open-source tools while documenting the major commercial platforms for context. Fully featured, globally certified open-source identity proofing platforms are still emerging; the strongest options today are biometric/document building blocks and early self-hosted KYC projects that require significant integration and validation work for production compliance use cases.
