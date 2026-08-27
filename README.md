# Awesome AI Governance [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of regulations, standards, risk frameworks, security resources, and open-source tools for governing AI systems — with a focus on agentic AI in regulated environments.

**NOTICE:** This list is curated, not exhaustive. Entries are grouped by topic and then by region, because a single document is often several things at once — the EU AI Act is regulation, transparency, and risk management in one. Entries carry a machine-readable tag comment in the source (`GEO`, `LEVEL`, `TOPIC`, `STATUS`, `SECTOR`, `TYPE`), except under *Related Awesome Lists* and *Maintainer*; the fields are documented in `contributing.md`. A ⭐ marks the sources I open first in an engagement. "Europe" is not "EU": the European Union is a supranational legal order, while the Council of Europe covers 46 states and works from a human-rights basis. Vendor marketing content is out of scope.

**→ [Framework Mapping: EU AI Act ↔ NIST AI RMF ↔ ISO/IEC 42001 ↔ DORA](FRAMEWORK-MATRIX.md)** — ten governance requirements mapped across the four frameworks, with article, function, and clause references.

## Contents

- [How I Use This List](#how-i-use-this-list)
- [Regulations & Law](#regulations--law)
- [Standards & Technical Specifications](#standards--technical-specifications)
- [Principles, Frameworks & Strategies](#principles-frameworks--strategies)
- [Risk, Safety & Incidents](#risk-safety--incidents)
- [Security & Resilience](#security--resilience)
- [Agentic AI Governance](#agentic-ai-governance)
- [Evaluation, Assurance & Red Teaming](#evaluation-assurance--red-teaming)
- [Transparency & Documentation](#transparency--documentation)
- [Reports, Monitoring & Policy Trackers](#reports-monitoring--policy-trackers)
- [Financial Services & Prudential AI Governance](#financial-services--prudential-ai-governance)
- [Sector-Specific Governance](#sector-specific-governance)
- [Related Awesome Lists](#related-awesome-lists)
- [Maintainer](#maintainer)

## How I Use This List

Five steps, in the order I actually run them on a regulated engagement. Deliberately unlinked — each source is one section below.

**1. EU AI Act.** Establish the legal role (provider or deployer), the risk classification, and the baseline obligations. Everything downstream depends on getting this right, and it is the step most often skipped.

**2. DORA and its ICT risk-management RTS.** For financial-sector deployments this is where operational resilience, critical dependencies, outsourcing, evidence, and incident management get pinned down. DORA is not an AI regulation — it is the substrate most productive AI and agentic workloads in finance actually run on.

**3. ISO/IEC 42001.** Turn the obligations into an auditable management system: ownership, controls, monitoring, continual improvement. This is what converts a legal analysis into something an auditor can accept.

**4. OWASP GenAI Security Project and MITRE ATLAS.** Map the concrete attack and failure paths. For agentic workflows — tool access, memory, delegated identity — this is where the real exposure sits, and where a purely legal analysis says nothing useful.

**5. NIST AI RMF.** The cross-functional structure for documenting governance decisions, risk treatment, test evidence, and residual risk. Useful even under EU law, because it gives the documentation a shape that non-lawyers can work with.

## Regulations & Law

### Europe

<!-- GEO: Europe | LEVEL: Regional | TOPIC: Regulation | STATUS: Binding | SECTOR: Cross-sector | TYPE: Law -->
- [EU AI Act — Regulation (EU) 2024/1689](https://eur-lex.europa.eu/eli/reg/2024/1689/oj) - Official legal text of the first comprehensive AI regulation, structured around a risk-based tiering of AI systems.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Regulation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [European Commission — AI Act policy page](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) - Official Commission hub for implementation guidance, delegated acts, and secondary legislation.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Regulation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [European Commission — AI Act governance and enforcement](https://digital-strategy.ec.europa.eu/en/policies/ai-act-governance-and-enforcement) - How the AI Act is actually enforced: AI Office, AI Board, national competent authorities, market surveillance, conformity assessment.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Regulation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [European AI Office](https://digital-strategy.ec.europa.eu/en/policies/ai-office) - The Commission body supervising general-purpose AI models and coordinating AI Act implementation across member states.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Regulation | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Framework -->
- [General-Purpose AI Code of Practice](https://digital-strategy.ec.europa.eu/en/policies/contents-code-gpai) - The voluntary instrument through which GPAI model providers demonstrate compliance with their AI Act obligations.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Regulation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Tool -->
- [AI Act Service Desk & Single Information Platform](https://ai-act-service-desk.ec.europa.eu/en) - Official Commission help desk and compliance assistant for organisations working out which AI Act obligations apply to them.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Regulation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Tool -->
- [EU AI Act Explorer](https://artificialintelligenceact.eu/) - Searchable, annotated version of the AI Act with a compliance checker and implementation timeline (Future of Life Institute).
<!-- GEO: Europe | LEVEL: International | TOPIC: Regulation | STATUS: Binding | SECTOR: Cross-sector | TYPE: Law -->
- [Council of Europe Framework Convention on AI](https://www.coe.int/en/web/artificial-intelligence/the-framework-convention-on-artificial-intelligence) - First legally binding international treaty on AI, framed around human rights, democracy, and the rule of law; open to non-European states.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Privacy | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Report -->
- [EDPB Opinion 28/2024 — AI models and data protection](https://www.edpb.europa.eu/our-work-tools/our-documents/opinion-board-art-64/opinion-282024-certain-data-protection-aspects_en) - Reference opinion on anonymity of models, legitimate interest, and the consequences of unlawfully processed training data.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Privacy | STATUS: Guidance | SECTOR: Public Sector | TYPE: Framework -->
- [European Data Protection Supervisor — Artificial Intelligence](https://www.edps.europa.eu/data-protection/our-work/subjects/artificial-intelligence_en) - Guidance on AI and data protection for EU institutions, including practical orientations on generative AI.
<!-- GEO: Europe | LEVEL: National | TOPIC: Privacy | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [ICO — Artificial intelligence (UK)](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/artificial-intelligence/) - UK regulator guidance on AI and data protection, including the AI and data protection risk toolkit.

### North America

<!-- GEO: North America | LEVEL: State/Province | TOPIC: Regulation | STATUS: Binding | SECTOR: Cross-sector | TYPE: Law -->
- [California SB 53 — Transparency in Frontier Artificial Intelligence Act](https://leginfo.legislature.ca.gov/faces/billNavClient.xhtml?bill_id=202520260SB53) - Frontier-model transparency and safety-incident reporting duties for large developers; the leading US state frontier-AI statute.
<!-- GEO: North America | LEVEL: State/Province | TOPIC: Regulation | STATUS: Binding | SECTOR: Cross-sector | TYPE: Law -->
- [Colorado SB24-205 — Consumer Protections for Artificial Intelligence](https://leg.colorado.gov/bills/sb24-205) - First broad US state law on algorithmic discrimination in consequential decisions, structured much like the EU AI Act's high-risk regime.
<!-- GEO: North America | LEVEL: National | TOPIC: Regulation | STATUS: Proposed | SECTOR: Cross-sector | TYPE: Law -->
- [Canada — Artificial Intelligence and Data Act (AIDA)](https://ised-isde.canada.ca/site/innovation-better-canada/en/artificial-intelligence-and-data-act) - Federal bill that died on the order paper with the January 2025 prorogation; the text and companion documents remain the reference point for Canadian AI regulation.
<!-- GEO: North America | LEVEL: State/Province | TOPIC: Regulation | STATUS: Binding | SECTOR: Cross-sector | TYPE: Database -->
- [IAPP US State AI Legislation Tracker](https://iapp.org/resources/article/us-state-ai-governance-legislation-tracker/) - Continuously updated tracker of enacted and pending US state-level AI governance laws.

### Asia-Pacific

<!-- GEO: Asia-Pacific | LEVEL: National | TOPIC: Regulation | STATUS: Binding | SECTOR: Cross-sector | TYPE: Law -->
- [China — Interim Measures for the Management of Generative AI Services](https://www.cac.gov.cn/2023-07/13/c_1690898327029107.htm) - Binding CAC rules on providers of public-facing generative AI services, including filing, labelling, and content obligations.
<!-- GEO: Asia-Pacific | LEVEL: National | TOPIC: Regulation | STATUS: Binding | SECTOR: Cross-sector | TYPE: Law -->
- [China — Provisions on Deep Synthesis Internet Information Services](https://www.cac.gov.cn/2022-12/11/c_1672221949318230.htm) - Binding rules on synthetic media and deepfakes; the origin of China's synthetic-content labelling regime.
<!-- GEO: Asia-Pacific | LEVEL: National | TOPIC: Regulation | STATUS: Binding | SECTOR: Cross-sector | TYPE: Law -->
- [South Korea — Framework Act on AI Development and Trust (English translation)](https://cset.georgetown.edu/publication/south-korea-ai-law-2025/) - Full English translation of the AI Basic Act, the second comprehensive national AI statute after the EU AI Act (CSET, Georgetown).
<!-- GEO: Asia-Pacific | LEVEL: National | TOPIC: Risk Management | STATUS: Proposed | SECTOR: Finance | TYPE: Framework -->
- [MAS — Proposed Guidelines on AI Risk Management](https://www.mas.gov.sg/publications/consultations/2025/consultation-paper-on-guidelines-on-artificial-intelligence-risk-management) - Singapore's supervisory expectations for financial institutions across the AI lifecycle, explicitly covering agentic use. Consultation of November 2025; supervisory expectations rather than legislation, with a transition period proposed before firms are expected to have implemented them.
<!-- GEO: Asia-Pacific | LEVEL: National | TOPIC: Regulation | STATUS: Binding | SECTOR: Cross-sector | TYPE: Tool -->
- [Korea AI Basic Act Explorer](https://aibasicact.kr/) - Article-by-article browsable version of the Korean AI Basic Act and its enforcement decree.

### Latin America

<!-- GEO: Latin America | LEVEL: National | TOPIC: Regulation | STATUS: Proposed | SECTOR: Cross-sector | TYPE: Law -->
- [Brazil — PL 2338/2023](https://www25.senado.leg.br/web/atividade/materias/-/materia/157233) - Brazil's comprehensive AI bill, approved by the Senate and now in the Chamber of Deputies; official dossier with full text and legislative history.

## Standards & Technical Specifications

### International

<!-- GEO: Global | LEVEL: International | TOPIC: Standard | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Framework -->
- [ISO/IEC 42001:2023 — AI Management Systems](https://www.iso.org/standard/81230.html) - The certifiable standard for establishing, implementing, and improving an AI management system (AIMS).
<!-- GEO: Global | LEVEL: International | TOPIC: Risk Management | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Framework -->
- [ISO/IEC 23894:2023 — AI Risk Management](https://www.iso.org/standard/77304.html) - Guidance on managing AI-related risk; the operational companion to ISO/IEC 42001.
<!-- GEO: Global | LEVEL: International | TOPIC: Risk Management | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Framework -->
- [ISO/IEC 42005:2025 — AI System Impact Assessment](https://www.iso.org/standard/42005) - Repeatable process for identifying and documenting the intended and unintended effects of an AI system on people and society.

### Europe

<!-- GEO: Europe | LEVEL: Regional | TOPIC: Standard | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Framework -->
- [CEN-CENELEC — Artificial Intelligence (JTC 21)](https://www.cencenelec.eu/areas-of-work/cen-cenelec-topics/artificial-intelligence/) - European standardisation work producing the harmonised standards that carry a presumption of conformity under the AI Act.

### North America

<!-- GEO: North America | LEVEL: National | TOPIC: Risk Management | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Framework -->
- [NIST AI Risk Management Framework (AI RMF 1.0)](https://www.nist.gov/itl/ai-risk-management-framework) - Voluntary framework structured around Govern, Map, Measure, and Manage; the de-facto benchmark outside the EU.
<!-- GEO: North America | LEVEL: National | TOPIC: Risk Management | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Framework -->
- [NIST AI 600-1 — Generative AI Profile](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf) - Companion profile to the AI RMF covering the risks specific to generative AI.
<!-- GEO: North America | LEVEL: National | TOPIC: Risk Management | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Tool -->
- [NIST Trustworthy & Responsible AI Resource Center](https://airc.nist.gov/) - Playbooks, glossary, and crosswalks for putting the AI RMF into practice.

## Principles, Frameworks & Strategies

### International

<!-- GEO: Global | LEVEL: International | TOPIC: Principles | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Framework -->
- [OECD AI Principles](https://oecd.ai/en/ai-principles) - The first intergovernmental AI standard (2019, updated 2024) and the source of the AI system definition used by the EU AI Act.
<!-- GEO: Global | LEVEL: International | TOPIC: Principles | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Framework -->
- [UNESCO Recommendation on the Ethics of AI](https://www.unesco.org/en/artificial-intelligence/recommendation-ethics) - Global normative framework adopted by 190+ member states, with a readiness assessment methodology for governments.
<!-- GEO: Global | LEVEL: International | TOPIC: Principles | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Framework -->
- [G7 Hiroshima AI Process](https://www.soumu.go.jp/hiroshimaaiprocess/en/index.html) - International guiding principles and code of conduct for organisations developing advanced AI systems.
<!-- GEO: Global | LEVEL: International | TOPIC: Principles | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Report -->
- [UN AI Advisory Body](https://www.un.org/en/ai-advisory-body) - The "Governing AI for Humanity" reports and the institutional groundwork for UN-level AI governance.

### Europe

<!-- GEO: Europe | LEVEL: National | TOPIC: Safety | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Report -->
- [UK AI Security Institute](https://www.aisi.gov.uk/) - Government research body publishing frontier-model evaluations, safety cases, and open evaluation tooling.

### North America

<!-- GEO: North America | LEVEL: National | TOPIC: Safety | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Report -->
- [Center for AI Standards and Innovation (CAISI)](https://www.nist.gov/aisi) - The NIST body responsible for US federal AI evaluation, standards, and testing work.
<!-- GEO: North America | LEVEL: National | TOPIC: Safety | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Policy -->
- [Anthropic Responsible Scaling Policy](https://www.anthropic.com/news/anthropics-responsible-scaling-policy) - A frontier lab's capability-threshold-based safety commitments; useful as a governance design pattern rather than as a norm.

### Asia-Pacific

<!-- GEO: Asia-Pacific | LEVEL: National | TOPIC: Principles | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [Japan — AI Guidelines for Business (METI/MIC)](https://www.meti.go.jp/shingikai/mono_info_service/ai_shakai_jisso/pdf/20260331_12.pdf) - Japan's soft-law guidance for AI developers, providers, and users across the system lifecycle (English, current version).
<!-- GEO: Asia-Pacific | LEVEL: National | TOPIC: Principles | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [Japan — Social Principles of Human-Centric AI](https://www8.cao.go.jp/cstp/english/humancentricai.pdf) - Cabinet Office principles that anchor Japan's human-centred, innovation-first approach to AI policy.
<!-- GEO: Asia-Pacific | LEVEL: National | TOPIC: Principles | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [Singapore — Model AI Governance Framework for Generative AI](https://aiverifyfoundation.sg/resources/mgf-gen-ai/) - Practical nine-dimension governance framework for deploying generative AI responsibly.
<!-- GEO: Asia-Pacific | LEVEL: National | TOPIC: Principles | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Framework -->
- [Australia — Guidance for AI Adoption](https://www.industry.gov.au/publications/guidance-for-ai-adoption) - Six essential practices for safe and responsible AI governance; the evolution of the Voluntary AI Safety Standard.
<!-- GEO: Asia-Pacific | LEVEL: National | TOPIC: Principles | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [India — AI Governance Guidelines](https://static.pib.gov.in/WriteReadData/specificdocs/documents/2025/nov/doc2025115685601.pdf) - MeitY's seven-principle, sector-regulator-led approach to AI governance, published under the IndiaAI Mission.

### Africa & Middle East

<!-- GEO: Africa | LEVEL: Regional | TOPIC: Principles | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [African Union — Continental Artificial Intelligence Strategy](https://au.int/en/documents/20240809/continental-artificial-intelligence-strategy) - Africa-wide strategy for developmental, inclusive, and rights-respecting AI adoption across member states.
<!-- GEO: Middle East | LEVEL: National | TOPIC: Principles | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [Saudi Data & AI Authority (SDAIA)](https://sdaia.gov.sa/en/default.aspx) - The national regulator publishing Saudi Arabia's AI ethics principles, generative AI guidelines, and data governance rules.
<!-- GEO: Middle East | LEVEL: National | TOPIC: Principles | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [Egypt — National Council for Artificial Intelligence](https://ai.gov.eg/) - Egypt's national AI strategy, charter of responsible AI, and implementation programmes.

## Risk, Safety & Incidents

### International

<!-- GEO: Global | LEVEL: International | TOPIC: Risk Management | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Database -->
- [MIT AI Risk Repository](https://airisk.mit.edu/) - Living database of 1,600+ AI risks extracted from taxonomies and frameworks, classified by cause and by domain.
<!-- GEO: Global | LEVEL: International | TOPIC: Safety | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Database -->
- [AI Incident Database (AIID)](https://incidentdatabase.ai/) - Community-maintained index of real-world AI harms and near-misses.
<!-- GEO: Global | LEVEL: International | TOPIC: Safety | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Database -->
- [OECD AI Incidents Monitor (AIM)](https://oecd.ai/en/incidents) - Automated global monitoring of AI incidents reported in news media, aligned with the OECD incident definition.
<!-- GEO: Global | LEVEL: International | TOPIC: Security | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Database -->
- [AI Vulnerability Database (AVID)](https://avidml.org/) - Open taxonomy and database of failure modes of AI models and systems.
<!-- GEO: Global | LEVEL: International | TOPIC: Safety | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Report -->
- [International AI Safety Report](https://www.gov.uk/government/publications/international-ai-safety-report-2025) - Scientific consensus assessment of advanced AI capabilities and risks, chaired by Yoshua Bengio and backed by 30 nations.

## Security & Resilience

### International

<!-- GEO: Global | LEVEL: International | TOPIC: Security | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [OWASP GenAI Security Project](https://genai.owasp.org/) - Umbrella project for LLM and agentic AI security guidance, including the Top 10 lists and supporting cheat sheets.
<!-- GEO: Global | LEVEL: International | TOPIC: Security | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [OWASP Top 10 for LLM Applications (2026)](https://genai.owasp.org/resource/owasp-genai-llm-top-10-2026/) - Reference taxonomy of critical LLM application security risks, mapped to NIST, MITRE ATLAS, and CWE.
<!-- GEO: Global | LEVEL: International | TOPIC: Security | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Framework -->
- [OWASP Top 10 for Agentic Applications](https://genai.owasp.org/resource/owasp-top-10-for-agentic-applications/) - Agent-specific risks: goal hijacking, tool misuse, identity and privilege abuse, and memory poisoning.
<!-- GEO: Global | LEVEL: International | TOPIC: Security | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Database -->
- [MITRE ATLAS](https://atlas.mitre.org/) - ATT&CK-style knowledge base of adversarial tactics and techniques observed against machine-learning systems.

### North America

<!-- GEO: North America | LEVEL: National | TOPIC: Security | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Report -->
- [NIST AI 100-2 — Adversarial Machine Learning Taxonomy](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2023.pdf) - Formal taxonomy and shared terminology for attacks on ML systems and their mitigations.

## Agentic AI Governance

### International

<!-- GEO: Global | LEVEL: International | TOPIC: Standard | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Tool -->
- [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) - Open protocol connecting AI systems to tools and data; the specification underlying much of today's agent tooling.
<!-- GEO: Global | LEVEL: International | TOPIC: Principles | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Report -->
- [Anthropic — Building Effective Agents](https://www.anthropic.com/engineering/building-effective-agents) - Engineering guidance on agent architectures, including when *not* to build an agent.
<!-- GEO: Asia-Pacific | LEVEL: National | TOPIC: Security | STATUS: Voluntary | SECTOR: Finance | TYPE: Framework -->
- [SAFR — Safeguards for Agentic Finance at Runtime](https://www.mas.gov.sg/publications/monographs-or-information-paper/2026/safeguards-for-agentic-finance-at-runtime) - Industry white paper convened by MAS with HSBC, J.P. Morgan, Mastercard, Visa, OCBC and others: four runtime components evaluate every proposed agent action before execution and resolve it to deny, escalate, auto-execute or observe. Explicitly not supervisory expectation — and the most concrete published answer to how agent actions get authorised.
<!-- GEO: Global | LEVEL: International | TOPIC: Regulation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Database -->
- [awesome-ai-agent-governance](https://github.com/systempromptio/awesome-ai-agent-governance) - Curated list focused on governing AI agents in production: policy enforcement, audit trails, MCP security.


## Evaluation, Assurance & Red Teaming

### International

<!-- GEO: Global | LEVEL: International | TOPIC: Evaluation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Tool -->
- [HELM](https://crfm.stanford.edu/helm/) - Stanford CRFM's Holistic Evaluation of Language Models; transparent, multi-metric benchmarking.
<!-- GEO: Global | LEVEL: International | TOPIC: Evaluation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Tool -->
- [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) - De-facto standard open-source harness for few-shot LLM benchmark evaluation.
<!-- GEO: Global | LEVEL: International | TOPIC: Security | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Tool -->
- [garak](https://github.com/NVIDIA/garak) - LLM vulnerability scanner probing for prompt injection, jailbreaks, data leakage, and toxicity.
<!-- GEO: Global | LEVEL: International | TOPIC: Evaluation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Tool -->
- [promptfoo](https://github.com/promptfoo/promptfoo) - Open-source tool for testing, evaluating, and red-teaming LLM applications, with CI integration.
<!-- GEO: Global | LEVEL: International | TOPIC: Security | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Tool -->
- [PyRIT](https://github.com/Azure/PyRIT) - Microsoft's Python Risk Identification Toolkit for generative AI red teaming.
<!-- GEO: Global | LEVEL: International | TOPIC: Evaluation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Tool -->
- [Giskard](https://github.com/Giskard-AI/giskard) - Open-source testing framework for ML models and LLM applications, including scan-based vulnerability detection.

### Europe

<!-- GEO: Europe | LEVEL: National | TOPIC: Evaluation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Tool -->
- [Inspect](https://github.com/UKGovernmentBEIS/inspect_ai) - Open-source framework for large language model evaluations, built and used by the UK AI Security Institute.

### Asia-Pacific

<!-- GEO: Asia-Pacific | LEVEL: National | TOPIC: Evaluation | STATUS: Voluntary | SECTOR: Cross-sector | TYPE: Tool -->
- [AI Verify](https://aiverifyfoundation.sg/) - Singapore's testing framework and toolkit for validating AI system behaviour against governance principles.

## Transparency & Documentation

### International

<!-- GEO: Global | LEVEL: International | TOPIC: Transparency | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Report -->
- [Model Cards for Model Reporting](https://arxiv.org/abs/1810.03993) - The foundational paper (Mitchell et al.) defining standardised model documentation.
<!-- GEO: Global | LEVEL: International | TOPIC: Transparency | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Report -->
- [Datasheets for Datasets](https://arxiv.org/abs/1803.09010) - Gebru et al.'s framework for documenting dataset provenance, composition, and intended use.
<!-- GEO: Global | LEVEL: International | TOPIC: Transparency | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Tool -->
- [Hugging Face Model Card Guide](https://huggingface.co/docs/hub/model-cards) - Practical, widely adopted implementation of model cards.

### North America

<!-- GEO: North America | LEVEL: National | TOPIC: Transparency | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Report -->
- [Foundation Model Transparency Index](https://crfm.stanford.edu/fmti/) - Stanford's periodic scoring of major foundation model developers against 100 transparency indicators.

## Reports, Monitoring & Policy Trackers

### International

<!-- GEO: Global | LEVEL: International | TOPIC: Regulation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Database -->
- [OECD.AI Policy Observatory](https://oecd.ai/) - Database of national AI strategies, policies, and regulatory initiatives across 70+ jurisdictions.
<!-- GEO: Global | LEVEL: International | TOPIC: Principles | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Report -->
- [Stanford AI Index](https://aiindex.stanford.edu/) - Annual data-driven report tracking AI progress, policy, economics, and public opinion.

## Financial Services & Prudential AI Governance

The deepest vertical in this list. DORA is not an AI regulation, but it is the operational-resilience and third-party substrate that most productive AI, GenAI, and agentic workloads in EU finance actually run on — which is where AI governance, outsourcing, cybersecurity, incident management, auditability, and business continuity meet.

### European Union — Binding Law and Technical Standards

<!-- GEO: Europe | LEVEL: Regional | TOPIC: Risk Management | STATUS: Binding | SECTOR: Finance | TYPE: Law -->
- ⭐ [Digital Operational Resilience Act (DORA) — Regulation (EU) 2022/2554](https://eur-lex.europa.eu/eli/reg/2022/2554/oj/eng) - Directly applicable EU regulation on ICT risk management, incident reporting, resilience testing, and ICT third-party risk for financial entities; applicable since 17 January 2025.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Risk Management | STATUS: Binding | SECTOR: Finance | TYPE: Standard -->
- ⭐ [DORA RTS — ICT Risk Management Framework — Delegated Regulation (EU) 2024/1774](https://eur-lex.europa.eu/eli/reg_del/2024/1774/oj/eng) - Technical standards specifying the ICT risk-management tools, methods, processes, and policies DORA requires, plus the simplified framework for smaller entities.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Risk Management | STATUS: Binding | SECTOR: Finance | TYPE: Standard -->
- [DORA RTS — ICT Third-Party Contracting — Delegated Regulation (EU) 2024/1773](https://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=OJ:L_202401773) - Minimum contractual content and pre-contractual risk assessment for ICT services supporting critical or important functions; the clause-level reference for AI vendor contracts.

### Germany — BaFin

<!-- GEO: Europe | LEVEL: National | TOPIC: Regulation | STATUS: Guidance | SECTOR: Finance | TYPE: Framework -->
- ⭐ [BaFin — AI Market Surveillance in the Financial Sector](https://www.bafin.de/DE/unternehmen-maerkte/aufsicht/alle-unternehmen/ki-marktueberwachung/ki-marktueberwachung_node.html) - BaFin's role as AI Act market-surveillance authority for AI systems tied to regulated financial activity, with its stated sequencing of prohibited practices, AI literacy, and transparency duties first (German).
<!-- GEO: Europe | LEVEL: National | TOPIC: Principles | STATUS: Guidance | SECTOR: Finance | TYPE: Framework -->
- [BaFin — Principles for the Use of Algorithms in Decision-Making Processes](https://www.bafin.de/SharedDocs/Downloads/DE/Aufsichtsrecht/dl_Prinzipienpapier_BDAI.pdf?__blob=publicationFile&v=1) - Supervisory principles on governance, data quality, model risk, traceability, accountability, and customer protection for algorithmic decisions (German, PDF).
<!-- GEO: Europe | LEVEL: National | TOPIC: Risk Management | STATUS: Guidance | SECTOR: Finance | TYPE: Report -->
- [BaFin — Big Data Meets Artificial Intelligence](https://www.bafin.de/SharedDocs/Downloads/DE/dl_bdai_studie.html) - The underlying study on challenges and implications of big data and AI for the supervision and regulation of financial services (German).
<!-- GEO: Europe | LEVEL: National | TOPIC: Risk Management | STATUS: Binding | SECTOR: Finance | TYPE: Framework -->
- [BaFin — Bank Supervisory Requirements for IT (BAIT), Circular 10/2017 (BA)](https://www.bafin.de/SharedDocs/Downloads/DE/Rundschreiben/dl_rs_1710_ba_BAIT.html) - German supervisory requirements for IT governance, IT operations, information security, and IT risk management; revised with effect from 17 January 2025 to align with DORA (German).

### European Supervisory Authorities

<!-- GEO: Europe | LEVEL: Regional | TOPIC: Regulation | STATUS: Guidance | SECTOR: Finance | TYPE: Framework -->
- ⭐ [EBA — Artificial Intelligence](https://www.eba.europa.eu/publications-and-media/publications/special-topic-artificial-intelligence) - The EBA's central resource on AI in EU banking, including its monitoring of machine-learning and general-purpose AI use cases.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Risk Management | STATUS: Guidance | SECTOR: Finance | TYPE: Report -->
- [EBA — Report on Big Data and Advanced Analytics](https://www.eba.europa.eu/publications-and-media/press-releases/eba-report-identifies-key-challenges-roll-out-big-data-and) - Governance, data management, ethics, explainability, consumer protection, and operational resilience for advanced analytics in banking.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Risk Management | STATUS: Guidance | SECTOR: Finance | TYPE: Report -->
- [EBA — Discussion Paper on Machine Learning for IRB Models](https://www.eba.europa.eu/discussion-paper-machine-learning-irb-models) - Supervisory expectations for the prudent use of machine learning inside internal ratings-based credit-risk models.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Risk Management | STATUS: Guidance | SECTOR: Finance | TYPE: Report -->
- [EBA — Follow-up Report on Machine Learning for IRB Models](https://www.eba.europa.eu/publications-and-media/press-releases/eba-publishes-follow-report-use-machine-learning-internal) - Practical use cases from the consultation and the reaffirmed recommendations for ML in regulatory-capital models.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Risk Management | STATUS: Guidance | SECTOR: Finance | TYPE: Framework -->
- ⭐ [EIOPA — Opinion on AI Governance and Risk Management](https://www.eiopa.europa.eu/publications/opinion-artificial-intelligence-governance-and-risk-management_en) - Risk-based, proportionate supervisory guidance for insurers covering data governance, record keeping, fairness, cybersecurity, explainability, and human oversight.
<!-- GEO: Europe | LEVEL: Regional | TOPIC: Regulation | STATUS: Guidance | SECTOR: Finance | TYPE: Report -->
- [EIOPA — AI Systems in the Insurance Sector: Regulatory Framework Factsheet](https://www.eiopa.europa.eu/publications/factsheet-regulatory-framework-applicable-ai-systems-insurance-sector_en) - How the AI Act interacts with sectoral insurance requirements, including the high-risk life- and health-insurance use cases.

### International Financial Stability

<!-- GEO: Global | LEVEL: International | TOPIC: Risk Management | STATUS: Guidance | SECTOR: Finance | TYPE: Report -->
- ⭐ [FSB — The Financial Stability Implications of Artificial Intelligence](https://www.fsb.org/2024/11/the-financial-stability-implications-of-artificial-intelligence/) - Global assessment of systemic vulnerabilities from AI adoption: third-party concentration, market correlation, cyber risk, model risk, data quality, governance, fraud, and disinformation.
<!-- GEO: Global | LEVEL: International | TOPIC: Risk Management | STATUS: Guidance | SECTOR: Finance | TYPE: Report -->
- [BIS FSI — Executive Summary of the FSB AI Report](https://www.bis.org/fsi/fsisummaries/exsum_23904.htm) - Concise supervisory summary of the FSB's recommendations on data gaps, regulatory adequacy, and supervisory capacity.

## Sector-Specific Governance

### Healthcare

<!-- GEO: Global | LEVEL: International | TOPIC: Principles | STATUS: Guidance | SECTOR: Healthcare | TYPE: Report -->
- [WHO — Ethics and governance of AI for health: large multi-modal models](https://www.who.int/publications/i/item/9789240084759) - WHO guidance on governing LMMs in health systems, covering liability, oversight, and deployment duties.
<!-- GEO: North America | LEVEL: National | TOPIC: Regulation | STATUS: Guidance | SECTOR: Healthcare | TYPE: Framework -->
- [FDA — Artificial Intelligence in Software as a Medical Device](https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-and-machine-learning-software-medical-device) - US regulatory approach to AI/ML-based medical devices, including predetermined change control plans.

### Employment

<!-- GEO: North America | LEVEL: State/Province | TOPIC: Regulation | STATUS: Binding | SECTOR: Employment | TYPE: Law -->
- [NYC Local Law 144 — Automated Employment Decision Tools](https://www.nyc.gov/site/dca/about/automated-employment-decision-tools.page) - Binding bias-audit and candidate-notification duties for automated hiring tools; the first enforced AI audit mandate.

### Autonomous Vehicles & Robotics

<!-- GEO: Global | LEVEL: International | TOPIC: Regulation | STATUS: Binding | SECTOR: Autonomous Vehicles | TYPE: Law -->
- [UNECE Vehicle Regulations (WP.29)](https://unece.org/transport/vehicle-regulations) - International regulations covering automated driving systems, including UN R155/R156 on cybersecurity and software updates.

## Related Awesome Lists

- [awesome-public-datasets](https://github.com/awesomedata/awesome-public-datasets) - The canonical curated list of open datasets; useful for grounding governance case studies in real data.
- [awesome-production-machine-learning](https://github.com/EthicalML/awesome-production-machine-learning) - Tools for deploying, monitoring, and securing ML in production (Institute for Ethical AI).
- [awesome-llm-security](https://github.com/corca-ai/awesome-llm-security) - Papers, tools, and writeups on LLM security.

## Maintainer

Maintained by [Leon Köllerwirth Hlihel](https://github.com/leonkoellerwirth-arch), who also publishes open governance artifacts for regulated and agentic-AI environments. Listed here rather than inside the categories above, so curation and authorship stay separate.

- [agentic-ai-governance-toolkit](https://github.com/leonkoellerwirth-arch/agentic-ai-governance-toolkit) - Governance artifacts for AI agents in regulated organizations: lifecycle models, risk scoring, EU AI Act and DORA checklists, and a working evaluator. *(maintainer)*
- [rag-approval-blueprint](https://github.com/leonkoellerwirth-arch/rag-approval-blueprint) - Approval file, control catalogue with test procedures, deletion evidence, and a worked approval run for RAG systems in BaFin-regulated institutions. *(maintainer)*
- [local-agent-pipeline](https://github.com/leonkoellerwirth-arch/local-agent-pipeline) - Fully local multi-agent pipeline with a tamper-evident audit trail, action-space whitelist, and human-in-the-loop gate; a reference pattern, not a framework. *(maintainer)*

## Contributing

Contributions are welcome. Please read [contributing.md](contributing.md) before opening a pull request.
