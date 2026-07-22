---
title: "FCAJ Community Day (Data Driven, AI Risen)"
date: 2026-06-27
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---



### Event Objectives

- Explore automated cloud operations systems and the architecture of the Deep Response Engine.
- Learn about Voice Agents and how to build natural, human-like AI conversations at scale.
- Understand the capabilities of AWS DevOps Agent and multi-agent reasoning for IT operations.
- Analyze AI-powered workforce planning and data-driven insights using Amazon Quick.
- Review security integrations and configuring private VPC connections using MCP (Model Context Protocol).

### Speakers

- **Truong Tran** - AI Solution Sales, Noventiq
- **Steve Tran** - CTO/Founder, CloudThinker
- **Trung Vu** - CEO, Revve AI
- **Anh Dang** - Solution Sales, Noventiq
- **Nghi Danh** - AI Engineer, Renova Cloud
- **Kiet Tran** - AI Engineer, AWS Student Builder Group
- **Bao Phan** - Cloud Engineer, Cloud Kinetics
- **Nguyen Nguyen** - Cloud Engineer, Cloud Kinetics
- **Toan Nguyen** - AWS Security Builder

### Key Highlights

#### 1. AgenticOps for your Cloud
- **Speaker:** Steve Tran
- **The Cloud Operations Paradox:** The evolution to Platform Engineering led to 4x more tools and 3x more engineers, yet MTTR remained flat. Engineers hit a "Complexity Wall".
- **Enterprise AgenticOps Solution:** An AI ecosystem of Specialist Agents (Cloud, Kubernetes, Security) coordinated by a Super Agent to automate complex manual tasks.
- **Core Philosophy:** Transitioning from alert-driven to action-driven systems ("Observability tools sees everything. CloudThinker acts on it. learn it.").
- **Operational Impact (ROI):**
  - Reduces MTTR by 87% and auto-resolves 70% of incidents.
  - Recovers 10-25% of wasted cloud resources.
  - Reduces engineer toil by 40%.

#### 2. Building Voice Agent at Scale
- **Speakers:** Trung Vu, Nghi Danh, Kiet Tran
- **Voice Agents Are Streaming Systems:** Requires simultaneous streams and bidirectional audio, not traditional request/response turns.
- **From Demo to Production:** The team chose a *Cascaded Pipeline (STT -> LLM -> TTS)* over *Speech-to-speech* to ensure text reliability for guardrails, accurate tool calling, and better handling of Vietnamese tonal complexities.
- **Latency Optimization:** Employed continuous streaming, preemptive generation, and early session warm-up to eliminate lag and make three hops feel like one.
- **Turn-taking & Control:** Developed a custom Vietnamese conversational model (81% accuracy) to prevent rude interruptions. Flow is strictly managed via State Machines and RAG for hallucination-free responses.
- **Operations:** Rigorous pre-launch evaluation, full observability, and deep integration with enterprise telephony (SIP, WebRTC, PII masking).

#### 3. AWS DevOps Agent: Your Always-Available Operations Teammate
- **Speakers:** Nguyen Nguyen, Bao Phan
- **The Cost of Manual Investigation:** Fragmented telemetry and knowledge gaps lead to high MTTD/MTTR and a purely reactive problem-solving culture.
- **Solution - AWS DevOps Agent:** An autonomous AI agent resolving and proactively preventing incidents across AWS, Azure, and on-prem.
- **Key Differentiators:** Learns application topology and context, enforces guardrails via MCP, integrates with Slack/ServiceNow, and requires zero-provision setup.
- **Incident Lifecycle (4 Steps):** Seamlessly navigates through Triage (Correlate) -> Investigation (Analyze) -> Mitigation (Plan) -> Prevention (Monitor).
- **ROI:** Enabled clients (WGU, ZENCHEF, KDDI) to reduce incident resolution times by 73% to 77%.

#### 4. AI-Powered Productivity: Workforce Planning For Enterprise
- **Speakers:** Truong Tran, Anh Dang
- **HR Pain Points:** Manual CV screening and gut-feel hiring cause high fail rates, talent gaps, and invisible strategic risks for the business.
- **Amazon Quick Suite Solution:** An AI ecosystem (Chat Agents, Research, Quick Sight, Flows, Automate) built on a secure Data Foundation. It cuts screening time by 80% and empowers data-driven decisions.
- **Data & Architecture:** Protected by strict guardrails. Seamlessly connects to Relational Data Stores, SaaS apps, and Knowledge Bases (via Quick Index) utilizing the high-speed SPICE engine.
- **"5 Step AI Workforce" Scenario:** A fully automated pipeline: 
  1. *Connect:* Seamlessly link ATS/LinkedIn data.
  2. *Automate:* AI evaluates scores and suggests salaries.
  3. *Visualize:* Generate dashboards on candidate flow.
  4. *Decide:* Auto-update pipeline status and draft offers.
  5. *Track:* Automate interview scheduling.

#### 5. Building secure private MCP for Quick
- **Speakers:** Toan Nguyen, Nghi Danh
- **MCP Architecture:** Overview of the Model Context Protocol connecting a Host/Client (e.g., Amazon Quick) to various MCP Servers.
- **The Security Context:** By default, Amazon Quick's MCP Connector requires a publicly accessible endpoint, increasing attack surfaces and violating strict enterprise policies (Zero Trust, Data Residency).
- **The Solution (VPC Connection):** Implementing a fully private pathway by forcing Amazon Quick to connect via a private-IP ENI and using Private DNS (Route 53 Resolver).
- **Secure Request Flow:** Routing moves entirely inside the VPC: Quick -> VPC Connection -> HTTPS to Internal ALB (TLS termination) -> HTTP to MCP Server. This ensures 100% private data transit.

---

### Key Takeaways

*After the event, I think I have gained knowledge about Amazon Quick, MCP, and how MCP works. I don't fully understand or learn much about the other topics yet, so perhaps I will research the remaining topics later. Additionally, during this event, I also practiced the habit of taking notes, which helped me avoid sleepiness and stay focused on listening.*

---

### Applying to Work

*Perhaps I will look further into Amazon Quick and apply it to my future projects. As for topics like Voice Agent or DevOps Agent, I will research more and consider applying them to my other personal projects.*

---

### Event Experience

*Since this was my third event, I had become familiar with the event atmosphere and was quite excited about the speakers' presentations. However, this event was not as lively as the previous two events I attended.*

> *This event felt like it went by quite quickly for me, but it was easy to understand and apply. Other than that, I have no further comments on this event.*

---

#### Event Photos

![Thong Hoai Quy participating in FCAJ Community Day](/images/4-EventParticipated/event3_proof.jpg)

![Slide "How DevOps Agent work" introducing incident lifecycle and devops agent workflows](/images/4-EventParticipated/event3_slide1.jpg)

![Slide "Challenges: The Cost of Manual Incident Investigation" detailing operational overhead and challenges](/images/4-EventParticipated/event3_slide2.jpg)
