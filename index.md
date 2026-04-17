# Derar Chekrouni
### Networks & Systems Engineer · Builder of Resilient Systems

> *"I don't just configure networks — I design systems that hold when everything else breaks."*

---

## About Me

I'm a Networks & Embedded Systems engineering student at the University of Algiers 1, with a hands-on background that stretches from low-level processor design all the way up to enterprise-grade cybersecurity assessments. I'm the kind of engineer who won't stop until the system works under real failure conditions — not just in theory.

My work lives at the intersection of **distributed systems**, **network infrastructure**, and **security**. I care deeply about systems that are resilient, secure, and built to last.

Outside the technical side, I've led teams, represented my class, and headed external relations for the ETIC Club — because good engineering also means communicating well and building things with people, not just for them.

---

## Core Skills

**Networks & Infrastructure**
- TCP/IP, Routing & Switching (OSPF, VLANs, STP, NAT, ACLs)
- Network Architecture, High Availability, Load Balancing, Failover Design

**Systems Administration**
- Linux, Distributed Systems, Stateless Application Design, Automated Leader Election

**Programming**
- Python, Dart/Flutter

**Languages**
- Arabic · French · English · Norwegian

---

## Featured Projects

---

### Distributed Online Voting Platform
**[GitHub](https://github.com/Mothrxa/Distributed-Voting)**

| | |
|---|---|
| **Tech Stack** | React, Nginx, Node.js, PostgreSQL, Patroni, etcd, HAProxy, Tailscale VPN |
| **Domain** | Systems & Network Administration · Distributed Systems |

A secure, production-grade voting platform built on a true three-tier distributed architecture — 12 virtual machines, zero single points of failure. Each tier runs behind its own HAProxy load balancer, with three nodes per tier operating independently so failures never cascade.

The database layer uses **PostgreSQL + Patroni + etcd** for automatic leader election and synchronous replication. The backend is a stateless **Node.js/Express** API cluster, horizontally scalable by design. The frontend is served by three **Nginx** nodes behind HTTPS. The entire infrastructure is connected over a **Tailscale VPN mesh**, with JWT authentication end-to-end.

Resilience was validated through live failure scenarios — nodes taken down mid-operation, with the system recovering automatically at every tier.
---

### EBIOS-RM Enterprise Security Assessment
**[GitHub](https://github.com/Mothrxa/EBIOS-RM)**

| | |
|---|---|
| **Tech Stack** | EBIOS-RM, ISO/IEC 27001, ANSSI, ANPDP/GDPR |
| **Domain** | Cybersecurity · Risk Management |

A comprehensive, real-world cybersecurity assessment for **@RCHIMED**, an architectural engineering firm — delivered as a 235-page report. All five EBIOS Risk Manager workshops were completed: from security baseline and threat actor mapping to strategic/operational attack scenarios and a full risk treatment plan. Deliverables include ISSP, BCP/DRP procedures with defined RTO/RPO, and over 30 feared events mapped across the attack surface.

---
### Dental Clinic Management System
*Bachelor Final Year Project*

| | |
|---|---|
| **Tech Stack** | Flutter Desktop/Android, PostgreSQL, UML modeling |
| **Domain** | Software Engineering |

A full Desktop app system for managing patients, appointments, and clinical staff. Requirements modeled with UML (use case, sequence, and class diagrams). Includes authentication and role-based access control. Delivered as a complete software engineering project from specification to implementation.

---

### Mothra — Secure Mailing Platform
**[GitHub](https://github.com/Mothrxa/Mothra) · [Live Demo](https://mothra-phi.vercel.app)**

| | |
|---|---|
| **Tech Stack** | Flutter Web, AES/CBC, RSA-2048, SHA-256, Supabase |
| **Domain** | Applied Cryptography · Full-Stack |

A fully deployed, end-to-end encrypted web mailing application built from scratch. Implements RSA-2048 for asymmetric key exchange, AES (CBC/ECB) for message confidentiality, RSA-based digital signatures for authentication, and SHA-256 integrity verification. Public keys and encrypted private keys are managed via a Supabase backend. Not a demo — a real deployment.

---

### OmniAI — AI-Powered Mobile Application
**[GitHub](https://github.com/Mothrxa/OmniAi)**

| | |
|---|---|
| **Tech Stack** | Flutter, Python/Flask, OpenAI, Whisper, Kokoro TTS, Tesseract OCR, Helsinki-NLP, Firebase |
| **Domain** | Mobile Development · AI Integration |

A Flutter mobile application bundling multiple AI tools in one place: chat assistant (GPT-4o-mini), speech-to-text (Whisper), text-to-speech (Kokoro), OCR (Tesseract), multilingual translation (Helsinki-NLP), text summarization (BART), and a full PDF toolkit. Backed by a Flask API handling all model inference, with Firebase authentication and a complete onboarding/profile flow.

---

### Custom Compiler
**[GitHub](https://github.com/Mothrxa/Compiler)**

| | |
|---|---|
| **Tech Stack** | C, MIPS R3000 assembly |
| **Domain** | Compiler Theory · Systems Programming |

Built a complete compiler following the classical compilation pipeline. Covers lexical analysis, syntactic parsing, semantic analysis with structured error reporting, intermediate representation generation, and final machine code targeting **MIPS R3000 assembly**. Every stage implemented from scratch.

---

### Mini MIPS Processor
**[GitHub](https://github.com/Mothrxa/Mips-R3000)**

| | |
|---|---|
| **Tech Stack** | Hardware description language, MIPS architecture |
| **Domain** | Computer Architecture |

Designed and implemented a single-cycle MIPS-like processor from the ground up — register file, ALU, instruction decoder, PC logic, and control unit. Debugged datapath/control interactions in detail, with partial support for branch and jump instructions. A deep dive into how machines actually execute instructions.

---

## Education & Certifications

| | |
|---|---|
| **Master 1 — Networks & Embedded Systems** | University of Algiers 1 · 2025 – Present |
| **Bachelor's Degree — Computer Science** | University of Algiers 1 · 2022 – 2025 |
| **Cisco Certified Network Associate (CCNA)** | 2026 |
| **ISC2 Certified in Cybersecurity (ISC2 CC)** | 2026 |

---

## Let's Connect

I'm open to collaborations, internships, and interesting problems.

[![Email](https://img.shields.io/badge/Email-chekrouni.derar@gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:chekrouni.derar@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Derar%20Chekrouni-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/derar-chekrouni-040092248/)
[![GitHub](https://img.shields.io/badge/GitHub-Mothrxa-181717?style=flat&logo=github)](https://github.com/Mothrxa)
