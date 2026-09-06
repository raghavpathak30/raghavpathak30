# Raghav Pathak

### Applied Cryptography & Security Engineering · LNMIIT '27 · Cybersecurity Intern, Omni Infoword

[Email](mailto:23ucs685@lnmiit.ac.in) · [LinkedIn](https://linkedin.com/in/<your-handle>)

I build systems that compute on data they aren't allowed to see, and tooling that decides which vulnerabilities are actually worth fixing. Currently working on homomorphic-encryption inference with faculty at LNMIIT, and on LLM-assisted security tooling.

---

## Experience

**Omni Infoword Pvt. Ltd.** · Cybersecurity Intern · May–Jul 2026 (~7 weeks)
SOC alert triage across Splunk, Microsoft Sentinel, QRadar and Elastic — suspicious-login investigation, phishing analysis, EDR policy management. Second half on application security: OWASP Top 10 testing of pre-release software, including exposed staging endpoints and sensitive files reported to the dev team.

**LNMIIT** · Undergraduate Researcher · 2025–present
Encrypted-inference and transciphering research with Prof. Debranjan Pal. Paper in preparation.

---

## Highlights

|  |  |
|---|---|
| **Grand Finalist** | PSB CyberShield 2026 — national hackathon, finale at IIT Hyderabad |
| **HTB Academy** | Skilled rank · working the Bug Bounty Hunter path |
| **Certification** | Google Cybersecurity Professional Certificate |

---

## Projects

- **[PPFDaaS](https://github.com/raghavpathak30/PPFDaaS)** — Fraud-detection inference over encrypted transactions. CKKS via Microsoft SEAL 4.1.2, C++17 gRPC server, Python client. The vendor never holds a secret key. Transciphering arm cuts client upload **249×** by shipping a symmetric ciphertext evaluated homomorphically server-side. Digest-pinned containers, cosign signatures, SBOMs.

- **[SetuGuard](https://github.com/raghavpathak30/SetuGuard)** — Android malware triage joined to mule-account detection. Static APK analysis → RAG reporting → YARA generation, plus a gradient-boosted account scorer linked on certificate-hash indicators. Measured **AUC 0.14** against a never-tuned-against corpus of real banking apps — the scorer ranks legitimate banks above malware, because both classes request the same permissions by construction. Documented rather than hidden.

- **[reachability-triage](https://github.com/raghavpathak30/reachability-triage)** — Ingests OSV/GHSA advisories and determines whether a CVE is genuinely reachable from a given codebase. Python, FastAPI, PostgreSQL, Docker, GitHub Actions. In development.

- **[PwnBot](https://github.com/raghavpathak30/PwnBot)** — LLM pentest assistant over the Groq API. Structured tool-output parsing and a scope guard that refuses targets outside the declared engagement.

---

## Notes

Every headline number in these repositories traces to a committed artifact file. Where a measurement turned out to be invalid — wrong parameter set, contaminated corpus, unreproducible host — the correction sits next to the original instead of replacing it. `MEASUREMENT_PROVENANCE.md` in PPFDaaS is the clearest example.

**Working with:** C++17, Python, Go, Docker, Microsoft SEAL, gRPC, FastAPI, PostgreSQL, GitHub Actions, Linux.

<!--
**raghavpathak30/raghavpathak30** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
