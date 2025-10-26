# EU Compliance Maturity Chain: From Directives to Customer Trust

> This document provides a **comprehensive, detailed explanation** of the EU Compliance Maturity Chain, outlining the interconnectedness of key regulations and frameworks from NIS2 to ISO 27001, culminating in customer trust. It's designed as robust technical documentation or training material.

---

## About this Document

*   **Audience:** Cybersecurity professionals, compliance officers, technical architects, and management interested in EU digital regulations and their practical implementation, particularly within critical infrastructure and utility sectors.
*   **Scope:** In-depth explanations of the compliance journey, practical application insights, and mapping to security controls and technical solutions on Azure/Databricks.
*   **Purpose:** To illustrate how various EU directives (NIS2, AI Act, CRA) build upon each other and are integrated through a management system like `ISO 27001` to foster resilience and trust.

---

## The Compliance Maturity Chain: From NIS2 to Customer Trust

Achieving robust cybersecurity and digital resilience in the EU is a journey that moves through interconnected levels of compliance maturity. This chain demonstrates how foundational security, responsible AI, and product resilience converge into an integrated management system that ultimately builds market confidence and customer trust.

### 1. NIS2 Directive – Security Foundations

*   **What it is / Why it matters:** The `NIS2 Directive` (Network and Information Security 2) is a cornerstone of EU cybersecurity. It mandates a baseline of **organizational and technical measures** for a broad range of `essential and important entities` to enhance their overall cyber resilience. It provides the initial regulatory push to secure critical digital infrastructure and services.
*   **Focus areas:** `Asset management`, `incident response`, `supplier risk management`, and `business continuity` are central to establishing a secure operational baseline.
*   **Outcome:** A secure operational baseline for digital infrastructure and critical services, crucial for protecting the EU's economy and society from cyber threats.

> **Dependency:** The `EU AI Act` and `Cyber Resilience Act (CRA)` fundamentally assume `NIS2` maturity for core security capabilities. Without a strong NIS2 foundation, subsequent compliance efforts will lack critical underlying security measures.

### 2. EU AI Act – Accountable and Explainable AI

*   **What it is / Why it matters:** The `EU AI Act` is the world's first comprehensive legal framework for artificial intelligence, establishing a risk-based approach to govern AI systems. It aims to ensure that AI deployed within the EU is **accountable, transparent, and trustworthy**, particularly in `high-risk use cases` such as critical infrastructure monitoring or leak detection.
*   **Requirements:** Introduces mandates for `human-in-the-loop (HITL)` oversight, `bias controls`, and extensive `AI lifecycle documentation`.
*   **Foundation:** It builds directly on the `NIS2` security baseline, specifically leveraging its requirements for `data integrity` and `traceability` as prerequisites for reliable and secure AI operations.

> **Dependency:** Without a secure `NIS2` foundation, critical AI data and systems cannot be adequately protected, making `AI Act` compliance unsustainable. Data integrity and system availability, core to `NIS2`, are essential for trustworthy AI.

### 3. Cyber Resilience Act (CRA) – Product and Software Security

*   **What it is / Why it matters:** The `Cyber Resilience Act (CRA)` targets the security of connected hardware and software products. Its goal is to ensure that products with digital elements are `secure-by-design` from their inception, have robust `vulnerability handling` processes, and undergo `post-market monitoring` throughout their entire lifecycle. This directly impacts developers and manufacturers of products, including those that integrate AI.
*   **Scope:** Ensures connected products (including `AI-based utilities platforms`) maintain cyber resilience throughout their lifecycle, from development to end-of-life.
*   **Extension:** It extends the organizational controls of `NIS2` and the technical controls related to data and system integrity from the `AI Act` directly into `product engineering` and supply chain management.

> **Dependency:** `NIS2` provides the overarching `governance layer` for an organization's security posture, while the `CRA` focuses on the `technical implementation layer` for securing specific products and software. They are complementary in ensuring end-to-end security.

### 4. ISO/IEC 27001 – Integrated Management System

*   **What it is / Why it matters:** `ISO/IEC 27001` is an internationally recognized standard for information security management systems (`ISMS`). It provides a holistic, structured framework for managing an organization's information security. When integrated with EU directives, it acts as the **formal management system** that unifies and operationalizes `NIS2`, `AI Act`, and `CRA` controls.
*   **Integration:** It maps organizational processes, risk management, and continuous improvement cycles to create `audit-ready frameworks` for all relevant regulations.
*   **Role:** Acts as a `“control hub”`, ensuring consistency, traceability, and verifiable evidence across all EU requirements, transforming disparate compliance efforts into a coherent, managed system.

> **Dependency:** `ISO 27001` is crucial for transforming episodic regulatory compliance into **sustainable, auditable, and continuously improving operations**. It provides the methodology to manage security risks systematically.

### 5. Customer Trust & EU Market Readiness

*   **What it is / Why it matters:** The ultimate outcome of integrating these compliance efforts through a robust `ISMS` is enhanced `customer trust` and `market readiness`. Compliance is not just a legal obligation but a strategic advantage.
*   **Benefits:**
    *   Customers gain confidence from visible **transparency and accountability**.
    *   Regulatory audits become simpler and faster due to centralized evidence and mature processes.
    *   Overall market confidence increases, leading to more robust partnerships and competitive advantage.

---

## Critical Insight: Unified Governance Builds Trust

> Achieving compliance with `NIS2`, `EU AI Act`, and `CRA` is not a checkbox exercise — it is a chain of **interdependent maturity levels**. Each regulation reinforces the others, contributing to a holistic security and compliance posture.
>
> When implemented through a unified framework (such as **Thinkwerke’s CIR³ Framework**):
>
> *   Each directive strengthens the others, creating synergistic benefits.
> *   Governance becomes `proactive` rather than merely `reactive`, anticipating risks.
> *   The organization gains measurable **resilience, audit readiness, and lasting customer trust**.

---

# ENISA Compliance Mind Map — Utilities / Critical Infrastructure

*Based on `ENISA Baseline Security Measures (2023)` & `Cybersecurity Maturity Model (2024)`*
*Customized for Utility, Water, and Energy Operators – Aligned with `NIS2`, `AI Act`, `CRA`, and `ISO 27001`*

This mind map illustrates how `ENISA's` guidance translates into practical implementation for critical infrastructure operators, cross-referencing specific controls with EU regulations and cloud-native solutions on Azure/Databricks.

| **Domain**                         | **ENISA Control Category**        | **Focus Area / Objective**                                       | **Utility-Specific Implementation (Azure / Databricks)**                         | **Linked Regulation / Article**      |
| :--------------------------------- | :-------------------------------- | :--------------------------------------------------------------- | :------------------------------------------------------------------------------- | :----------------------------------- |
| **1. Governance & Accountability** | Policy & Risk Management          | Define risk ownership, establish policies, and assign board-level accountability. | Adopt unified `NIS2` governance; risk owners mapped in `Azure AD` and `ServiceNow CMDB`. | `NIS2 Art. 21(1)`, `ISO 27001 A.5`  |
| **2. Asset & Configuration Mgmt**  | Asset Identification              | Maintain updated `CMDB` of `OT/IT` systems, datasets, and `AI models`. | Use `Azure Resource Graph`, `Defender for Cloud`, and `Unity Catalog` for full inventory. | `NIS2 Art. 21(2)(a)`, `CRA Annex I`  |
| **3. Access & Identity Security**  | Authentication & Authorization    | Enforce `least privilege`, `MFA`, and `just-in-time access`.     | Implement `Azure AD PIM`, `SCIM sync` with Databricks, and `RBAC` in `Unity Catalog`. | `NIS2 Art. 21(2)(c)`, `ISO 27001 A.5.17` |
| **4. Threat & Vulnerability Mgmt** | Security Operations & Patch Mgmt  | Detect, assess, and mitigate vulnerabilities across environments. | Enable `Defender for Cloud`, integrate patch validation via `CI/CD` and Databricks cluster policies. | `CRA Art. 10`, `NIS2 Art. 21(2)(d)`  |
| **5. Data Protection & AI Integrity** | Data Security & AI Governance     | Protect data integrity, ensure lawful processing, and control `AI model risk`. | Use `Microsoft Purview`, `Unity Catalog masking`, and `MLflow lineage` to enforce `AI transparency`. | `AI Act Art. 9–15`, `GDPR`, `NIS2 Art. 21` |
| **6. Incident Management & Reporting** | Detection & Notification          | Implement structured detection, triage, and reporting workflows. | Route Databricks audit logs to `Sentinel`; `Logic Apps` for `24h/72h NIS2 reporting templates`. | `NIS2 Art. 23`, `ENISA IR Guidelines` |
| **7. Supply Chain Security**       | Third-Party Risk                  | Assess and monitor dependencies, vendors, and firmware integrity. | Evaluate supplier risk through `Azure Policy`, `ACR image scanning`, and `SBOM` in `CI/CD`. | `NIS2 Art. 21(2)(f)`, `CRA Annex II` |
| **8. Backup & Recovery**           | Business Continuity               | Ensure resilience via recovery testing and redundant design.      | Use `ADLS versioning`, `Delta Lake time travel`, and quarterly restoration validation. | `NIS2 Art. 21(2)(e)`, `ISO 27001 A.5.29` |
| **9. Secure Development & Product Resilience** | Secure SDLC                       | Apply `security-by-design` principles to connected devices and software. | Integrate `DevSecOps` gates, static code analysis, and `CRA conformity` in release pipeline. | `CRA Annex I & II`, `ENISA SDLC Framework` |
| **10. Monitoring & Continuous Improvement** | Audit, Metrics & Maturity         | Continuously assess and improve security maturity using `ENISA’s model`. | Deploy **Thinkwerke CIR³ Framework** with `Grafana` & `Sentinel dashboards` for compliance metrics. | `ENISA Maturity Model 2024`, `ISO 27001 A.9` |
| **11. Awareness & Training**       | Human Factors                     | Build staff competence in cybersecurity, compliance, and `AI ethics`. | Conduct quarterly workshops on `NIS2` and `AI risk`; integrate `Azure Learning Path analytics`. | `NIS2 Recital 68`, `ISO 27001 A.6` |
| **12. Reporting & Board Oversight** | Governance Reporting              | Provide evidence-driven reports to executive and supervisory authorities. | Generate unified compliance dashboard (**CIR³**) for board oversight and `ENISA-style quarterly reports`. | `NIS2 Art. 25`, `ENISA Oversight Model` |

---

### Summary Insight

> `ENISA’s` model expects **continuous, evidence-based cybersecurity governance** across the entire lifecycle — from **board accountability to AI-driven automation**.
> For utilities, integrating `NIS2`, `AI Act`, and `CRA` controls within a unified framework (like **Thinkwerke CIR³**) delivers measurable resilience, comprehensive compliance, and lasting customer trust.

---

**Prepared by:** Thinkwerke – Strategy Meets Security
**Date:** October 2025

---

### Regulatory Compliance Matrix: ENISA Expectations and Utility Actions

This matrix details the key requirements of each regulation, what `ENISA` expects from entities, the specific actions utilities should take, and the corresponding deliverables or evidence needed for auditing.

| **Regulation**                                | **Key ENISA Focus / Articles**                                                                                                                                                | **What ENISA Expects**                                                                                                                                                     | **Utility-Specific Compliance Actions**                                                                                                                                     | **Deliverables / Evidence**                                                                                     |
| :-------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------- |
| **NIS2 Directive (Directive (EU) 2022/2555)** | - `Art. 21`: Security & Risk Mgmt  <br> - `Art. 23`: Incident Notification  <br> - `Art. 25`: Supervision  <br> - `ENISA Baseline Measures (2023)`                              | - Board-level cybersecurity accountability  <br> - Risk management & policy framework  <br> - Supply chain & incident control  <br> - `24h/72h/1-month incident reporting`   | - Map `OT/IT network` & secure data flows (Azure + IoT)  <br> - `CIRATS integration` for rapid incident alerts  <br> - Adopt `ENISA Baseline 49 Controls`                       | - Risk Register (aligned to `ISO 27001`)  <br> - Incident Response Plan & Reports  <br> - `NIS2 Compliance Matrix`  |
| **EU AI Act (Reg. (EU) 2024/1689)**           | - `Art. 9`: Risk Mgmt System  <br> - `Art. 14`: Human Oversight (`HITL`)  <br> - `Art. 15`: Accuracy & Robustness  <br> - `Annex III (High-Risk AI)`  <br> - `Annex IV (Conformity File)` | - Secure & transparent AI systems  <br> - `HITL` oversight and accountability  <br> - Documentation of data sources & model lineage  <br> - Bias, drift & robustness testing | - Identify AI systems as `“high-risk”` (leak detection, anomaly detection)  <br> - Define `HITL` process (Databricks workflow)  <br> - Implement `AI risk register + model cards` | - `AI Risk Assessment`  <br> - `HITL Roles & Log Evidence`  <br> - Model Cards & Technical File (`Annex IV`)          |
| **EU Cyber Resilience Act (CRA)**             | - `Annex I`: Security by Design  <br> - `Annex II`: CE Marking  <br> - `Art. 10–11`: Vulnerability Disclosure  <br> - `ENISA IoT Security Guidelines`                             | - Secure product lifecycle (`SDLC`)  <br> - Continuous vulnerability management  <br> - Transparent update & patch policy  <br> - Disclosure process within `24h`              | - Apply `ENISA CRA IoT guidelines` to smart meters/gateways  <br> - `SBOM (Software Bill of Materials)` for all firmware  <br> - Integrate `CRA conformity checks` in `CI/CD`       | - `CE Technical Documentation`  <br> - `SBOM` + Patch Logs  <br> - `CRA Declaration of Conformity`                    |
| **ISO 27001 Alignment (2022 Update)**         | - `ENISA ISMS Maturity Model`  <br> - `Annex A cross-mapping`                                                                                                                     | - Continuous improvement loop for `ISMS`  <br> - Risk & control verification  <br> - Audit trail integrity                                                                   | - Map `ENISA baseline → ISO controls`  <br> - Embed `NIS2/AI/CRA` controls into `ISMS`                                                                                            | - `ISO 27001 Readiness Audit Pack`  <br> - Control Evidence Summary                                               |
| **Cross-Regulation Governance**               | - `ENISA Cybersecurity Maturity Model`  <br> - `Threat Landscape 2024`  <br> - `Incident Notification Templates`                                                                    | - Unified governance model across regulations  <br> - Clear accountability and risk visibility  <br> - Automated evidence and dashboards                                   | - Deploy **CIR³ framework** (Continuous Intelligence, Integration, Resilience)  <br> - `Sentinel` & `Grafana dashboards`  <br> - Compliance dashboard for board oversight           | - Unified Compliance Dashboard  <br> - `ENISA-formatted Quarterly Report`  <br> - Cross-Regulation Control Matrix |

---

# NIS2 Directive – Core Control Requirements Checklist

*Aligned with `ENISA`, `NIS2 Directive Articles 21 & 23`, and `ISO/IEC 27001` Control Mapping*

This checklist provides a high-level overview of core control requirements from the `NIS2 Directive`, focusing on actionable objectives and linking them to specific articles for rapid assessment.

| **Requirement**                                    | **Control Objective**                                                                                            | **Linked Article / Reference** | **Status / Implementation Evidence**      |
| :------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------- | :----------------------------- | :---------------------------------------- |
| **Asset Inventory in CMDB**                        | Ensure all critical assets and systems are identified, tracked, and linked to `configuration management database`. | `Art. 21(2)(a)`                | ☐ Entry exists in `CMDB` (ID recorded)      |
| **Vulnerability Management Process**               | Establish continuous vulnerability identification, assessment, and remediation with defined schedule.            | `Art. 21(2)(d)`                | ☐ Linked process and schedule defined     |
| **Incident Reporting & Contact Runbook**           | Implement reporting procedures, including defined roles and escalation contacts, integrated into repository.     | `Art. 23`                      | ☐ Incident response runbook documented    |
| **Backup & Recovery Procedures**                   | Maintain tested and documented backup and recovery plans to ensure business continuity.                          | `Art. 21(2)(e)`                | ☐ Backup and recovery tested and verified |
| **Supplier Risk Assessment**                       | Evaluate suppliers, dependencies, and containers for security posture and contractual risk.                      | `Art. 21(2)(d,f)`              | ☐ Supplier risk analysis completed        |
| **Data Transfer & Legal Basis (Conditional – EU)** | Validate `GDPR` and cross-border data transfer compliance for EU-based processing.                                 | `GDPR / NIS2 interplay`        | ☐ Data transfer and legal basis reviewed  |

---

# NIS2 Directive – Databricks on Azure Implementation Checklist

*Aligned with `ENISA Baseline Measures` · `ISO/IEC 27001 Annex A` · `Preventio Leak Detection Platform`*

This checklist details specific technical configurations and data processing practices for implementing `NIS2` controls within a Databricks on Azure environment, focusing on evidence and auditability.

| **NIS2 Control**                           | **Databricks / Azure Configuration**                                                 | **Data Processing Practice (Bronze → Silver → Gold)**                                   | **Audit Evidence / Notes**                                                   |
| :----------------------------------------- | :----------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------- |
| **Asset Inventory (`Art.21(2)(a)`)**       | Use `Unity Catalog` for asset registration and `Azure Resource Graph` to sync resources to `ServiceNow CMDB`. | Register every dataset, Delta table, and ML model with owner, classification, and retention policy. | `CMDB` record IDs, `Unity Catalog` ownership reports, configuration snapshots. |
| **Vulnerability Management (`Art.21(2)(d)`)** | Apply Databricks cluster policies, enforce runtime pinning, enable `Defender for Cloud`, and scan base images for vulnerabilities. | Integrate vulnerability scanning in `CI/CD pipeline`; perform monthly runtime upgrade validation cycles. | `Defender` vulnerability reports, `CI/CD pipeline` logs, runtime upgrade tickets. |
| **Incident Reporting (`Art.23`)**          | Stream Databricks audit logs to `Microsoft Sentinel` and trigger `Logic Apps` for automated `24-hour incident notifications`. | Tag each incident with related `Unity Catalog` dataset and responsible owner for traceability. | `Sentinel` alerts, `Logic App` execution reports, incident documentation (`24h/72h`). |
| **Backup & Recovery (`Art.21(2)(e)`)**     | Enable `ADLS versioning` and soft delete, `Delta Lake time travel`, and `MLflow model versioning` with `GRS replication`. | Conduct quarterly restore tests for Delta tables and ML models to validate `RPO/RTO performance`. | Restore logs, test reports, validation screenshots.                            |
| **Supplier Risk (`Art.21(2)(d,f)`)**       | Enforce `Private Link` for Databricks, `ADLS`, and `Event Hub`; apply EU-only region policies; `PIM/MFA` and `SCIM sync` for identity management. | Approve `Azure Container Registry` images through security review; maintain `SBOM` for all dependencies. | Supplier `SLA`, `ACR` scan reports, `Azure Policy` compliance exports.           |
| **Data Transfer & Legal (`GDPR/NIS2`)**    | Use `Microsoft Purview` for lineage and sensitivity labeling; enforce column-level masking via `Unity Catalog`. | Hash or remove `PII` at Silver layer; ensure Gold layer aggregates are anonymized and EU-based. | `Purview` lineage exports, `Unity Catalog` masking `DDLs`, `GDPR DPA/DTIA documentation`. |
| **Risk & Monitoring (`Art.21(2)(a,b)`)**   | Leverage `Delta Expectations`, `Job ACLs`, and `Sentinel analytics` for anomaly detection and proactive monitoring. | Use `MLflow metrics` for model drift tracking and trigger alerts on threshold breaches. | `MLflow drift reports`, `Sentinel incidents`, and alert logs.                   |
| **Access Control (`Art.21(2)(c)`)**        | Apply `Unity Catalog RBAC`, `SCIM group sync`, and `service principal-based authentication` to enforce least privilege. | Use separate service accounts for pipelines; conduct periodic access reviews every `6–12 months`. | `UC GRANT` exports, `SCIM sync logs`, access review approvals.                 |
| **Change Control (`Art.21(2)(g)`)**        | Use `Azure DevOps` or `GitHub Actions` for `CI/CD`; enforce `four-eyes approval` for production promotion and `PR validation`. | Ensure all notebook, job, and cluster policy changes are version-controlled with review gates. | Pull request approvals, release notes, and version control audit trails.       |

---

### Pipeline Reference

This describes a typical secure data pipeline architecture leveraging Azure and Databricks for critical infrastructure data processing.

```
IoT Hub → Event Hub → ADLS (Private Endpoints) → Databricks Bronze → Silver → Gold Zones → MLflow Registry → Power BI/APIs → Sentinel Monitoring & Purview Lineage
```

---

**Prepared by:** Thinkwerke – Strategy Meets Security
**Date:** October 2025

---

# EU AI Act Compliance Checklist

### Databricks on Azure – Water Leak Detection AI (Utilities / Critical Infrastructure – Germany)

*Aligned with `EU AI Act (Reg. EU 2024/1689)`, `ENISA AI Security Framework`, and `ISO/IEC 42001`*

This checklist details the practical implementation steps for complying with the `EU AI Act` using Databricks on Azure, specifically tailored for a `high-risk` AI system like a water leak detection platform in critical infrastructure.

| **AI Act Requirement**          | **Description / Intent**                                                                        | **Implementation on Databricks (Azure)**                                 | **Evidence / Deliverables**                              | **Linked Articles / Annexes**             |
| :------------------------------ | :---------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------- | :---------------------------------------- |
| **AI System Classification**    | Determine if system is *high-risk* under `Annex III` (critical infrastructure & water management). | Classify leak detection models as *High-Risk AI*; register in compliance catalog. | AI System Register (with risk level, owner, and version). | `Art. 6–7`, `Annex III(1)(b)`             |
| **Risk Management Framework**   | Establish continuous risk identification, evaluation, and mitigation process for AI lifecycle.    | Deploy `AI Risk Register` in Databricks (`Delta table`); integrate with `Purview lineage` and `CI/CD risk gates`. | Risk Register, Mitigation Matrix, `CI/CD` logs.          | `Art. 9`                                  |
| **Data Governance & Quality**   | Ensure datasets are accurate, representative, and free from bias.                               | Manage datasets through `Unity Catalog` with source lineage, data validation notebooks, and bias detection scripts. | Data Quality Report, Bias Analysis Summary.              | `Art. 10(3–5)`                            |
| **Technical Documentation (Conformity File)** | Maintain detailed documentation of design, data sources, architecture, and version history. | Auto-generate documentation using `MLflow metadata` and model registry.    | Conformity File (`Annex IV` format).                     | `Art. 11`, `Annex IV`                     |
| **Record-Keeping & Logging**    | Enable traceability of operations, model updates, and decisions.                                | Store inference logs in `ADLS` and `MLflow`; log metadata (model ID, run ID, parameters). | `MLflow` Logs, Inference Audit Trail.                    | `Art. 12`                                 |
| **Transparency & Explainability** | Ensure users can interpret AI outputs and decisions.                                            | Implement `SHAP / LIME` explainability notebooks in Databricks; expose results in `Power BI dashboard`. | Explainability Report, Model Interpretability Metrics.   | `Art. 13`                                 |
| **Human Oversight (HITL)**      | Ensure `human-in-the-loop` validation for critical AI decisions.                                | Define `HITL` workflow in Databricks Jobs; approval steps triggered via `Logic Apps`. | `HITL` Policy Document, Event Logs, Approval Records.    | `Art. 14`                                 |
| **Accuracy, Robustness & Cybersecurity** | Maintain high levels of accuracy, resilience to drift, and protection from manipulation. | Track model drift with `MLflow metrics`; `Sentinel integration` for anomaly alerts; enforce runtime security. | Model Drift Report, `Sentinel` Logs, Adversarial Test Results. | `Art. 15`, `ENISA AI Security`            |
| **Conformity Assessment**       | Verify that the system meets EU harmonized standards before deployment.                         | Conduct internal pre-assessment; validate against `ENISA AI baseline` and `ISO/IEC 42001`. | Conformity Assessment Record, Validation Checklist.      | `Art. 43`, `Annex VI`                     |
| **Post-Market Monitoring**      | Continuously monitor AI performance and compliance after release.                               | Automate monitoring via `Sentinel` and `Grafana dashboards`; track incidents through **CIR³ framework**. | Monitoring Dashboard, Periodic AI Review Report.         | `Art. 61`, `Annex VII`                    |
| **Incident & Risk Reporting**   | Notify competent authority within `15 days` for serious incidents or non-compliance.            | Integrate `Logic App` alert pipeline for regulatory notifications and internal escalation. | Incident Report Template, Notification Logs.             | `Art. 62`                                 |
| **Data Protection & GDPR Alignment** | Ensure data minimization, lawful basis, and data subject rights.                                | Use `Purview DLP classification`; anonymize datasets at Silver layer before model training. | `DPA / DTIA` Reports, Data Masking Proofs.               | `GDPR Art. 5–6`, `AI Act Recital 44`      |
| **Supplier & Third-Party Model Control** | Manage third-party AI models and libraries under `CRA/NIS2` supply chain obligations.     | Maintain `SBOM` and version tracking in `ACR`; validate dependencies with `Defender for DevOps`. | `SBOM` File, Dependency Security Report.                 | `Art. 28`, `CRA Annex II`                 |
| **Accountability & Governance** | Assign roles and document decision-making responsibilities.                                     | Define `AI Compliance Officer` role in `Azure AD`; map to organizational `RACI` under **CIR³ Framework**. | Governance Matrix, Role Register.                        | `Art. 29`, `ENISA Governance Baseline`    |

---

### Integration with Thinkwerke CIR³ Framework

The **Thinkwerke CIR³ Framework** (Continuous Intelligence · Integration · Resilience) ensures a holistic approach to compliance by:

*   Providing unified governance across `NIS2`, `AI Act`, `CRA`, and `ISO 27001`.
*   Establishing an `ENISA-compliant` evidence trail and dashboard view for internal audits and regulatory reporting.
*   Enabling `HITL` accountability, comprehensive data traceability, and robust model lifecycle assurance.

---

### Summary

> Implementing the `EU AI Act` within a Databricks on Azure environment provides not only compliance, but also continuous assurance and operational excellence.
> By connecting foundational governance (`NIS2`) and product resilience (`CRA`) through unified `AI lifecycle management`, utilities gain crucial **transparency, safety, and trust — all essential for EU market readiness**.

---

**Prepared by:** Thinkwerke – Strategy Meets Security
**Date:** October 2025
