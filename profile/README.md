## Sixi AI

Sixi AI red-teams LLM agents and turns what it finds into evidence an auditor can use.
Domiciled in Switzerland.

Autonomous attack agents adapt to the target, chain techniques across a conversation, and send a
break again to confirm it. A finding records how often it reproduced. A technique that never
reached the target is reported as not assessed, never as passed.

### What it covers

- 46 attack agents and 318 techniques
- OWASP LLM Top 10, MITRE ATLAS, OWASP Agentic AI Threats, the EU AI Act and GDPR
- Agents reached over REST, MCP, A2A, WebSocket, or a chat widget on a web page
- Reports that map findings to EU AI Act articles, and name the articles a scan did not assess

### How it is delivered

- **The package.** One Go binary that runs in your own network, with an offline licence file beside
  it. No telemetry and no phone-home. Attacker models can run in Switzerland, the EU, or on your
  own hardware.
- **The hosted trial.** Three quick scans at [sixi.ch](https://sixi.ch), for organisations in
  Switzerland. It is there to show what a report looks like.

### Open source

- **[scan-action](https://github.com/sixi-ai/scan-action)** — a GitHub Action that red-teams an
  agent endpoint on every run and files the findings as SARIF in the Security tab. Apache-2.0.

- **[sixi-assure-rules](https://github.com/sixi-ai/sixi-assure-rules)** — the deterministic rule packs, regulatory corpus and typed-model schema behind Sixi Assure; every finding cites its clause. Apache-2.0.

- **[rbrus/sixi-scanner](https://github.com/rbrus/sixi-scanner)** — a standalone Apache-2.0 binary that red-teams an agent endpoint on your own machine. No account, no network round trip, 21 publicly documented techniques, reports as SARIF. A personal project by Radoslaw Brus and not a Sixi product, but it is the thing to reach for when the hosted service is not an option.

  It is a baseline, not a substitute: 21 techniques against the hosted library's
  coverage, and it judges with string matching rather than the full adjudication
  engine. What it does have is that it installs in one command and you can read
  every line of it.

### Early access

**Sixi Assure** — continuous, evidence-grade assurance for agentic systems, edge to cloud — is in build. Request early access at [sixi-early-access.web.app](https://sixi-early-access.web.app).

### Contact

contact@sixi.ai
