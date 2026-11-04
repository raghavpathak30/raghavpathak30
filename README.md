# Raghav Pathak

**Backend and AI engineering, with a security background.** Final-year CSE at LNMIIT Jaipur, graduating 2027.

I build systems that are honest about what they don't know: an agent that answers *unknown* instead of guessing whether a CVE is reachable, a RAG pipeline that can only cite what it actually retrieved, and encrypted inference where the server never sees the data it scores.

[raghavpathak.me](https://raghavpathak.me) &nbsp;·&nbsp; [LinkedIn](https://linkedin.com/in/raghav-pathak-b14b46282) &nbsp;·&nbsp; [Email](mailto:raghavpathak0130@gmail.com)

---

### Now

- **Software Engineering Intern (AI & Automation), MarkeTreasure.** Auditing a rule-based equity screener (~12,000 stocks, ~30 years of daily OHLCV). 70+ defects catalogued so far; an independent review verified 61 of 68 audit claims and found none wrong.
- **Undergraduate researcher, LNMIIT.** Comparing CKKS homomorphic-encryption inference against HERA and Rubato transciphering for fraud scoring on encrypted data, with Prof. Debranjan Pal. Paper in preparation.
- **Building [reachability-triage](https://github.com/raghavpathak30/reachability-triage).** Releases are gated on hand-labelled evals.

---

### Selected work

**[reachability-triage](https://github.com/raghavpathak30/reachability-triage)**: is this CVE actually reachable from my code?
An AST call graph feeds a LangGraph tool-calling agent, which returns a verdict with evidence, or *unknown* when the evidence isn't there. Jobs run on PostgreSQL, and the React + TypeScript frontend uses an API client generated from the OpenAPI schema, so backend contract changes fail CI.
→ 30 hand-labelled eval fixtures · 30 of 30 real-model runs with zero confident wrong verdicts
`Python` `FastAPI` `PostgreSQL` `LangGraph` `React` `TypeScript` `Docker`

**[PPFDaaS](https://github.com/raghavpathak30/PPFDaaS)**: fraud-detection inference over encrypted transactions.
CKKS via Microsoft SEAL 4.1.2, a C++17 gRPC server and a Python client. The vendor never holds a secret key. The transciphering arm ships a symmetric ciphertext that the server evaluates homomorphically.
→ 249× smaller client upload · digest-pinned containers, cosign signatures, SBOMs
`C++17` `Microsoft SEAL` `gRPC` `Python` `Docker`

**[SetuGuard](https://github.com/raghavpathak30/SetuGuard)**: Android malware triage, Grand Finalist at PSB CyberShield 2026 (IIT Hyderabad).
Static APK analysis feeds a RAG pipeline in which a local Mistral 7B emits a schema-constrained report. Citations are restricted to valid chunk IDs and pass through a grounding gate, and YARA rules are generated from the findings.
→ zero failures across 7 hostile-input cases · scoring endpoint 11× faster, peak memory 2.9× lower
`Python` `FAISS` `Mistral 7B`

**[Dispute Desk](https://github.com/raghavpathak30/razorpay-disputedesk)**: LLM chargeback-evidence responder, Razorpay AI Buildathon 2026.
Takes a payment chargeback, assembles evidence from transaction context, and drafts the dispute response. Built solo in 5 days.
`Python` `LLM APIs`

**PwnBot**: LLM pentest assistant over the Groq API, with structured tool-output parsing and a scope guard that refuses targets outside the declared engagement.

---

### How I report numbers

Every headline number in these repositories traces to a committed artifact file. When a measurement turned out to be invalid (wrong parameter set, contaminated corpus, unreproducible host), the correction sits next to the original instead of replacing it. [`MEASUREMENT_PROVENANCE.md`](https://github.com/raghavpathak30/PPFDaaS) in PPFDaaS is the clearest example.

---

### Experience

**MarkeTreasure Investment LLC** · Software Engineering Intern (AI & Automation) · Sep 2026 – present · remote
**Omni Infoword** · Cybersecurity Intern · May – Jul 2026 (7 weeks): SOC alert triage across Splunk, Microsoft Sentinel, QRadar and Elastic, then an OWASP Top 10 test pass on pre-release software
**LNMIIT** · Undergraduate Researcher · 2025 – present

Also: Hack The Box Academy, Skilled rank · Google Cybersecurity Professional Certificate · Head of Sponsorship, Vivacity

---

### Stack

**Languages** Python · TypeScript · C++17 · Go · SQL · Bash
**Backend** FastAPI · PostgreSQL · SQLAlchemy · Alembic · gRPC · React
**AI** LangGraph · tool calling · RAG (FAISS) · structured output · evals
**Security & crypto** Microsoft SEAL (CKKS) · OWASP testing · Splunk · YARA
**Infra** Docker · GitHub Actions · Linux · cosign · SBOMs
