# Enterprise AI Assistant for Incident, Risk & Gap Analysis (Azure)

## Overview
This project demonstrates how an **enterprise-grade AI assistant** can be designed to support structured decision-making within **information security, risk management, and regulatory compliance**.

The solution is built using **Microsoft Azure AI Studio (Foundry)** and is intentionally designed as an **analytical decision-support system**, not a general-purpose chatbot.

The assistant supports professionals working within **SOC, GRC, ISMS, risk management, and security governance** functions across **private organizations, regulated industries, and public sector environments**, with explicit alignment to recognized frameworks such as **NIS2** and **ISO/IEC 27001**.

---

## Purpose & Scope

This project implements an **enterprise AI assistant** designed to support:

- Structured incident analysis  
- Risk assessment  
- Compliance-oriented gap analysis  

The assistant is suitable for use in:

- **Private organizations**  
  (e.g. banks, financial institutions, insurance, fintech, large enterprises)
- **Consulting firms and MSSPs**
- **Public sector and critical infrastructure organizations**

It is built as an **analytical decision-support tool**, not as a detection, monitoring, or response engine.

---

## Focus Areas

The AI assistant is designed with the following focus:

### Governance and Internal Control
Supporting roles, responsibilities, decision-making structures, and compliance with internal and external requirements.

### Structured and Traceable Analysis
Providing consistent, auditable outputs for:
- SOC teams  
- GRC & risk management  
- Information security and compliance functions  

This applies across both **private and public organizations**.

### Analytical Decision Support
The assistant does **not** perform live detection, monitoring, or automated response.  
It supports human analysts by structuring findings, identifying gaps, and assessing risk.

---

## Intended Use

The assistant operates **on top of existing technical and organizational inputs**, such as:

- Incident descriptions
- Log excerpts and technical findings
- IR and SOC reports
- Policy texts and regulatory requirements
- Risk and compliance documentation

It helps transform this input into **structured analysis** suitable for professional security, risk, and governance roles.

---

## Governance & Limitations

To ensure responsible and enterprise-ready usage:

- ❌ No live detection or threat monitoring  
- ❌ No automated containment or remediation actions  
- ❌ No decision-making on behalf of the organization  

✅ The assistant is used strictly as:
- An **analytical support tool**
- A **quality and consistency aid** for human analysts
- A **complement to existing SOC, SIEM, IR, and GRC processes**

---

## Supported Analysis Types

The assistant is optimized for structured outputs such as:

### Incident Analysis
- Incident classification and indicators
- Root cause assessment
- Impact and risk evaluation
- Identification of uncertainties and information gaps
- Recommended short- and long-term actions

### Risk Analysis
- Asset, threat, and vulnerability-based assessment
- Likelihood and impact evaluation
- Qualitative risk level determination
- Separation of risk assessment from response actions

### Gap Analysis (Governance & Compliance)
- Comparison between requirements and current state
- Identification of control and process gaps
- Risk-based prioritization of improvements
- Alignment with frameworks such as NIS2 and ISO/IEC 27001

### Requirement Extraction
- Structured extraction of requirements from policy or regulatory text
- Clear, auditable requirement formulation
- Categorization into:
  - Governance
  - Process
  - Technical controls
  - Roles and responsibilities

---

## Technology Context

The solution is implemented and tested using **Azure AI Studio (Foundry)**, with a strong emphasis on:

- Enterprise governance
- Role-based access control
- Traceability and auditability
- Compatibility with both private-sector and public-sector security practices

---

## Analyst Tooling Context

This AI assistant is designed to support **human analysts** by structuring and contextualizing findings from common **incident response and security analysis tools**.

It does **not** perform live detection or response actions.  
Instead, it operates on observations, indicators, and outputs produced by technical investigation workflows.

Typical analyst tooling inputs may include results from:
- Endpoint investigation (CMD / PowerShell)
- Network traffic analysis (Wireshark)
- Case management and incident tracking (TheHive)
- Log and artifact review from forensic workflows

For reference examples of such analyst tooling and investigation artifacts, see:

📂 **Incident Response Toolkit Repository**  
https://github.com/allen-camille/INCIDENT-RESPONSE

This design explicitly positions the AI as a **decision-support and analysis layer**, bridging technical findings with structured incident analysis, risk assessment, and governance alignment.

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
  Outputs are defensible and suitable for review by ISAM, CISO, risk owners, or auditors.

---

## Core Capabilities

### Incident Analysis
Structured incident analysis aligned with **recognized best practices**  
(e.g. MSB guidance, ISO/IEC 27001):
- Incident classification
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

Risk analysis is performed independently from incident response actions.

### Gap Analysis (NIS2 / ISO/IEC 27001)
Gap analysis structured as:
- Identified requirement
- Current state (observed facts only)
- Identified gap
- Risk associated with the gap
- Analytical recommendations

The output is suitable for **ISMS development**, **regulatory preparedness**, and **internal audits**.

---

## Architecture & Development Approach

The project follows a **three-track development model**:

### Track A – No-Code Prompt Governance
- Behavior control via system instructions
- Output structure and role boundaries enforced
- Focus on analytical rigor rather than creativity

### Track B – Azure AI Studio (Enterprise)
- AI agent built and versioned in Azure AI Studio
- Controlled publishing and testing in an enterprise context
- Governance-driven configuration rather than free-form prompting

### Track C – Python / LangChain (Planned)
- Planned implementation of equivalent logic using Python and LangChain
- Intended to demonstrate technical depth and architectural understanding

---

## Validation & Testing

The assistant has been tested using **realistic enterprise scenarios**, including:
- Suspected malware and botnet activity
- Incidents involving financial and personal data
- Scenarios in regulated environments (private and public sector)
- Governance and compliance requirements under NIS2 and ISO/IEC 27001

Each scenario was evaluated through:
- Incident analysis
- Risk analysis
- Gap analysis
- Management-level analytical summaries

Outputs demonstrate **consistency**, **analytical maturity**, and **governance alignment**.

---

## Scenario-Based Validation

To validate the assistant’s behavior, governance alignment, and analytical quality,
it was tested using multiple **realistic enterprise security scenarios**.

The scenarios were intentionally selected to represent different incident types
commonly encountered in **banking, regulated industries, enterprise IT, and the public sector**.
All scenarios were analyzed strictly as **analytical decision support**, without
live detection or automated response.

### Scenario 1 – Suspected Account Takeover (ATO)
The assistant was validated against a suspected account takeover scenario,
focusing on:
- Identity and customer risk
- Unauthorized access indicators
- Qualitative risk assessment
- Governance-aware response recommendations

The output demonstrated careful separation between facts and assumptions,
appropriate risk classification, and responsible escalation guidance without
overstepping into operational or legal decision-making.

---

### Scenario 2 – Compromised Business-Critical Server
The assistant was tested using a compromised enterprise server scenario,
emphasizing:
- Infrastructure and availability impact
- Business-critical operations
- Potential malware or unauthorized access
- Risk to continuity and internal services

The analysis highlighted operational impact, containment principles,
and long-term governance improvements while maintaining a non-automated,
decision-support role.

---

### Scenario 3 – Regulatory & Reporting Assessment
A regulatory and reporting-focused scenario was used to assess the assistant’s
ability to:
- Evaluate potential notification obligations
- Reason about regulatory thresholds (e.g. GDPR, sector-specific rules)
- Clarify internal governance, roles, and responsibilities

The assistant correctly avoided legal conclusions, emphasized documentation,
and framed reporting decisions as evidence-based responsibilities of
appropriate internal stakeholders.

---

### Validation Outcome
Across all scenarios, the assistant consistently demonstrated:
- Structured and repeatable analysis
- Governance-first reasoning
- Responsible handling of uncertainty
- Clear separation between analysis and decision-making

This validation confirms the assistant’s suitability as an **enterprise-grade
analytical support tool** for incident response, risk assessment, and
compliance-oriented security workflows.

## Responsible AI Considerations

This project explicitly avoids:
- Autonomous decision-making
- Operational security instructions
- Legal conclusions or advice
- Alarmist or speculative language

The assistant operates strictly as a **support function for qualified professionals**.

---

## Project Status

✅ Track A – Completed  
✅ Track B – Completed and validated through test scenarios  
🔜 Track C – Planned  

---

## Author

Developed by **Allen Camille Muco**  
Focus areas: Information Security, GRC, Cloud Security, and Responsible AI

---

## Disclaimer

This project is a **demonstrative and educational implementation**.  
It is not intended to replace professional security operations, legal assessment, or organizational governance processes.
