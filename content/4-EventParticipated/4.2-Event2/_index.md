---
title: "FCAJ Community Day"
date: 2026-05-23
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---



### Event Objectives

- Share knowledge on the role of context in making AI work effectively.
- Introduce the smart AI assistant Amazon Quick and its capabilities in data exploration and workflow automation.
- Present solutions for security, cost optimization, and performance enhancement at the edge using Amazon CloudFront.
- Share practical experience from a 36-hour Hackathon (LotusHacks) to build a product from idea to reality.
- Demystify the non-determinism of "deterministic" LLM settings and outline mitigation strategies.
- Introduce enterprise-grade Multi-Agent systems using a startup credit scoring case study.

### Speakers

- **Vy Lam** - Senior Business Systems Analyst, VPBank
- **Thao Nguyen** - GenAI Engineer, VIB
- **Mai Nguyen** - GenAI Engineer, VIB
- **Uyen Le** - GenAI Engineer, VIB
- **Pham Nguyen Hai Anh** - Cloud Consultant, G-AsiaPacific Vietnam
- **Thinh Nguyen** - Devops Engineer, FCAJ
- **Tinh Truong** - Platform Engineer, GoTymeX
- **Duc Dao** - Solutions Architect, Cloud Kinetics

### Key Highlights

#### 1. Context Is Everything: Making AI Actually Work for You

- **Speaker:** Tinh Truong (Platform Engineer, GoTymeX)
- **The Core Problem of AI Today:** Current AI models are already powerful, but the reason we often get generic or incorrect answers is not a bad model, but a lack of "Context". AI cannot read your mind.
- **3 Common Prompting Mistakes:**
  - *The "Internet Puller":* Dumping too much irrelevant documentation confuses the AI (Context Quality > Context Quantity).
  - *Telling AI what it already knows:* Providing redundant information instead of focusing on what needs to change.
  - *No Goal, No Constraints:* Asking vague questions without clear goals, constraints, or success criteria.
- **The Evolution - Second AI Brain:** The future of AI is not just Prompts, but **Prompt + Context + Memory**. The "Second AI Brain" concept allows systems to automatically remember, store, and retrieve the right context using Vector DB architectures.
- **Context Framework:** Always define 4 elements before asking AI: Goal, Relevant info, Constraints, and Success criteria.

#### 2. Friendly AI Assistant with Amazon Quick

- **Speaker:** Pham Nguyen Hai Anh (Cloud Consultant, G-AsiaPacific Vietnam)
- **Solving Business Problems:** Business users often perform repetitive and time-consuming tasks like gathering information and analyzing data from multiple sources.
- **Amazon Q Ecosystem (Quick Suite):** Provides a unified and secure experience with powerful Agentic AI capabilities, connecting to 40+ data sources (Databases, Web search, User files) in the enterprise.
- **Key Features:**
  - *Quick Chat & Insights:* Q&A and information retrieval from World knowledge & Company data.
  - *Quick Flows:* Automating workflows (Marketing, Sales, HR) using natural language without writing code.
  - *Quick Spaces & BI Dashboards:* Collaborative workspaces and smart data visualization.
- **Practical Application (PM Assistant):** A Project Manager assistant can automatically create Minutes of Meeting (MoM), send emails to stakeholders, and schedule the next meeting with simple configurations.

#### 3. From Edge To Origin: CloudFront as Your Foundation

- **Speaker:** Thinh Nguyen (Devops Engineer, FCAJ)
- **Customer Challenges:** Hard to estimate CDN costs due to traffic variability (pay-as-you-go). Users fear massive bill spikes from DDoS attacks or sudden viral content.
- **Comprehensive Protection (DDoS & Security):**
  - A massive global network (700+ PoPs) distributes and absorbs large-scale DDoS attacks at the edge.
  - Integrated advanced features like Origin cloaking (OAC, VPC Origin), Viewer access control (Geo-blocking), and Signed URLs to prevent content theft.
- **Performance & Cost Optimization:**
  - Multi-layer caching and Origin Shield improve Cache Hit Ratios, preventing origin overload.
  - HTTP/3 (QUIC/UDP) support and automatic compression reduce load times by up to 81%.
  - Significantly reduces Load Balancer and origin CPU load (EC2 CPU drops from 5% to 1%). Ultimately, CloudFront reduces overall infrastructure costs.

#### 4. 36 hrs with LotusHacks – Building UTMorpho from Idea to Reality

- **Speakers:** Thao Nguyen, Mai Nguyen, Uyen Le (GenAI Engineers, VIB)
- **The LotusHacks 2026 Journey:** The real-life experience of coding continuously for 36 hours at Vietnam's largest hackathon.
- **From Zero to UTMorpho:** The initial brainstorm was tough ("Head empty"). The team found their idea by looking at their daily work, turning real workplace frustrations into the UTMorpho product.
- **Technical Challenges & Pressure:**
  - Struggled with AI Overgeneration, Token limits, and Burnout near pitch time.
  - The Turning Point was focusing on a "Focused Editing Experience", cutting unnecessary features to highlight the core value.
- **Key Learnings:** Real Frustration Creates Real Ideas. "More Ideas ≠ Better Ideas". Finally, Team Sync is the most critical survival factor in a hackathon.

#### 5. Non-Determinism of "Deterministic" LLM Settings

- **Speaker:** Duc Dao (Solutions Architect, Cloud Kinetics)
- **The Temperature = 0 Myth:** Many engineers assume that setting `Temperature = 0` makes an LLM perfectly deterministic (same input always yields exact same output). This is often relied upon for JSON parsing or automated testing.
- **The Reality:** Research shows accuracy can vary by up to 15% (and up to 70% gap on the same task) between identical runs.
- **Root Causes:**
  - *Technical:* Floating-point arithmetic on GPUs is non-associative: `(a+b)+c != a+(b+c)`. Tiny rounding differences can flip the final token selection.
  - *Commercial:* "Inference batching". API providers group multiple users' requests into one batch for GPU efficiency, which slightly alters the computation for your specific request.
- **Mitigation Strategies:**
  - Treat LLM outputs as probabilistic and build systems that handle variance.
  - Using `Temp = 0.1` is often a better "sweet spot" than `0` to prevent models from getting stuck in repetitive loops.

#### 6. Enterprise-Grade Multi-Agent System: The Case of Startup Credit Scoring

- **Speaker:** Vy Lam (Senior Business Systems Analyst, VPBank)
- **The Data Mismatch:** Traditional credit scoring (requiring 3 years of statements, collateral) completely fails for startups (who only have 6-18 months of runway, with IP and Team as assets).
- **The Single Agent Problem:** Using one AI Agent as a "Credit Approver" leads to context limits, expertise dilution, lack of checks & balances, and creates a single point of failure.
- **Multi-Agent Architecture (Virtual Credit Committee):** Building a committee of specialized agents: Financial Analyst, Market Analyst, Team Evaluator, Risk Assessor, and Compliance.
  - *Benefits:* Parallel processing, full auditability, and agents can cross-check each other's assumptions.
- **Enterprise-Grade Requirements:** To reach Production, the system must address 6 pillars: Security (MFA, Encryption), Data Governance, Network (VPC, PrivateLink), Operations, Human Factors, and Compliance (SOC 2, GDPR).
- **Operational ROI:** Processing time drops by 95% (from 2-3 weeks to 2-4 hours), saving 95% in costs. Enterprise AI isn't just about making things work; it's about making them work securely, reliably, and at scale.

---

### Key Takeaways

*After the event, I learned a lot of useful things from the speakers, especially about optimizing costs with CloudFront, managing and allocating time effectively when working in teams, and many other beneficial topics.*

---

### Applying to Work

*Regarding the application of the knowledge I heard, I think I can apply time management and effective task and time allocation when working in teams, as well as optimize costs when using CloudFront. The remaining knowledge is quite new to me, so I will probably research and apply it in the future.*

---

### Event Experience

*When participating in today's FCAJ Community Day event, I felt very excited and happy to hear the speakers share real-world knowledge on using AI for work. Although I was still a bit shy and didn't dare to ask questions, I learned a lot from the event and had the opportunity to connect and chat with many other participants. Even though this was the second event I attended, it felt like the first time—exciting and highly anticipated.*

---

#### Event Photos

![Thong Hoai Quy participating in FCAJ Community Day](/images/4-EventParticipated/event2_proof.jpg)

![Slide "Context Is Everything" presented by Tinh Truong](/images/4-EventParticipated/event2_slide1.jpg)

> *Finally, I found today's event extremely beneficial; it helped me acquire a lot of new knowledge and also gave me the opportunity to network with other participants.*
