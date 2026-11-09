# Awesome Autonomous AI Recovery OPS Agent [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

> A curated directory of production-grade **Autonomous AI Recovery OPS Agents**, **Self-Healing Infrastructure Tools**, **AIOps Platforms**, and **Automated Incident Response Frameworks**.

As cloud-native architectures and microservices scale beyond human response times, autonomous operations (AIOps) and AI recovery agents have emerged to diagnose anomalies, orchestrate root cause analysis (RCA), execute remediation runbooks, and protect business continuity automatically.

---

## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [Proprietary SaaS Solutions](#proprietary-saas-solutions)
- [Open-Source AI Recovery & SRE Agents](#open-source-ai-recovery--sre-agents)
- [Autonomous Recovery Agent Architecture](#autonomous-recovery-agent-architecture)
- [Taxonomy & Classification](#taxonomy--classification)
- [Contributing](#contributing)
- [License](#license)

---

## Sector Overview & Market Dynamics

The global market for **AIOps and Autonomous IT Operations** is valued between **$17.4 billion and $21.2 billion in 2026** and is projected to expand rapidly toward **$37.8 billion to $62.0+ billion by the early 2030s**, compounding at a CAGR of approximately **15% to 22%**.

The sector exhibits **moderate fragmentation** rather than a winner-take-all dynamic:
- **Core Platform Consolidation:** A small tier of full-stack observability and cyber-resilience leaders (Datadog, Cisco/Splunk, Dynatrace, ServiceNow) controls approximately 38% of global enterprise market spend, expanding their footprint via mega-acquisitions.
- **Specialized & Agentic Fragmentation:** A large, fast-growing landscape of purpose-built autonomous remediation startups, niche incident-response engines, and cloud-native open-source agents prevents monopolistic concentration.
- **Hyperscaler Coexistence:** Native cloud provider tooling (AWS Systems Manager, Azure Monitor, Google Cloud Vertex AIOps) coexists with third-party multi-cloud agents that provide cross-cloud disaster recovery and unified telemetry control.

---

## Proprietary SaaS Solutions

The following table evaluates top enterprise SaaS platforms offering autonomous operations, AI investigation assistants, and automated recovery pipelines. Entries are **sorted in descending order by company size** (market capitalization or latest enterprise valuation).

| Platform / Vendor | Company Size (Market Cap / Valuation) | Starting Pricing (Specific Entry Tier) | Free Tier / Free Trial Limits | Autonomous / Recovery Capabilities |
| :--- | :--- | :--- | :--- | :--- |
| **[Datadog Bits AI](https://www.datadoghq.com/)** | **~$63.0B Market Cap** *(NYSE: DDOG, ~$2.6B ARR)* | **$15.00 / host / month** *(Pro Tier, annual commitment; $18.00/mo on-demand)* | **Free Forever:** Up to 5 hosts (1-day metric retention). **Trial:** 14-day free trial of full enterprise suite including Bits AI SRE without host caps. | Bits AI SRE agent executes automated incident investigations, correlates code commits with error spikes, synthesizes APM traces, and drafts remediation runbooks. |
| **[Splunk AI Assistant](https://www.splunk.com/)** *(Cisco)* | **$28.0B Valuation** *(Acquisition price by Cisco; Splunk ARR $4.2B+)* | **$15.00 / host / month** *(Splunk Observability Suite)* or **$1,800 / GB / day / year** *(Splunk Cloud ingest)* | **Trial:** 14-day free cloud trial capped at **5 GB / day ingest** (no data export). **Self-Hosted Free:** 500 MB/day indexing forever (1 user, no alerting). | AI Assistant and Event Analytics aggregate multi-source alerts, suppress alert noise by 80%+, and trigger automated webhooks and SOAR runbooks. |
| **[Rubrik Agent Cloud & Ruby AI](https://www.rubrik.com/)** | **~$18.5B Market Cap** *(NYSE: RBRK, ~$1.6B ARR)* | **$1,500.00 / year** *(Entry-level workload protection packs; enterprise contracts typically $25k+/yr)* | **Trial:** 30-day enterprise proof-of-concept (PoC) in an isolated sandbox upon sales qualification (no permanent free tier). | Ruby AI guides automated cyber recovery, assesses blast radius after ransomware attacks, detects backup anomalies, and triggers clean-room restores. |
| **[Dynatrace Davis AI](https://www.dynatrace.com/)** | **~$13.0B Market Cap** *(NYSE: DT, ~$1.5B ARR)* | **$0.01 / memory-GiB / hour** *(~$58.00/month for 8 GiB host on Full-Stack Monitoring with Davis AI)* | **Trial:** 15-day free trial of Full-Stack Monitoring with Davis AI, capped at **50 Host Units** (~800 GiB memory equivalent). | Causal AI and predictive AI engine delivers precise root-cause determination down to the code line, mapping dynamic topology and triggering automated remediation workflows. |
| **[SentinelOne Purple AI](https://www.sentinelone.com/)** | **~$8.5B Market Cap** *(NYSE: S, ~$1.0B ARR)* | **$69.99 / endpoint / year** *(Singularity Core)*; **$179.99 / endpoint / year** *(Singularity Complete w/ Purple AI)* | **Trial:** 30-day guided enterprise sandbox / proof-of-concept (PoC) with simulated attack playbooks (no self-serve free tier). | Agentic security analyst that translates natural-language incident prompts into multi-hop telemetry queries, auto-quarantines affected endpoints, and reverses unauthorized filesystem changes. |
| **[Cohesity Turing](https://www.cohesity.com/)** | **~$7.0B Valuation** *(Series H / Veritas Enterprise Data integration)* | **$50.00 / TB / month** *(Cloud Backup-as-a-Service capacity equivalent, billed annually)* | **Trial:** 30-day free trial of Cohesity Cloud Services with access to threat detection, isolated recovery sandbox, and snapshot analytics. | Integrated GenAI and ML engine for RAG-based secondary data querying, automated ransomware anomaly detection, and rapid immutable snapshot rollback. |
| **[Commvault Cloud AgentRecover](https://www.commvault.com/)** | **~$6.7B Market Cap** *(NASDAQ: CVLT, ~$1.2B ARR)* | **$1.70 / user / month** *(M365 Backup Standard)* or **$58.50 / TB / month** *(File & Object cloud workloads)* | **Trial:** 30-day free trial of Commvault Cloud SaaS workloads (up to 25 users or 1 TB evaluation quota, no credit card required). | Automated agent discovery, backup protection, and autonomous recovery for distributed endpoint AI runtimes (e.g., ChatGPT desktop, Claude Cowork) and enterprise cloud infrastructure. |
| **[Veeam Data Platform & Intelligence](https://www.veeam.com/)** | **~$5.0B Valuation** *(Insight Partners acquisition; $1.2B+ ARR)* | **$155.00 / workload / year** *(Veeam Universal License Foundation, minimum 10-pack at $1,550/yr)* | **Free Forever:** Community Edition supports up to **10 workloads/VMs** permanently. **Trial:** 30-day unrestricted trial of full Enterprise Plus platform. | Workload-level backup orchestration, instant VM restore, automated disaster recovery testing (SureBackup), and intelligent documentation/ops assistance. |
| **[PagerDuty Advance](https://www.pagerduty.com/)** | **~$2.0B Market Cap** *(NYSE: PD, ~$450M ARR)* | **$21.00 / user / month** *(Professional tier, annual commitment; $25.00/mo monthly)* | **Free Forever:** Up to **5 users**, 1 on-call schedule, 1 escalation policy, and 100 international alerts/month. **Trial:** 14-day trial of Business & Advance tier. | Generative and agentic SRE assistant providing automated incident triage, Slack/Teams ChatOps summaries, event grouping, and Runbook Automation execution. |
| **[Druva AI Resilience & Dru SRE](https://www.druva.com/)** | **~$2.0B Valuation** *(Series H; $200M+ ARR)* | **$8.00 / user / month** *(M365 SaaS protection)* or **$210.00 / TB / month** *(Server/VM cloud backup post-dedupe)* | **Trial:** 30-day free trial of Druva Data Resiliency Cloud (up to 1 TB cloud backup data or 25 SaaS seats). | Dru SRE Agent continuously monitors backup health, DruAI handles natural-language forensic investigations, and Dru MetaGraph powers cross-cloud disaster recovery orchestration. |

---

## Open-Source AI Recovery & SRE Agents

Leading open-source projects providing autonomous investigation, incident triage, and self-healing operations. **Sorted in descending order by GitHub stargazers count.**

| Project | Stars | Focus & License | Key Autonomous Capabilities |
| :--- | :--- | :--- | :--- |
| **[Keep](https://github.com/keephq/keep)** | [![GitHub stars](https://img.shields.io/github/stars/keephq/keep?style=social&color=white)](https://github.com/keephq/keep/stargazers) | **AIOps & Alert Management**<br>`Apache-2.0` | Ingests alerts across all monitoring platforms (Datadog, Grafana, CloudWatch, Sentry), deduplicates and correlates events, enriches tickets with LLMs, and executes automated multi-step recovery workflows. |
| **[K8sGPT](https://github.com/k8sgpt-ai/k8sgpt)** | [![GitHub stars](https://img.shields.io/github/stars/k8sgpt-ai/k8sgpt?style=social&color=white)](https://github.com/k8sgpt-ai/k8sgpt/stargazers) | **Kubernetes AI SRE**<br>`Apache-2.0` | Scans Kubernetes clusters to diagnose hidden failures, crashes, and misconfigurations. Translates complex cluster events into plain-English root causes and outputs remediation steps using local or cloud LLMs. |
| **[Coroot](https://github.com/coroot/coroot)** | [![GitHub stars](https://img.shields.io/github/stars/coroot/coroot?style=social&color=white)](https://github.com/coroot/coroot/stargazers) | **AI-Powered Root Cause Analysis**<br>`Apache-2.0` | Uses eBPF telemetry to map application topologies, detect network and database bottlenecks, continuously inspect service health, and deliver automated zero-config root cause analysis for distributed systems. |
| **[StackStorm](https://github.com/StackStorm/st2)** | [![GitHub stars](https://img.shields.io/github/stars/StackStorm/st2?style=social&color=white)](https://github.com/StackStorm/st2/stargazers) | **Event-Driven Auto-Remediation**<br>`Apache-2.0` | The "IFTTT for Ops" engine connecting monitoring events directly to remediation actions. Includes 160+ integration packs and 6,000+ pre-built actions to automate self-healing incident remediation loops. |
| **[HolmesGPT](https://github.com/HolmesGPT/holmesgpt)** | [![GitHub stars](https://img.shields.io/github/stars/HolmesGPT/holmesgpt?style=social&color=white)](https://github.com/HolmesGPT/holmesgpt/stargazers) | **Autonomous SRE Investigation Agent**<br>`Apache-2.0` *(CNCF Sandbox)* | Agentic loop querying live observability backends (Prometheus, Grafana, Datadog, Splunk) upon receiving Alertmanager/PagerDuty alerts. Runs tool-assisted investigations, identifies root causes, and posts findings to Jira/Slack. |
| **[Robusta](https://github.com/robusta-dev/robusta)** | [![GitHub stars](https://img.shields.io/github/stars/robusta-dev/robusta?style=social&color=white)](https://github.com/robusta-dev/robusta/stargazers) | **K8s Alert Automation & Runbooks**<br>`MIT` | Enriches Prometheus alerts with contextual cluster data (pod logs, graphs, histories), integrates AI explanations, and automates self-healing operations (e.g., auto-restart, pod evictions, scaling). |
| **[Botkube](https://github.com/kubeshop/botkube)** | [![GitHub stars](https://img.shields.io/github/stars/kubeshop/botkube?style=social&color=white)](https://github.com/kubeshop/botkube/stargazers) | **Kubernetes Collaborative ChatOps**<br>`MIT` | Bi-directional communication agent that monitors cluster events, provides AI-driven debugging recommendations directly in Slack/Teams/Discord, and safely executes verified triage commands. |

---

## Autonomous Recovery Agent Architecture

A standard autonomous recovery agent loop consists of five operational phases:

```
+-----------------------------------------------------------------------------------+
|                        1. TELEMETRY & ALERT INGESTION                             |
|          (Metrics, Distributed Traces, Syslogs, eBPF Events, Webhooks)           |
+------------------------------------------+----------------------------------------+
                                           |
                                           v
+-----------------------------------------------------------------------------------+
|                     2. CONTEXTUAL NOISE REDUCTION & TOPOLOGY                      |
|       (Dynamic Service Graph, Alert Deduplication, Anomaly Correlation)           |
+------------------------------------------+----------------------------------------+
                                           |
                                           v
+-----------------------------------------------------------------------------------+
|               3. AI INVESTIGATION & ROOT CAUSE ANALYSIS (RCA)                     |
|  (Agentic LLM Tool Calling: Log Dumps, Diff Commits, Profiling & Vector Memory)   |
+------------------------------------------+----------------------------------------+
                                           |
                                           v
+-----------------------------------------------------------------------------------+
|                 4. REMEDIATION POLICY & HUMAN-IN-THE-LOOP (HITL)                  |
|    (Rule Verification, Guardrails, Canary Validation, Approval Webhook / ChatOps)  |
+------------------------------------------+----------------------------------------+
                                           |
                                           v
+-----------------------------------------------------------------------------------+
|                    5. AUTONOMOUS RECOVERY EXECUTION & VERIFICATION                |
|    (Snapshot Rollback, Traffic Rerouting, Pod Restart, Runbook Action, Post-Mortem)|
+-----------------------------------------------------------------------------------+
```

1. **Ingest:** Streams raw telemetry from OpenTelemetry collectors, Prometheus alerts, and APM tools.
2. **Contextualize:** Reconstructs service dependency graphs to localize the disturbance.
3. **Diagnose:** An autonomous agent uses LLM tool-calling (querying logs, git diffs, pod metrics) to isolate root causes.
4. **Safeguard:** Evaluates safety policies, rate limits, and permission boundaries before initiating destructive changes.
5. **Recover & Verify:** Executes remediation actions (e.g., snapshot rollback, autoscaling, container restart) and verifies that SLOs recover to baseline.

---

## Taxonomy & Classification

| Category | Typical Scope | Representative Tools |
| :--- | :--- | :--- |
| **Root Cause Investigation (RCA)** | Read-only diagnostic agents that investigate alerts and publish structured explanations. | HolmesGPT, K8sGPT, Coroot, Datadog Bits AI |
| **Event Correlation & Alert AIOps** | Multi-source event ingestion engines that de-duplicate alerts and correlate signals. | Keep, PagerDuty Advance, Splunk AI |
| **Self-Healing Runbook Execution** | Event-driven engines that execute pre-defined or dynamically selected operational scripts. | StackStorm, Robusta |
| **Cyber Resilience & Disaster Recovery** | Snapshot validation, clean-room restoration, and ransomware recovery orchestration. | Rubrik Ruby AI, Druva Dru SRE, Cohesity Turing, Veeam |

---

## Contributing

Contributions are very welcome! If you know of an open-source tool, agentic framework, or enterprise platform that fits this list:

1. Fork this repository.
2. Create a new branch: `git checkout -b add-my-tool`.
3. Add your tool with objective facts, specific pricing/limits, or star count badges.
4. Open a pull request!

---

## License

This repository and its documentation are open-sourced under the [Apache 2.0 License](LICENSE).
