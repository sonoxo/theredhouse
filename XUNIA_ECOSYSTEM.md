# 🔴 The Red House — XUNIA Ecosystem Layer

> **Ecosystem bio:** The Red House is XUNIA’s authorized adversarial-security and remediation layer. It turns controlled security testing into structured findings, ontology-ready relationships, prioritized risk, and reviewable fixes that can flow back into the wider XUNIA ecosystem.

## Role in XUNIA

The Red House is not a standalone identity replacement for the upstream RedAmon project. It is the **XUNIA integration layer** around the repository’s existing security capabilities.

**Primary responsibility:** authorized security validation, attack-surface mapping, finding triage, remediation orchestration, and security telemetry normalization.

### Ecosystem flow

```text
XUNIA HQ / Control Plane
        ↓
THE RED HOUSE
  ├─ authorized recon
  ├─ controlled validation
  ├─ security knowledge graph
  ├─ AI triage
  └─ remediation / GitHub PR
        ↓
Shared XUNIA Ontology
        ↓
Black House / Green House / Zyra / other approved ecosystem services
```

## Ontology contract

The Red House should expose security information as reusable ecosystem objects rather than isolated scan output.

| Object | Purpose |
|---|---|
| `Asset` | approved host, service, repository, API, container, or environment |
| `Finding` | normalized security observation or vulnerability |
| `Evidence` | reproducible proof attached to a finding |
| `Risk` | severity, exploitability, exposure, confidence, and business impact |
| `Relationship` | graph edge connecting assets, identities, findings, controls, and fixes |
| `Control` | policy or defensive measure intended to reduce a risk |
| `Remediation` | proposed or implemented fix |
| `ChangeSet` | reviewable code/configuration change such as a GitHub pull request |
| `Run` | one authorized assessment or validation execution |

## Ecosystem principles

- **Permission first:** only assets explicitly owned by or authorized for the operator belong in active testing scope.
- **Human approval at critical boundaries:** potentially disruptive actions and remediation merges remain reviewable.
- **Structured over siloed:** findings should be emitted in a form that XUNIA services can ingest, correlate, query, and audit.
- **Defensive value:** every validated finding should be able to terminate in a control, remediation, exception, or documented risk decision.
- **Portable telemetry:** logs and graph data should carry stable IDs, timestamps, source, confidence, environment, and authorization context.
- **No implicit cross-house access:** connection to another XUNIA house or service does not automatically authorize testing of that service.

## Recommended integration envelope

```json
{
  "source": "theredhouse",
  "ecosystem": "xunia",
  "domain": "security",
  "mode": "authorized-testing",
  "run_id": "<stable-run-id>",
  "asset_id": "<stable-asset-id>",
  "finding_id": "<stable-finding-id>",
  "severity": "info|low|medium|high|critical",
  "confidence": 0.0,
  "status": "observed|validated|triaged|remediating|resolved|accepted",
  "evidence": [],
  "relationships": [],
  "remediation": null,
  "timestamp": "RFC3339"
}
```

## House relationships

- **XUNIA HQ** — discovery, registry, policy, orchestration, and ecosystem navigation.
- **Black House** — broader cyber/intelligence and defensive operating context where applicable.
- **Green House / BIO workloads** — treated as protected high-sensitivity workloads; Red House may validate only explicitly authorized environments and should default to non-destructive checks.
- **Zyra / application services** — application-layer findings can be converted into repository issues, fixes, or pull requests.

## Short repository bio

**XUNIA Red House — authorized adversarial-security, security knowledge-graph, AI triage, and remediation layer for the XUNIA ecosystem.**

## Upstream attribution

This repository retains the upstream RedAmon project’s original licensing, maintainer attribution, documentation, and legal/security disclaimers. XUNIA ecosystem material describes how this fork is positioned and integrated; it does not claim authorship of upstream work.
