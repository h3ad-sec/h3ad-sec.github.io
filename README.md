# H3AD-SEC

**SOC Analyst & Detection Engineering Portfolio Platform**

H3AD-SEC is a modular portfolio platform built by a SOC analyst and detection engineer. It hosts a growing suite of tools covering threat intelligence, detection engineering, threat hunting, and SOC operations — all accessible from the browser, no installation required.

Live at: [h3ad-sec.github.io](https://h3ad-sec.github.io)

---

## Modules

### [H3AD-X](https://h3ad-sec.github.io/H3AD-X/) — Threat Intelligence
IOC enrichment, artifact extraction, and infrastructure mapping.

| Tool | Description |
|------|-------------|
| [VERDIKT](https://h3ad-sec.github.io/VERDIKT/) | Bulk IOC checker — 6 TI sources, BYOK + managed mode |
| [X-VERDIKT](https://h3ad-sec.github.io/X-VERDIKT/) | Deep IP enrichment — 10+ sources, IP Intel mode |
| [PARSE-X](https://h3ad-sec.github.io/PARSE-X/) | Artifact extractor from raw text — 18 types, client-side |
| [DNSCOPE](https://h3ad-sec.github.io/DNSCOPE/) | Domain/IP infrastructure mapper — ASN, PDNS, certs, CDN/WAF |
| [MAILSCOPE](https://h3ad-sec.github.io/MAILSCOPE/) | Email header analyzer — SPF/DKIM/DMARC, hop chain, spoofing detection |

### [H3AD-AI](https://h3ad-sec.github.io/H3AD-AI/) — AI-Assisted Security
AI-augmented analyst workflows for runbook generation, query building, and ATT&CK mapping.

| Tool | Description |
|------|-------------|
| [INSIGHT-AI](https://h3ad-sec.github.io/INSIGHT-AI/) | AI runbook generator — L3/SME persona, 10-section incident playbooks |
| [QUERYCRAFT-AI](https://h3ad-sec.github.io/QUERYCRAFT-AI/) | AI query builder — KQL, Sigma, XQL from natural language |
| [FPLENS-AI](https://h3ad-sec.github.io/FPLENS-AI/) | False positive analyzer — likelihood scoring with analyst justification |
| [ATTMAP-AI](https://h3ad-sec.github.io/ATTMAP-AI/) | ATT&CK mapper — technique identification from alert/log context |
| [CHRONO-AI](https://h3ad-sec.github.io/CHRONO-AI/) | Timeline builder — structured event chronology from raw investigation notes |
| [MALBRIEF-AI](https://h3ad-sec.github.io/MALBRIEF-AI/) | Malware behavior analyzer — classification, TTPs, detection signatures |
| [PROMPTVAULT](https://h3ad-sec.github.io/PROMPTVAULT/) | AI prompt library — curated SOC/detection/threat hunting prompts by category |

### [H3AD-DETECT](https://h3ad-sec.github.io/H3AD-DETECT/) — Detection Engineering
Detection query libraries mapped to MITRE ATT&CK.

| Tool | Description |
|------|-------------|
| [TRACERULES](https://h3ad-sec.github.io/TRACERULES/) | Detection query arsenal — KQL, Sigma, XQL |

### [H3AD-HUNT](https://h3ad-sec.github.io/H3AD-HUNT/) — Threat Hunting
Hypothesis generation and investigation pivot tooling.

| Tool | Description |
|------|-------------|
| [HYPOS](https://h3ad-sec.github.io/HYPOS/) | ATT&CK-based hypothesis platform with curated hunting packs |
| [PIVEX](https://h3ad-sec.github.io/PIVEX/) | Interactive pivot graph — 36 artifact types, 168+ pivot relationships |
| [TRACEPULSE](https://h3ad-sec.github.io/TRACEPULSE/) | Threat-specific query packs tied to campaigns and CVEs |

### [H3AD-OPS](https://h3ad-sec.github.io/H3AD-OPS/) — SOC Operations
Day-to-day analyst workflow tooling.

| Tool | Description |
|------|-------------|
| [QUICKTRACE](https://h3ad-sec.github.io/QUICKTRACE/) | Daily workflow queries — AUTH, NETWORK, ENDPOINT, CLOUD |
| [SHIFTLOG](https://h3ad-sec.github.io/SHIFTLOG/) | Shift handover report generator — structured 6-section form |
| [PHISHOPS](https://h3ad-sec.github.io/PHISHOPS/) | Phishing investigation tracker — 7-step workflow, live IOC aggregator |

### [H3AD-DF](https://h3ad-sec.github.io/H3AD-DF/) — Digital Forensics
Artifact analysis and forensic triage tooling.

| Tool | Description |
|------|-------------|
| [REGSCOPE](https://h3ad-sec.github.io/REGSCOPE/) | Registry artifact analyzer — persistence detection, ATT&CK mapping |
| [MALBRIEF-AI](https://h3ad-sec.github.io/MALBRIEF-AI/) | Malware behavior analyzer — also listed under H3AD-AI |

### [H3AD-IR](https://h3ad-sec.github.io/H3AD-IR/) — Incident Response
Structured IR playbooks and workflow tooling. No tools live yet.

### [H3AD-LEARN](https://h3ad-sec.github.io/H3AD-LEARN/) — Security Training
Modular browser-native security training for SOC analysts and detection engineers.

| Module | Status | Chapters |
|--------|--------|----------|
| Threat Hunting | Live | 9 chapters — PEAK, TaHiTI, Admiralty, KQL/Sigma, advanced techniques |
| LOLBAS | Live | 8 chapters — certutil, mshta, regsvr32, tradecraft, detection queries, APT campaigns |

---

## Design Principles

- Browser-first — most tools are static GitHub Pages with no build step
- No data retention — enrichment tools either run client-side or proxy through serverless functions without logging
- MITRE ATT&CK aligned — detection and hunting tools map to tactics and techniques
- Dark / light theme across all tools
- Fully responsive — all tools work across mobile, tablet, and desktop (320px to 2560px)
- Accessible — keyboard navigation, ARIA labels, focus-visible rings, colorblind-safe status system (cyan/amber/gray)

---

## Stack

- HTML / CSS / Vanilla JS — no framework dependency
- GitHub Pages (static hosting)
- Vercel serverless functions (backend proxies for managed-mode tools)
