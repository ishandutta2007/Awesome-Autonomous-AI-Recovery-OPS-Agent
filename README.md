# Awesome-Autonomous-AI-Recovery-OPS-Agent

I can't create the file, commit, or push—I have no filesystem, no shell, and no Git credentials. Everything I produce is text. You will need to save and push it yourself.

I also have to flag what the search results actually support, because **most entries in your list have no usable pricing**, and the open-source side has exactly one strong project.

## The data problems

**Druva's AI Agent is not a single product—it is a platform-wide capability.** Druva's "AI Resilience" pillar includes Dru SRE Agent (continuous backup reliability), DruAI (natural-language investigation), and Dru MetaGraph (graph intelligence) . **No standalone pricing for the AI agent surfaced**; it is part of the Druva platform, which uses consumption-based pricing.

**Veeam Intelligence is a documentation chatbot, not a recovery ops agent.** It answers product questions from Veeam docs, is limited to **200 questions per 24 hours per license**, and **requires a paid license or Evaluation license**—not available on Community Edition . Advanced Mode (infrastructure-aware) requires **Veeam Data Platform Advanced/Premium or Enterprise Plus** . **Do not present it as an autonomous recovery agent.**

**Cohesity Turing is a support chatbot, not a recovery ops agent.** The blog describes it as an "AI-driven Support Experience" that acts as a virtual SRE for troubleshooting . **No pricing surfaced.** The Computer Weekly article describes Turing as a broader AI toolset for backup and ransomware, but still not a recovery orchestration agent .

**Rubrik Ruby AI is an optional feature of Security Cloud with no list price.** Licenseware confirms Rubrik AI (formerly "Ruby") is an optional feature for threat investigations, **not enabled by default**, **excluded from the SLA**, and provided "as is" . Rubrik Agent Cloud uses a **platform fee plus annual token allotment** . **No dollar figures surfaced.**

**Commvault's AI is AgentRecover for laptop agent configurations.** It discovers and protects agent configurations (Claude Cowork, ChatGPT desktop) on managed devices, and recovers them after disruption . **It is not a recovery ops agent for infrastructure**—it is endpoint agent data protection.

**Datadog Bits AI pricing did not surface.** The Korean pricing page returned fragments about APM and Data Streams Monitoring, not Bits AI .

**Dynatrace Davis AI is priced per host-hour.** The AIOps guide lists **from ~$0.08/host/hour** for full-stack monitoring, with **Davis AI included** for anomaly detection and root cause . Annual recurring revenue exceeds **$1.5B** .

**Splunk AI Assistant has no separate line-item price.** It is **included with Splunk Cloud Platform or Enterprise subscriptions**, but the base subscription is the real cost: **first-year total $80.5K–$203.2K** (base $126.5K), **three-year $174.8K–$406.3K** . **Do not present the AI assistant as free—the platform is the cost.**

**New Relic AI (formerly Grok) has no separate AI pricing.** It is included with New Relic seats under Standard, Pro, and Enterprise tiers, with a free tier covering **100 GB/month** . Cost estimates mirror Splunk's: **$80.5K–$203.2K first year** .

**SentinelOne Purple AI is $41.99 per endpoint** per CDW listing . This is a subscription license for the AI assistant add-on, not the full EDR platform.

## Open-source: what actually exists

**HolmesGPT** is the only genuine open-source AI recovery/ops agent surfaced: **Apache 2.0, CNCF sandbox project**, originally by Robusta.Dev with major contributions from Microsoft . It is an **agentic loop that queries live observability data** (Prometheus, Grafana, Datadog, Kubernetes, Splunk, New Relic, and many more) to identify root causes. It fetches alerts from AlertManager, PagerDuty, OpsGenie, or Jira, and **writes findings back** . It supports any LLM provider and runs in **operator mode** for scheduled investigations .

**HolmesGPT is an investigation agent, not a recovery agent.** It does not execute recovery actions—it diagnoses root causes and writes findings. **Do not present it as a replacement for Druva's recovery automation or Rubrik's autonomous recovery.**

**No star count surfaced for HolmesGPT.** Do not invent one.

## What I recommend

**Split into three honest categories:**

**1. AI-Powered Recovery & Resilience Platforms** (proprietary, mostly quote-only):
- **Druva** — Dru SRE Agent + DruAI + Dru MetaGraph; platform pricing 
- **Rubrik** — Ruby AI optional, excluded from SLA; Agent Cloud token-based 
- **Commvault** — AgentRecover for laptop agent configs, not infra recovery 

**2. AI Observability Assistants** (proprietary, included with platform):
- **Dynatrace Davis AI** — from ~$0.08/host/hour 
- **Splunk AI Assistant** — included with Splunk; $80.5K–$203.2K first year 
- **New Relic AI** — included with seats; $80.5K–$203.2K first year 
- **SentinelOne Purple AI** — $41.99/endpoint 
- **Veeam Intelligence** — 200 questions/24h, paid license required 
- **Cohesity Turing** — support chatbot, no pricing 

**3. Open-Source**:
- **HolmesGPT** — Apache 2.0, CNCF sandbox, root cause investigation, not recovery execution 

**Do not present Veeam Intelligence or Cohesity Turing as recovery ops agents**—they are chatbots. **Do not present Splunk/New Relic AI as free**—the platform subscription is the cost.

If you paste your current `README.md` and confirm you want this framing, I will produce the complete file as text for you to save. I will not fabricate Druva or Rubrik AI pricing, present Veeam's documentation chatbot as an autonomous agent, or claim HolmesGPT executes recovery.
