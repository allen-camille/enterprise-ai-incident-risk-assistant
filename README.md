# Enterprise AI Assistant for Incident, Risk & Gap Analysis (Azure)

## Overview
This project demonstrates how an **enterprise-grade AI assistant** can be designed to support structured decision-making within **information security, risk management, and regulatory compliance**.

The solution is built using **Microsoft Azure AI Studio (Foundry)** and is intentionally designed as an **analytical decision-support system**, not a general-purpose chatbot. The assistant supports professionals working within **SOC, GRC, ISMS, and public sector environments**, with explicit alignment to **NIS2** and **ISO/IEC 27001**.

---

## Purpose
The purpose of this project is to demonstrate:
- Responsible and governed use of AI in information security
- Structured analytical methodologies for incident, risk, and gap assessments
- How AI can support — but not replace — human decision-making
- How regulatory and governance requirements can be embedded into AI behavior

This project is developed as part of professional skills development and is suitable for portfolios, interviews, and applied discussions within security and compliance teams.

---

## Design Principles
The AI assistant is governed by the following principles:

- **No speculation**  
  The assistant does not invent facts, causes, or impacts. Missing information is explicitly identified.

- **Structured and repeatable analysis**  
  All outputs follow defined analytical frameworks.

- **Governance-first approach**  
  Technical observations are always linked to governance, compliance, and organizational impact.

- **Neutral decision support**  
  The assistant provides analytical considerations, not operational commands or legal advice.

- **Auditability and traceability**  
  Outputs are defensible and suitable for review by ISAM, CISO, or auditors.

---

## Core Capabilities

### Incident Analysis
Structured incident analysis aligned with MSB guidance and ISO/IEC 27001:
- Incident classification and indicators
- Scope and affected assets
- Impact considerations
- Identified uncertainties and evidence gaps
- Lessons learned and improvement areas

### Risk Analysis
Risk assessments based on formal methodology:
- Asset
- Threat
- Vulnerability
- Likelihood
- Impact
- Qualitative risk level

Risk is assessed independently from incident response actions.

### Gap Analysis (NIS2 / ISO/IEC 27001)
Gap analysis structured as:
- Identified requirement
- Current state (observed facts only)
- Identified gap
- Risk associated with the gap
- Analytical recommendations

The analysis is suitable for ISMS development, regulatory preparedness, and internal audits.

---

## Architecture & Development Approach

The project follows a **three-track development model**:

### Track A – No-Code Prompt Governance
- Behavior control via system instructions
- Output structure and role boundaries enforced
- Focus on analytical rigor rather than creativity

### Track B – Azure AI Studio (Enterprise)
- AI agent built and versioned in Azure AI Studio (Foundry)
- Controlled publishing and testing in enterprise context
- Governance-driven configuration rather than free-form prompting

### Track C – Python / LangChain (Planned)
- Planned implementation of equivalent logic using Python
- Intended to demonstrate technical depth and understanding of underlying architectures

---

## Validation & Testing
The assistant has been tested using realistic scenarios involving:
- Suspected malware / botnet activity
- Financial and personal data handling in public sector context
- NIS2 and ISO/IEC 27001 regulatory requirements

Each scenario was evaluated through:
- Incident analysis
- Risk analysis
- Gap analysis
- Management-level executive summaries

Outputs demonstrate consistency, analytical maturity, and governance alignment.

---

## Responsible AI Considerations
This project explicitly avoids:
- Autonomous decision-making
- Operational security instructions
- Legal conclusions or advice
- Alarmist or speculative language

The assistant operates strictly as a **support function** for qualified personnel.

---

## Project Status
✅ Track A – Completed  
✅ Track B – Completed and validated  
🔜 Track C – Planned

---

## Author
Developed by **Allen Camille Muco**  
Focus areas: Information Security, GRC, Cloud Security, and Responsible AI

---

## Disclaimer
This project is a demonstrative and educational implementation. It is not intended to replace professional security operations, legal assessment, or organizational governance processes.
