# Botium Toys — Security Audit & Compliance Assessment

**GRC Practice | Controls Assessment, Risk Identification & Regulatory Compliance Evaluation | Google Cybersecurity Professional Certificate**

[![Status](https://img.shields.io/badge/Status-Complete-success)](#)
[![Course](https://img.shields.io/badge/Google%20Cybersecurity-Module%202-blue)](#)
[![Framework](https://img.shields.io/badge/Framework-NIST%20CSF-orange)](#-audit-methodology--framework)
[![Compliance](https://img.shields.io/badge/Compliance-PCI%20DSS%20%7C%20GDPR%20%7C%20SOC-red)](#-compliance-checklist)
[![Controls](https://img.shields.io/badge/Controls%20Assessed-14-brightgreen)](#-controls-assessment-checklist)

---

## 🎯 Project Overview

This project is a complete internal security audit conducted for **Botium Toys**, a fictional small U.S. toy business with growing online presence and international customers. As part of the **Google Cybersecurity Professional Certificate (Module 2: Risk and Compliance)**, the audit evaluates the company's current security posture, assesses existing controls, and identifies gaps in regulatory compliance across **PCI DSS**, **GDPR**, and **SOC type 1 & 2** frameworks.

The audit follows the **NIST Cybersecurity Framework (CSF)** and produces a prioritized set of control and compliance recommendations to reduce organizational risk and protect sensitive customer data.

**Key Finding:** Only 5 of 14 controls are currently in place. All 4 PCI DSS best practices are unmet, representing critical exposure given that Botium Toys processes customer payment data online and in-store.

---

## 🏢 Organization Profile

| Field | Detail |
|-------|--------|
| **Organization** | Botium Toys |
| **Industry** | Retail — Toy Development & Sales |
| **Scope** | Entire security program: on-premises + e-commerce infrastructure |
| **Locations** | Single physical location (U.S.) + online storefront |
| **Customer Reach** | Domestic (U.S.) + International (incl. E.U.) |
| **Payment Processing** | In-store (POS) + Online (credit card) |
| **Concern** | Rapid business growth outpacing security controls |
| **Risk Score** | **8 / 10** (High) — insufficient controls relative to asset exposure |

---

## 📊 Audit Summary Metrics

| Metric | Value |
|--------|-------|
| **Total Controls Assessed** | 14 |
| **Controls In Place** | 5 (36%) |
| **Controls Missing** | 9 (64%) |
| **PCI DSS Best Practices Met** | 0 / 4 (0%) |
| **GDPR Best Practices Met** | 3 / 4 (75%) |
| **SOC 1 & 2 Best Practices Met** | 2 / 4 (50%) |
| **Overall Compliance Rate** | 42% |
| **Critical Risk Controls Missing** | 4 (Least Privilege, Encryption, IDS, Disaster Recovery) |

---

## 🔍 Audit Methodology & Framework

### NIST CSF Alignment

This audit uses the **NIST Cybersecurity Framework** as its structural backbone, evaluating controls across three categories:

| Control Category | Description | Examples Assessed |
|-----------------|-------------|------------------|
| **Administrative / Managerial** | Policies and procedures governing human behaviour and data management | Least Privilege, Separation of Duties, Password Policies, Disaster Recovery |
| **Technical** | Technology-based solutions protecting systems and data | Firewall, IDS, Encryption, Antivirus, Backups, Password Management |
| **Physical / Operational** | Controls limiting physical access to assets | Locks, CCTV, Fire Detection/Prevention |

### Control Types Evaluated

| Type | Purpose |
|------|---------|
| **Preventative** | Stop an incident before it occurs |
| **Corrective** | Restore assets or operations after an incident |
| **Detective** | Identify whether an incident is occurring or has occurred |
| **Deterrent** | Discourage threat actors from attempting an attack |

---

## ✅ Controls Assessment Checklist

> *Does Botium Toys currently have this control in place?*

### Administrative / Managerial Controls

| Status | Control | Type | Purpose |
|--------|---------|------|---------|
| ❌ **NO** | Least Privilege | Preventative | Reduce risk from malicious insiders or compromised accounts |
| ❌ **NO** | Disaster Recovery Plans | Corrective | Provide business continuity after an incident |
| ❌ **NO** | Password Policies | Preventative | Reduce likelihood of account compromise via brute force or dictionary attacks |
| ❌ **NO** | Separation of Duties | Preventative | Reduce risk and impact from malicious insiders or compromised accounts |

### Technical Controls

| Status | Control | Type | Purpose |
|--------|---------|------|---------|
| ✅ **YES** | Firewall | Preventative | Filter unwanted or malicious traffic from entering the network |
| ❌ **NO** | Intrusion Detection System (IDS) | Detective | Detect and flag anomalous traffic matching a known signature or rule |
| ❌ **NO** | Backups | Corrective | Restore and recover from a security event |
| ✅ **YES** | Antivirus Software | Corrective | Detect and quarantine known threats |
| ❌ **NO** | Manual Monitoring for Legacy Systems | Preventative | Identify and manage threats to out-of-date systems |
| ❌ **NO** | Encryption | Deterrent | Provide confidentiality to sensitive information at rest and in transit |
| ❌ **NO** | Password Management System | Preventative | Reduce password fatigue and enforce credential hygiene |

### Physical / Operational Controls

| Status | Control | Type | Purpose |
|--------|---------|------|---------|
| ✅ **YES** | Locks (offices, storefront, warehouse) | Deterrent/Preventative | Deter and prevent unauthorized physical access to assets |
| ✅ **YES** | CCTV Surveillance | Preventative/Detective | Reduce risk of physical incidents; support post-incident investigation |
| ✅ **YES** | Fire Detection/Prevention | Detective/Preventative | Detect fire conditions and prevent damage to physical assets and servers |

---

## 📋 Compliance Checklist

> *Does Botium Toys currently adhere to this compliance best practice?*

### 💳 Payment Card Industry Data Security Standard (PCI DSS)

> **Context:** Botium Toys accepts and processes credit card payments both in-store and online, making PCI DSS compliance mandatory.

| Status | Best Practice | Risk if Not Addressed |
|--------|--------------|----------------------|
| ❌ **NO** | Only authorized users have access to customers' credit card information | Unauthorized internal access to payment data; insider threat risk |
| ❌ **NO** | Credit card information is stored, accepted, processed, and transmitted in a secure environment | Data exposure during storage and transmission; breach risk |
| ❌ **NO** | Data encryption procedures implemented for credit card touchpoints and data | Unencrypted cardholder data vulnerable to interception |
| ❌ **NO** | Secure password management policies adopted | Weak credentials create entry point for attackers targeting payment systems |

**PCI DSS Compliance: 0 / 4 — Critical Failure ⛔**

---

### 🇪🇺 General Data Protection Regulation (GDPR)

> **Context:** Botium Toys conducts business with customers in the E.U., making GDPR compliance a legal obligation.

| Status | Best Practice | Risk if Not Addressed |
|--------|--------------|----------------------|
| ❌ **NO** | E.U. customers' data is kept private/secured | Non-compliance with GDPR Article 5; potential regulatory fines |
| ✅ **YES** | Plan in place to notify E.U. customers within 72 hours of a data breach | Meets GDPR Article 33 breach notification obligation |
| ✅ **YES** | Data is properly classified and inventoried | Supports data minimization and purpose limitation principles |
| ✅ **YES** | Privacy policies, procedures, and processes are enforced to document and maintain data | Meets accountability and transparency requirements |

**GDPR Compliance: 3 / 4 — Partial Compliance ⚠️**

---

### 🏛️ System and Organizations Controls (SOC Type 1 & SOC Type 2)

> **Context:** SOC reports assess internal controls over financial reporting and security. Relevant given Botium Toys' handling of PII and financial data.

| Status | Best Practice | Risk if Not Addressed |
|--------|--------------|----------------------|
| ✅ **YES** | User access policies are established | Access governance baseline is in place |
| ❌ **NO** | Sensitive data (PII/SPII) is confidential/private | Customer PII at risk of exposure without proper access controls and encryption |
| ✅ **YES** | Data integrity ensures data is consistent, complete, accurate, and validated | Data reliability requirements are met |
| ❌ **NO** | Data is available to individuals authorized to access it | Lack of role-based access control (RBAC) undermines data availability principles |

**SOC Compliance: 2 / 4 — Partial Compliance ⚠️**

---

## 🚨 Risk Findings & Prioritized Recommendations

### Critical — Implement Immediately

| # | Control / Gap | Compliance Impact | Justification |
|---|--------------|------------------|---------------|
| 1 | **Encryption** | PCI DSS, GDPR, SOC | Customer credit card data and PII transmitted and stored without encryption; highest data breach risk |
| 2 | **Least Privilege** | PCI DSS, SOC | All employees currently have access to internally stored data; violates need-to-know principle |
| 3 | **Separation of Duties** | PCI DSS, SOC | No division of critical functions; single-user access to sensitive operations creates fraud risk |
| 4 | **Intrusion Detection System (IDS)** | SOC | No mechanism to detect active threats or anomalous activity on the network |

### High — Implement in Near Term

| # | Control / Gap | Compliance Impact | Justification |
|---|--------------|------------------|---------------|
| 5 | **Disaster Recovery Plans** | SOC, Business Continuity | No documented plan for restoring operations after an incident; single point of failure risk |
| 6 | **Backups** | SOC, Business Continuity | No backup strategy in place; a ransomware attack or hardware failure could cause total data loss |
| 7 | **Password Policies** | PCI DSS | No minimum password complexity requirements enforce; brute force attacks are viable |
| 8 | **Password Management System** | PCI DSS | Password fatigue increases risk of reuse and weak credential selection across systems |

### Medium — Plan and Schedule

| # | Control / Gap | Compliance Impact | Justification |
|---|--------------|------------------|---------------|
| 9 | **Legacy System Monitoring** | SOC, General Risk | Unpatched legacy systems lack automated coverage; manual monitoring procedures needed |
| 10 | **EU Customer Data Privacy** | GDPR Article 5 | Customer data privacy/security controls not yet fully enforced for E.U. data subjects |
| 11 | **Asset Classification** | GDPR, PCI DSS | Without proper asset classification, additional required controls cannot be identified |

---

## 📐 Control Gap Visualization

```
Controls Assessment Summary
─────────────────────────────────────────────────────────
Administrative Controls    ████░░░░░░░░  0 / 4   (0%)
Technical Controls         ████░░░░░░░░  2 / 7  (29%)
Physical Controls          ████████████  3 / 3 (100%)
─────────────────────────────────────────────────────────
Overall Controls           █████░░░░░░░  5 / 14  (36%)

Compliance Frameworks
─────────────────────────────────────────────────────────
PCI DSS                    ░░░░░░░░░░░░  0 / 4   (0%)  ⛔ Critical
GDPR                       █████████░░░  3 / 4  (75%)  ⚠️  Partial
SOC Type 1 & 2             ██████░░░░░░  2 / 4  (50%)  ⚠️  Partial
─────────────────────────────────────────────────────────
Overall Compliance         █████░░░░░░░  5 / 12  (42%)
```

---

## 🗺️ Botium Toys — Current Security Posture

```
┌─────────────────────────────────────────────────────────────────┐
│               BOTIUM TOYS ASSET & RISK OVERVIEW                  │
├─────────────────────────────────────────────────────────────────┤
│  PHYSICAL LOCATION                  ONLINE STOREFRONT           │
│  ✅ Locks                           ❌ No Encryption             │
│  ✅ CCTV                            ❌ No IDS                    │
│  ✅ Fire Detection                  ❌ No Password Policies      │
│  ✅ Firewall (network)              ❌ No Least Privilege        │
│  ✅ Antivirus                       ❌ No Backups                │
│                                     ❌ No Disaster Recovery      │
├─────────────────────────────────────────────────────────────────┤
│  DATA ASSETS AT RISK                REGULATORY EXPOSURE         │
│  • Customer PII                     • PCI DSS — 0% compliant    │
│  • Credit card information          • GDPR — 75% compliant      │
│  • Cardholder data (in-store)       • SOC 1 & 2 — 50% compliant │
│  • E.U. customer data               • Risk Score: 8 / 10        │
│  • Legacy system data               • All employees have        │
│                                       full data access          │
└─────────────────────────────────────────────────────────────────┘
```

---

## 📝 Audit Recommendations Summary

Based on the controls assessment and compliance checklist findings, the following recommendations were submitted to IT management:

**Controls to Implement Immediately:**

Multiple controls need to be implemented to improve Botium Toys' security posture and better ensure the confidentiality of sensitive information, including **Least Privilege**, **Disaster Recovery Plans**, **Password Policies**, **Separation of Duties**, an **IDS**, **ongoing legacy system management**, **Encryption**, and a **Password Management System**.

**Compliance Gap Remediation:**

To address gaps in compliance, Botium Toys needs to implement controls such as **Least Privilege**, **Separation of Duties**, and **Encryption**. The company also needs to **properly classify assets** to identify additional controls that may need to be implemented to improve their security posture and better protect sensitive information.

**Priority Order for Stakeholder Communication:**

1. Encrypt all cardholder data and PII immediately — eliminates highest-impact data breach risk
2. Implement Least Privilege and Separation of Duties — closes insider threat and access control gaps
3. Deploy an IDS — provides visibility into active threats targeting the network
4. Establish Disaster Recovery and Backup procedures — ensures business continuity
5. Enforce Password Policies and deploy a Password Management System — reduces credential attack surface
6. Classify all assets — enables identification of further controls and compliance obligations

---

## 🛠️ Skills & Frameworks Demonstrated

<table>
<tr>
<td width="25%">

**GRC Practice**
- Internal security auditing
- Controls gap analysis
- Risk scoring & prioritization
- Stakeholder reporting

</td>
<td width="25%">

**Compliance Frameworks**
- PCI DSS (payment security)
- GDPR (data privacy — E.U.)
- SOC Type 1 & 2 (organizational controls)
- NIST CSF (risk management)

</td>
<td width="25%">

**Control Domains**
- Administrative/Managerial
- Technical controls
- Physical/Operational
- Preventative, Detective, Corrective, Deterrent types

</td>
<td width="25%">

**Risk Assessment**
- Asset inventory evaluation
- Threat & vulnerability mapping
- Compliance obligation identification
- Remediation planning

</td>
</tr>
</table>

---

## 📚 Audit Documents

| Document | Description |
|----------|-------------|
| **[Controls & Compliance Checklist](docs/Controls_and_compliance_checklist.docx)** | Completed Yes/No assessment for all 14 controls and 12 compliance best practices |
| **[Control Categories Reference](docs/Control_categories.docx)** | Full reference of administrative, technical, and physical control types and purposes |

---

## 🎓 Project Context

**Course:** Google Cybersecurity Professional Certificate  
**Module:** Course 2 — Play It Safe: Manage Security Risks  
**Topic:** Conducting a Security Audit  
**Completed:** 2025

**Learning Objectives Covered:**
- ✅ Conduct an internal security audit using a structured checklist
- ✅ Identify missing controls across administrative, technical, and physical domains
- ✅ Evaluate compliance against PCI DSS, GDPR, and SOC type 1 & 2 standards
- ✅ Assess organizational risk based on asset exposure and control gaps
- ✅ Formulate prioritized recommendations for IT management and stakeholders
- ✅ Communicate findings clearly to both technical and non-technical audiences

---

## 📧 Contact

**Kanhay Thakore**  
GRC | Risk Assessment | Security Auditing | Compliance

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/kanhaythakore/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black)](https://github.com/Kanhay-Thakore)
[![Email](https://img.shields.io/badge/Email-Contact-red)](mailto:thakorekanhay70@gmail.com)

---

## 📄 License

This project is part of my academic and professional portfolio demonstrating GRC and security audit capabilities. All findings, checklists, and recommendations are based on a simulated audit scenario from the Google Cybersecurity Professional Certificate program.

---

⭐ **If you find this project valuable, please give it a star!**

*Last Updated: 2025*
