# Framework Mapping Matrix

**EU AI Act ↔ NIST AI RMF ↔ ISO/IEC 42001 ↔ DORA**

*Last reviewed: 2026-08*

> **Orientation, not legal advice.** This matrix shows where four frameworks address a comparable
> governance requirement. It is a starting point for scoping, not a compliance mapping and not a
> substitute for legal or supervisory advice. A row on the same line does **not** mean the
> requirements are equivalent in scope, addressee, or legal effect — only that they concern the
> same subject. Verify every reference against the primary text before relying on it.

## Reading the columns

| Column | Source used | Note |
| ------ | ----------- | ---- |
| **EU AI Act** | [Regulation (EU) 2024/1689](https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng), as amended by [Regulation (EU) 2026/1744](https://eur-lex.europa.eu/eli/reg/2026/1744/oj/eng) (the "Digital Omnibus on AI") | Most rows cite Chapter III obligations for **high-risk** AI systems. These do not apply to every AI system — see *Applicability* below. |
| **NIST AI RMF** | [AI RMF 1.0 (NIST AI 100-1)](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf) | Cited by function and subcategory (GOVERN / MAP / MEASURE / MANAGE). Outcomes, not controls. |
| **ISO/IEC 42001** | ISO/IEC 42001:2023 | Numbered clauses (4–10) are requirements; `A.x` are Annex A reference controls. The standard is paywalled; only structure and titles are reproduced here. |
| **DORA** | [Regulation (EU) 2022/2554](https://eur-lex.europa.eu/eli/reg/2022/2554/oj/eng) | **DORA is not an AI framework.** It regulates ICT risk and operational resilience for EU financial entities. It is included because most productive AI workloads in EU finance run on ICT arrangements DORA governs — but several rows below have no DORA counterpart, and that is stated rather than papered over. |

---

## Main matrix

### Risk Management

| | |
| --- | --- |
| **EU AI Act** | Art. 9 — risk management system for high-risk AI, a continuous iterative process run and documented across the whole lifecycle. Art. 6 + Annex III determine whether it applies at all. Art. 27 — fundamental rights impact assessment, for certain deployers. |
| **NIST AI RMF** | MAP 1.5 (risk tolerances determined), MAP 5.1 (likelihood and magnitude of each identified impact), MANAGE 1.2 (treatment prioritised by impact, likelihood, resources), MANAGE 1.3 (responses to high-priority risks developed and documented), MANAGE 1.4 (negative residual risks documented). |
| **ISO/IEC 42001** | 6.1.2 AI risk assessment, 6.1.3 AI risk treatment, 6.1.4 AI system impact assessment; 8.2/8.3/8.4 operational execution of the same; A.5.2 AI system impact assessment process. |
| **DORA** | Art. 6 — ICT risk management framework, documented, reviewed at least annually (Art. 6(5)); Art. 8–11 identification, protection and prevention, detection, response and recovery; Art. 16 simplified framework for smaller entities. **Scope is ICT risk, not model risk.** |

### Governance / Accountability Structure

| | |
| --- | --- |
| **EU AI Act** | Art. 16 obligations of providers; Art. 17 quality management system; Art. 26 obligations of deployers; Art. 25 responsibilities along the AI value chain (including when a deployer becomes a provider); Art. 22 authorised representatives; Art. 4 AI literacy of staff. |
| **NIST AI RMF** | GOVERN 1.1 (legal and regulatory requirements understood and documented), GOVERN 1.3, GOVERN 2.1 (roles, responsibilities and lines of communication), GOVERN 2.3 (executive leadership takes responsibility), GOVERN 3.2 (roles for human–AI configurations and oversight). |
| **ISO/IEC 42001** | 5.1 leadership and commitment, 5.2 AI policy, 5.3 roles, responsibilities and authorities; A.2.2 AI policy, A.2.3 alignment with other organisational policies, A.3.2 AI roles and responsibilities, A.3.3 reporting of concerns. |
| **DORA** | Art. 5 governance and organisation — the **management body** defines, approves, oversees and bears ultimate responsibility (Art. 5(2)(a)), sets roles for ICT functions (Art. 5(2)(c)), and must keep its own ICT knowledge current (Art. 5(4)). Art. 5(3) requires a designated role monitoring ICT third-party arrangements. Art. 6(4) requires an independent ICT risk control function. |

### Documentation & Transparency

| | |
| --- | --- |
| **EU AI Act** | Art. 11 + Annex IV technical documentation; Art. 13 transparency and provision of information to deployers (instructions for use); Art. 18 documentation keeping; Art. 47 EU declaration of conformity; Art. 50 transparency obligations for certain AI systems (disclosure of AI interaction, marking of synthetic content); Art. 53(1) + Annexes XI and XII for general-purpose AI models; Art. 86 right to explanation of individual decision-making. |
| **NIST AI RMF** | GOVERN 1.4 (risk management process and outcomes transparent), GOVERN 4.2 (teams document and communicate risks and impacts), MAP 2.2 (knowledge limits documented), MEASURE 2.8 (transparency and accountability risks examined), MEASURE 2.9 (model explained, validated and documented). |
| **ISO/IEC 42001** | 7.5 documented information; A.6.2.3 documentation of AI system design and development, A.6.2.7 AI system technical documentation, A.8.2 system documentation and information for users, A.8.5 information for interested parties. |
| **DORA** | Art. 28(3) — register of information covering **all** contractual arrangements on the use of ICT services, maintained at entity, sub-consolidated and consolidated level, produced to the competent authority on request; templates in [Implementing Regulation (EU) 2024/2956](https://eur-lex.europa.eu/eli/reg_impl/2024/2956/oj/eng). This documents the ICT arrangement, **not** the model. |

### Human Oversight

| | |
| --- | --- |
| **EU AI Act** | Art. 14 — the strongest text of the four. High-risk systems must be designed so natural persons can effectively oversee them (14(1)); oversight must be commensurate with **risk, level of autonomy and context of use** (14(3)); the overseer must be able to disregard, override or reverse the output (14(4)(d)) and to interrupt the system through a stop button or equivalent, halting it in a safe state (14(4)(e)); 14(4)(b) addresses automation bias. Art. 26(2) — the deployer must assign oversight to persons with the necessary competence, training, authority and support. |
| **NIST AI RMF** | GOVERN 3.2 (policies define and differentiate roles for human–AI configurations and oversight), MAP 3.5 (processes for human oversight defined, assessed and documented), MANAGE 2.4 (mechanisms and assigned responsibilities to **supersede, disengage or deactivate** systems behaving inconsistently with intended use). |
| **ISO/IEC 42001** | No control titled "human oversight". The nearest are A.9.2 processes for responsible use of AI systems, A.9.4 intended use of the AI system, and A.6.2.6 AI system operation and monitoring. Human oversight is expressible under 42001, but the standard does not prescribe it as a discrete control. |
| **DORA** | **No counterpart.** DORA governs the resilience of ICT systems, not human oversight of model outputs. The adjacent obligation is management-body accountability (Art. 5(2)) — governance of the function, not of individual decisions. |

### Robustness / Security

| | |
| --- | --- |
| **EU AI Act** | Art. 15 — accuracy, robustness and cybersecurity across the lifecycle; 15(4) resilience against errors, faults and inconsistencies, including feedback loops in systems that keep learning after deployment; 15(5) resilience against unauthorised third parties altering use, outputs or performance by exploiting vulnerabilities. Art. 55(1)(a) adversarial testing and (1)(d) cybersecurity for general-purpose AI models with systemic risk. |
| **NIST AI RMF** | MEASURE 2.5 (system demonstrated to be valid and reliable before deployment), MEASURE 2.6 (regular safety evaluation), MEASURE 2.7 (security and resilience evaluated and documented), MEASURE 2.13 (effectiveness of the TEVV metrics themselves). |
| **ISO/IEC 42001** | A.6.2.4 AI system verification and validation; A.4.4 tooling resources and A.4.5 system and computing resources. 42001 does not restate an information-security control set — that regime is expected to sit alongside it. |
| **DORA** | The deepest column. Art. 9 protection and prevention, Art. 10 detection, Art. 11 response and recovery, Art. 12 backup and restoration; Art. 24–25 digital operational resilience testing, Art. 26–27 threat-led penetration testing (TLPT) and tester requirements; detail in [Delegated Regulation (EU) 2024/1774](https://eur-lex.europa.eu/eli/reg_del/2024/1774/oj/eng). |

### Incident Reporting

| | |
| --- | --- |
| **EU AI Act** | Art. 73 — serious incidents reported to market surveillance authorities: not later than **15 days** after awareness (73(2)), **2 days** for a widespread infringement or an incident under Art. 3(49)(b) (73(3)), **10 days** where a person has died (73(4)); an incomplete initial report is permitted (73(5)). Art. 20 corrective actions and duty of information; Art. 26(5) deployer duty to inform provider and authority and to suspend use; Art. 79 procedure for systems presenting a risk; Art. 87 protection of reporting persons. |
| **NIST AI RMF** | GOVERN 4.3 (practices enabling testing, identification of incidents, and information sharing), MANAGE 4.1 (post-deployment plans include incident response and recovery), MANAGE 4.3 (incidents and errors communicated to relevant AI actors including affected communities; tracking and recovery documented). No reporting deadlines — it is a voluntary framework. |
| **ISO/IEC 42001** | A.8.4 communication of incidents, A.8.3 external reporting; 10.2 nonconformity and corrective action. |
| **DORA** | Art. 17 ICT-related incident management process, Art. 18 classification of incidents and cyber threats, Art. 19 reporting of major ICT-related incidents and voluntary notification of significant cyber threats, Art. 22 supervisory feedback, Art. 23 payment-related operational or security incidents; classification criteria, materiality thresholds and report content in [Delegated Regulation (EU) 2024/1772](https://eur-lex.europa.eu/eli/reg_del/2024/1772/oj/eng). |

### Third-Party / Supply Chain

| | |
| --- | --- |
| **EU AI Act** | Art. 25 responsibilities along the AI value chain; Art. 53 obligations of providers of general-purpose AI models, including the information to be passed to downstream providers (Annex XII); Art. 23 importers, Art. 24 distributors. |
| **NIST AI RMF** | GOVERN 6.1 (policies addressing third-party risks, including IP infringement), GOVERN 6.2 (contingency processes for failures or incidents in third-party data or AI systems deemed high-risk), MAP 4.1 (mapping technology and legal risks of components including third-party data or software), MAP 4.2 (internal risk controls for third-party components), MANAGE 3.1 (third-party risks monitored, controls applied and documented), MANAGE 3.2 (**pre-trained models monitored** as part of regular maintenance). |
| **ISO/IEC 42001** | A.10.2 allocating responsibilities, A.10.3 suppliers, A.10.4 customers; A.4.3 data resources, A.7.3 acquisition of data. |
| **DORA** | The strongest column in the matrix. Art. 28 general principles, including the register of information (28(3)) and pre-contractual assessment (28(4)); Art. 29 preliminary assessment of ICT concentration risk; Art. 30 key contractual provisions; Art. 31–44 the Oversight Framework for **critical** ICT third-party service providers, including designation (Art. 31), the Lead Overseer (Art. 33, 35), inspections (Art. 39) and ongoing oversight (Art. 40). Contracting detail in [Delegated Regulation (EU) 2024/1773](https://eur-lex.europa.eu/eli/reg_del/2024/1773/oj/eng); subcontracting of critical or important functions in [Delegated Regulation (EU) 2025/532](https://eur-lex.europa.eu/eli/reg_del/2025/532/oj/eng). |

### Monitoring & Post-Market

| | |
| --- | --- |
| **EU AI Act** | Art. 72 — post-market monitoring system based on a documented plan that forms part of the Annex IV technical documentation; as amended by Regulation (EU) 2026/1744, the Commission is to issue guidance and a template by 2 September 2027. Art. 26(5) deployer monitoring against the instructions for use; Art. 74 market surveillance. |
| **NIST AI RMF** | GOVERN 1.5 (ongoing monitoring and periodic review of the risk management process), MANAGE 4.1 (post-deployment monitoring plans, including **appeal and override**, decommissioning, incident response, change management), MANAGE 4.2 (measurable continual improvement integrated into updates), MEASURE 2.6 (regular safety evaluation), MEASURE 4.2 (measurement results reviewed by domain experts and users). |
| **ISO/IEC 42001** | 9.1 monitoring, measurement, analysis and evaluation; 10.1 continual improvement; A.6.2.6 AI system operation and monitoring. |
| **DORA** | Art. 10 detection (mechanisms to promptly detect anomalous activities), Art. 13 learning and evolving (post-incident review feeding back into the framework), Art. 6(5) at-least-annual review of the framework. |

### Data Quality / Data Governance

| | |
| --- | --- |
| **EU AI Act** | Art. 10 — data and data governance for training, validation and testing sets: relevance, representativeness, error handling, examination for bias, data-collection provenance. Art. 26(4) deployer duty on relevance of input data where it controls it. Art. 4a (inserted by Regulation (EU) 2026/1744) permits processing of special categories of personal data strictly for bias detection and correction, under enumerated safeguards. |
| **NIST AI RMF** | The core framework has **no dedicated data-governance category**. The nearest outcomes are MAP 2.3 (scientific integrity and TEVV considerations), MEASURE 2.10 (privacy risk examined and documented), MEASURE 2.11 (fairness and bias examined and documented). This is a real gap relative to the AI Act and ISO/IEC 42001. |
| **ISO/IEC 42001** | The most explicit column. A.7.2 data for development and enhancement, A.7.3 acquisition of data, A.7.4 quality of data for AI systems, A.7.5 data provenance, A.7.6 data preparation; A.4.3 data resources. |
| **DORA** | Art. 5(2)(b) — policies maintaining high standards of **availability, authenticity, integrity and confidentiality** of data; Art. 12 backup, restoration and recovery. This is data integrity and availability, not training-data quality or representativeness. |

### Auditability

| | |
| --- | --- |
| **EU AI Act** | Art. 12 record-keeping — automatic recording of events (logs) over the lifetime of the system, at a level of traceability appropriate to the intended purpose; Art. 19 provider log retention of **at least six months**; Art. 26(6) the same duty on deployers for logs under their control; Art. 17 quality management system; Art. 18 documentation keeping; Art. 21 cooperation with competent authorities; Art. 43 conformity assessment, with Annex VII covering assessment of the quality management system and the technical documentation. |
| **NIST AI RMF** | GOVERN 1.4 (process and outcomes documented through transparent policies), GOVERN 1.6 (mechanisms to **inventory** AI systems), MEASURE 1.3 (testing involving internal experts who were not front-line developers), MEASURE 3.1 (approaches, personnel and documentation for tracking identified risks). |
| **ISO/IEC 42001** | 9.2 internal audit, 9.3 management review, 7.5.3 control of documented information; A.6.2.8 AI system recording of event logs. This is the only column of the four that is **certifiable** by an accredited body — which is usually why it appears in an audit conversation at all. |
| **DORA** | Art. 5(2)(f) management-body approval and review of ICT internal audit plans; Art. 6(6) the ICT risk management framework is subject to internal audit by auditors with sufficient ICT expertise; Art. 6(7) formal follow-up and remediation of critical ICT audit findings; Art. 37–39 supervisory information requests, investigations and inspections in respect of critical ICT third-party providers. |

---

## Which framework for what

| | **EU AI Act** | **NIST AI RMF 1.0** | **ISO/IEC 42001:2023** | **DORA** |
| --- | --- | --- | --- | --- |
| **Purpose** | Place AI systems on the EU market lawfully; product-safety-style obligations tiered by risk, plus a separate regime for general-purpose AI models. | Give an organisation a shared structure for identifying, measuring and treating AI risk, and for documenting the decisions. | Run an auditable **AI management system**: ownership, controls, monitoring, continual improvement. | Keep EU financial entities operationally resilient to ICT disruption, and bring their critical ICT providers under supervision. |
| **Binding?** | **Binding** EU regulation, directly applicable. Not "certifiable"; high-risk systems undergo conformity assessment and CE marking, and harmonised standards give a presumption of conformity (Art. 40, 42). | **Voluntary.** Not certifiable. No conformity mechanism. | **Voluntary to adopt, certifiable** by an accredited certification body — the only one of the four that produces a certificate. | **Binding** EU regulation, directly applicable, in application since **17 January 2025** (Art. 64). |
| **Scope** | AI systems and general-purpose AI models placed on the market or put into service in the EU, plus certain third-country uses whose output is used in the EU (Art. 2). | Any organisation, any sector, any jurisdiction. Technology- and lifecycle-neutral. | Any organisation that develops, provides or uses AI, of any size, in any sector. | ~20 categories of EU financial entities plus designated critical ICT third-party service providers. **ICT resilience — not AI.** |
| **Audience** | Providers, deployers, importers, distributors; market surveillance authorities; notified bodies. | Risk, engineering, product and policy functions that need one vocabulary across disciplines. | Management-system owners, second line, internal and external auditors. | Management body, ICT risk control function, outsourcing and procurement, competent authorities. |
| **Applicability note** | Chapters I and II applied from 2 February 2025. The general date of application is 2 August 2026. Regulation (EU) 2026/1744 amended Art. 113: the **high-risk** obligations in Chapter III Sections 1–3 now apply from **2 December 2027** for Annex III systems and **2 August 2028** for Annex I embedded systems. Most Chapter III rows above are therefore not yet in application. | — | Structure follows the ISO harmonised management-system format, so it composes with ISO/IEC 27001 and ISO 9001 rather than replacing them. | Applies regardless of whether AI is involved. It reaches AI workloads because they run on ICT services, ICT third parties and ICT arrangements. |

---

## Agentic AI specifics

Where the frameworks bite hardest once an agent holds tool access, credentials and the ability to
act — and where they run out.

1. **Human oversight scales with autonomy, and the AI Act says so explicitly.** Art. 14(3) makes the
   oversight measures commensurate with the *level of autonomy* and context of use. For a high-risk
   agent, Art. 14(4)(d) (disregard, override, reverse the output) and 14(4)(e) (interrupt through a
   stop button that halts the system in a safe state) are the two clauses most likely to shape the
   architecture, not the documentation.

2. **A kill switch is the one requirement all three AI frameworks converge on.** AI Act Art. 14(4)(e),
   NIST MANAGE 2.4 (supersede, disengage or deactivate), and — read together — ISO/IEC 42001 A.9.2
   and A.6.2.6. If an agent cannot be stopped mid-execution, three frameworks are unsatisfied at once.

3. **Logging is a hard requirement, and agent action logs are what it should capture.** AI Act
   Art. 12 requires automatic event recording over the system's lifetime, Art. 19 and Art. 26(6)
   require retention of at least six months on the provider and deployer side respectively, and
   ISO/IEC 42001 A.6.2.8 asks for event logs as a control. None of them specify that the log must
   record *which tool the agent called, with what arguments, under whose authority*.

4. **Action authorisation is the largest gap.** No framework in this matrix defines a pre-execution
   authorisation gate for an individual agent action. The AI Act's closest analogue is Art. 14(5) —
   confirmation by two natural persons — and it applies only to remote biometric identification, not
   to agents generally. NIST MANAGE 4.1 mentions *appeal and override*, a post-hoc remedy rather
   than a gate. The most concrete published treatment is the MAS-convened
   [SAFR](https://www.mas.gov.sg/publications/monographs-or-information-paper/2026/safeguards-for-agentic-finance-at-runtime)
   paper, which is an industry white paper, not a supervisory expectation.

5. **Delegated identity and credentials are not addressed anywhere.** An agent acting under a service
   account, or under a human's delegated authority, raises questions of attribution and revocation
   that none of the four frameworks answer. DORA governs the ICT arrangement; the AI Act governs the
   system; neither governs the identity the agent acts under.

6. **Third-party risk is well covered — for the model, less so for the tools.** DORA Art. 28–30 and
   the register of information under Art. 28(3) capture the ICT services an agent depends on, and
   NIST MANAGE 3.2 asks that pre-trained models be monitored. What is not captured is the transitive
   surface an agent reaches at runtime: the MCP servers, APIs and data sources it can call, which may
   never appear in a contractual register.

7. **Multi-agent and emergent behaviour is out of scope everywhere.** Every framework here assumes a
   system with a definable intended purpose. AI Act Art. 15(4) addresses feedback loops in systems
   that continue to learn, which is the nearest text, but nothing addresses interaction effects
   between several agents, or an agent whose effective scope of action is defined by the tools it
   happens to be given.

8. **Incident reporting deadlines assume a human notices.** AI Act Art. 73(2)–(4) and DORA Art. 19
   run from the moment of awareness. For an agent operating continuously and unattended, the design
   question the frameworks do not answer is what makes the organisation *aware* in the first place —
   which is a detection requirement (DORA Art. 10, NIST MEASURE 2.6) doing work the reporting
   articles quietly presuppose.

---

## Verification

Article numbers and titles for the EU AI Act and DORA were extracted from the EUR-Lex texts of
Regulation (EU) 2024/1689, Regulation (EU) 2026/1744 and Regulation (EU) 2022/2554. NIST references
were taken from NIST AI 100-1. ISO/IEC 42001 clause and Annex A references reflect the published
structure of the standard, which is paywalled and not reproduced here.

Where a framework has no counterpart for a row, this document says so rather than inventing one.

Corrections are welcome — see [contributing.md](contributing.md).
