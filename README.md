<p align="center">
  <img src="docs/assets/logo.png" alt="RedAmon / The Red House" width="120"/>
</p>

<h1 align="center">🔴 THE RED HOUSE</h1>
<p align="center"><strong>XUNIA Authorized Security • Knowledge Graph • AI Triage • Remediation</strong></p>

<p align="center">
  The Red House is XUNIA’s authorized adversarial-security and remediation layer. It converts controlled security testing into structured findings, ontology-ready relationships, prioritized risk, evidence, and reviewable fixes that can flow back into the wider XUNIA ecosystem.
</p>

<p align="center">
  <a href="XUNIA_ECOSYSTEM.md"><b>XUNIA Ecosystem Guide</b></a> ·
  <a href=".xunia/ecosystem.json"><b>Ecosystem Manifest</b></a> ·
  <a href="UPSTREAM_REDAMON_README.md"><b>Full RedAmon Documentation</b></a> ·
  <a href="SECURITY.md"><b>Security Policy</b></a>
</p>

> **AUTHORIZED USE ONLY:** The Red House is for systems you own or have explicit written authorization to assess. Cross-house membership, repository access, or ecosystem affiliation does not create authorization to test an external target.

---

## XUNIA ecosystem role

```text
XUNIA HQ / CONTROL PLANE
          ↓
   🔴 THE RED HOUSE
   ├─ authorized reconnaissance
   ├─ controlled validation
   ├─ security knowledge graph
   ├─ AI finding triage
   ├─ risk normalization
   └─ remediation / reviewable PRs
          ↓
   SHARED XUNIA ONTOLOGY
          ↓
BLACK HOUSE • GREEN HOUSE / BIO • ZYRA • APPROVED SERVICES
```

The Red House wraps the upstream **RedAmon** security framework with a XUNIA integration contract. The underlying project provides containerized reconnaissance, security validation, Neo4j attack-surface graphs, AI-assisted triage, and remediation workflows. The XUNIA layer adds ecosystem identity, ontology bindings, cross-house boundaries, and machine-readable integration metadata.

### Core ecosystem objects

| Object | Role |
|---|---|
| `Asset` | Approved host, service, repository, API, container, or environment |
| `Finding` | Normalized security observation or vulnerability |
| `Evidence` | Reproducible evidence attached to a finding |
| `Risk` | Severity, exploitability, exposure, confidence, and impact |
| `Relationship` | Graph edge linking assets, identities, findings, controls, and fixes |
| `Control` | Defensive policy or technical safeguard |
| `Remediation` | Proposed or implemented fix |
| `ChangeSet` | Reviewable code/configuration mutation |
| `Run` | Auditable execution record |

**BIO / Green House boundary:** biotechnology, health, pharma, research, or similarly sensitive workloads are treated as high-sensitivity and **non-destructive by default**. External activity requires explicit scope and authorization.

---

## Maintainers & ecosystem stewards

<table>
<tr>
<td align="center" valign="top" width="33.33%">
<img src="docs/assets/samuele.png" alt="Samuele Giampieri" width="120"/><br/>
<b>Samuele Giampieri</b><br/>
Upstream Creator, Maintainer & AI Platform Architect<br/><br/>
<small>AI platform architect and full-stack lead behind RedAmon, with production experience across agentic AI, ML, cloud systems, and security automation.</small><br/><br/>
<a href="https://www.linkedin.com/in/samuele-giampieri-b1b67597/">LinkedIn</a> · <a href="https://github.com/samugit83">GitHub</a> · <a href="https://www.devergolabs.com/">Devergo Labs</a>
</td>
<td align="center" valign="top" width="33.33%">
<img src="docs/assets/ritesh.png" alt="Ritesh Gohil" width="120"/><br/>
<b>Ritesh Gohil</b><br/>
Upstream Maintainer & Lead Security Researcher<br/><br/>
<small>Security engineer and researcher with experience across Web, API, Mobile, Network, and Cloud penetration testing, CVE research, and security architecture.</small><br/><br/>
<a href="https://www.linkedin.com/in/riteshgohil25/">LinkedIn</a> · <a href="https://github.com/L4stPL4Y3R">GitHub</a>
</td>
<td align="center" valign="top" width="33.33%">
<img src="https://github.com/sonoxo.png?size=240" alt="Douglas Brown" width="120"/><br/>
<b>Douglas Brown</b><br/>
XUNIA Ecosystem Maintainer & AI/Security Systems Builder<br/><br/>
<small>Maintainer of the XUNIA / ZYRA integration layer, focused on governed agentic systems, security architecture, ontology-driven workflows, AI application development, and auditable human-controlled execution. ZYRA currently records a reconciled 34-record credential, training, and professional-development ledger with evidence tiered by issuer verification and supplied provenance.</small><br/><br/>
<b>Selected credential evidence</b><br/>
<small>Palantir Foundry Aware · Introduction to Foundry & AIP for Enterprise Organizations · Deep Dive: Data Protection Tools in Foundry · Palantir Data Science Fundamentals · Google Cybersecurity Professional Certificate · Google AI Professional Certificate · IBM Quantum Machine Learning · Red Hat System Administration I training · Foundations of Business Intelligence.</small><br/><br/>
<a href="https://www.linkedin.com/in/douglasbrownjr/">LinkedIn</a> · <a href="https://github.com/sonoxo">GitHub</a> · <a href="https://github.com/sonoxo/zyra">ZYRA</a><br/>
<a href="https://github.com/sonoxo/zyra/blob/main/ZYRA.README.md"><b>Credential ledger</b></a>
</td>
</tr>
</table>

> **Attribution boundary:** Samuele Giampieri and Ritesh Gohil are identified here for their upstream RedAmon roles. Douglas Brown’s maintainer role applies to the **sonoxo/theredhouse XUNIA integration/fork** and does not imply maintainer status in the upstream `samugit83/redamon` project.

---

## Upstream platform

The Red House is built around the open-source **RedAmon** framework. To keep the complete technical documentation, architecture, installation instructions, tool matrix, security model, community information, and original maintainer material intact, the previous README is preserved verbatim here:

### 📘 [Open the complete upstream RedAmon README →](UPSTREAM_REDAMON_README.md)

Upstream project: [samugit83/redamon](https://github.com/samugit83/redamon)  
Upstream website: [redamon.org](https://www.redamon.org/)

---

## XUNIA integration contract

The machine-readable integration contract lives at [`.xunia/ecosystem.json`](.xunia/ecosystem.json). Current Red House capabilities include:

- authorized reconnaissance and controlled security validation;
- security knowledge-graph generation;
- finding triage and risk normalization;
- remediation orchestration and reviewable GitHub PR flows;
- security telemetry export into approved XUNIA ontology consumers;
- explicit authorization context and human review for disruptive actions;
- no implicit cross-house authorization.

See [`XUNIA_ECOSYSTEM.md`](XUNIA_ECOSYSTEM.md) for the human-readable architecture and operating boundaries.

---

## Repository map

| Resource | Purpose |
|---|---|
| [`XUNIA_ECOSYSTEM.md`](XUNIA_ECOSYSTEM.md) | Red House role inside the ecosystem |
| [`.xunia/ecosystem.json`](.xunia/ecosystem.json) | Machine-readable ecosystem identity and ontology contract |
| [`UPSTREAM_REDAMON_README.md`](UPSTREAM_REDAMON_README.md) | Preserved complete upstream-facing README |
| [`SECURITY.md`](SECURITY.md) | Security policy |
| [`DISCLAIMER.md`](DISCLAIMER.md) | Authorized-use and legal boundaries |
| [`LICENSE`](LICENSE) | Repository license |
| [`THIRD-PARTY-LICENSES.md`](THIRD-PARTY-LICENSES.md) | Third-party licensing inventory |
| [`ZYRA credential ledger`](https://github.com/sonoxo/zyra/blob/main/ZYRA.README.md) | Douglas Brown credential/provenance evidence used by this fork |

---

<p align="center"><strong>🔴 RED HOUSE // XUNIA</strong><br/>Authorized security in. Structured evidence out. Human control at consequential boundaries.</p>
