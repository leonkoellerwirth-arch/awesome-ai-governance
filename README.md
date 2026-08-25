# Awesome AI Governance [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of regulations, standards, risk frameworks, security resources, and open-source tools for governing AI systems — with a focus on agentic AI in regulated environments.

**NOTICE:** This list is curated, not exhaustive. Entries are grouped by topic and then by region, because a single document is often several things at once — the EU AI Act is regulation, transparency, and risk management in one. Every entry in the topical sections additionally carries a machine-readable tag comment in the source (`GEO`, `LEVEL`, `TOPIC`, `STATUS`, `SECTOR`, `TYPE`); the fields are documented in `contributing.md`. "Europe" is not "EU": the European Union is a supranational legal order, while the Council of Europe covers 46 states and works from a human-rights basis. Vendor marketing content is out of scope.

## Contents

- [Regulations & Law](#regulations--law)
- [Standards & Technical Specifications](#standards--technical-specifications)
- [Principles, Frameworks & Strategies](#principles-frameworks--strategies)
- [Risk, Safety & Incidents](#risk-safety--incidents)
- [Security & Resilience](#security--resilience)
- [Agentic AI Governance](#agentic-ai-governance)
- [Evaluation, Assurance & Red Teaming](#evaluation-assurance--red-teaming)
- [Transparency & Documentation](#transparency--documentation)
- [Reports, Monitoring & Policy Trackers](#reports-monitoring--policy-trackers)
- [Sector-Specific Governance](#sector-specific-governance)
- [Related Awesome Lists](#related-awesome-lists)

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
<!-- GEO: Global | LEVEL: International | TOPIC: Regulation | STATUS: Guidance | SECTOR: Cross-sector | TYPE: Database -->
- [awesome-ai-agent-governance](https://github.com/systempromptio/awesome-ai-agent-governance) - Curated list focused on governing AI agents in production: policy enforcement, audit trails, MCP security.

<!--
  MAINTAINER ENTRIES — pending. The two placeholder entries that were here pointed at
  repositories that do not exist yet (governance-mcp, ai-governance-decision-kit).
  They were removed rather than shipped as dead links. Candidates to add once decided:
    - https://github.com/leonkoellerwirth-arch/agentic-ai-governance-toolkit
    - https://github.com/leonkoellerwirth-arch/local-agent-pipeline
    - https://github.com/leonkoellerwirth-arch/rag-approval-blueprint
  Mark any self-maintained entry with *(maintainer)* per contributing.md.
-->

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

## Sector-Specific Governance

### Healthcare

<!-- GEO: Global | LEVEL: International | TOPIC: Principles | STATUS: Guidance | SECTOR: Healthcare | TYPE: Report -->
- [WHO — Ethics and governance of AI for health: large multi-modal models](https://www.who.int/publications/i/item/9789240084759) - WHO guidance on governing LMMs in health systems, covering liability, oversight, and deployment duties.
<!-- GEO: North America | LEVEL: National | TOPIC: Regulation | STATUS: Guidance | SECTOR: Healthcare | TYPE: Framework -->
- [FDA — Artificial Intelligence in Software as a Medical Device](https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-and-machine-learning-software-medical-device) - US regulatory approach to AI/ML-based medical devices, including predetermined change control plans.

### Finance

<!-- GEO: Global | LEVEL: International | TOPIC: Risk Management | STATUS: Guidance | SECTOR: Finance | TYPE: Report -->
- [FSB — The Financial Stability Implications of Artificial Intelligence](https://www.fsb.org/2024/11/the-financial-stability-implications-of-artificial-intelligence/) - Financial Stability Board analysis of systemic risk channels created by AI adoption in finance.

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

## Contributing

Contributions are welcome. Please read [contributing.md](contributing.md) before opening a pull request.
