---
title: "AWS First Cloud Journey - Workshop"
date: 2026-05-09
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

{{% notice warning %}}
⚠️ **Note:** The information below is for reference purposes only. Please **do not copy it verbatim** into your report, including this warning.
{{% /notice %}}

# Summary Report: “AWS First Cloud Journey - Sharing Session”

### Event Objectives

- Explore gamified learning strategies to build productive habits and maintain consistent study streaks.
- Learn standard and advanced prompt engineering techniques to maximize LLM response quality.
- Understand token economics and the serverless architecture design of a prompt optimization application (Proptimizer) on AWS.

### Speakers

- **Huynh Hoang Long** - Admin of FCAJ
- **Nguyen Tuan Thinh** - DevOps/Cloud Engineer, First Cloud AI Journey
- **Khang** - Speaker of Session 3
- **Thao Nguyen** - GenAI Engineer, VIB

### Key Highlights

#### 1. Addicted to Learning Like You're Addicted to Social Media
- **Speaker:** Huynh Hoang Long (Admin of FCAJ)
- **Dopamine Mechanics:** Dopamine is released when expecting a reward. Apply "Variable Reward" and "Learning Loop" (Curiosity → Try → Explore → Satisfaction) to keep learners engaged.
- **3 Brain Hacks to Make Learning Feel Like Playing:**
  * *Fear of Loss:* Maintain consistent study habits using streak mechanics (similar to Duolingo, TikTok, or daily game check-in rewards).
  * *Trick the Amygdala:* Simplify goals with the **2-Minute Rule** (just open the file, read one page, or solve one question to start easily).
  * *Instant Feedback:* Reward yourself immediately after milestones (e.g., study for 25 minutes to get +10 XP, get coffee after finishing a chapter).
- **Conclusion:** Winners are those who build habits/systems that help them continue automatically every day.

#### 2. Automated Prompt Engineering: Enhancing LLM Output Quality
- **Speaker:** Nguyen Tuan Thinh (DevOps/Cloud Engineer, First Cloud AI Journey)
- **Overview:** Writing clear, structured prompts (Role, Instruction, Context, Constraints...) helps optimize output quality and control token costs (Token Economics).
- **Advanced Prompting Techniques:**
  * *Chain-of-Thought (CoT) & Self-Consistency:* Reason sequentially and select the most consistent response.
  * *Tree of Thoughts (ToT):* Branch thoughts like a tree to evaluate and find the optimal path.
  * *RAG & Role Prompting.*
- **Proptimizer Project (Solution Architecture):** A browser extension to optimize prompts and chat with AI:
  * *S3 & CloudFront:* Store and distribute static web assets globally with low latency.
  * *Cognito:* Manage user registration, sign-in, and secure authentication via JWT.
  * *API Gateway & Lambda:* Route APIs and process business logic serverless.
  * *Amazon Bedrock:* Connect foundation models (like Claude) to optimize prompts.
  * *DynamoDB & CloudWatch:* Store user data (NoSQL) and monitor logs/metrics.
  * *Cost & Demo:* Optimized infrastructure cost at $0 (excluding Bedrock). Demo site hosted at `https://d3jqm7so635aqb.cloudfront.net`.

#### 3. AI-Ready Freshers: Skills and Mindset in the AI Era
- **Speaker:** Khang
- **AI Impact & Multiplier:** AI can empower or demote you. You can outsource your thinking, but you cannot outsource your understanding. AI is a multiplier, not a replacement.
- **Growth Mindset & Integrity:**
  * Ask "Why?" and embrace mistakes as lessons.
  * Do your best even when no one is watching, avoid "AI shortcuts," and build your character.
- **Career Direction & Evaluation:**
  * Career fulfillment lives at the intersection of: What you love (Passion), What benefits you (Benefits), and What you have to do (Responsibility).
  * 5 Benefits of Work: Salary, Experience, Network, Knowledge, and Growth.
  * 5 Dimensions of Evaluation: Attitude, Competence, Experience, Exposure, and Potential.
- **Next Actions:** Ask "Why?", form a long-term roadmap (Look far, start Small), and build a team because "to go far, go together".

#### 4. BMAD Method: Bringing Your Agile & AI Teams into Your IDE
- **Speaker:** Thao Nguyen (GenAI Engineer, VIB)
- **The Issue with Vibe Coding:** Entrusting an entire project to a single chat interface ignores the Software Development Life Cycle (SDLC), leading to context bloat, fragmented code, and non-scalable projects.
- **BMAD Method (Context Engineering):** Shifting to an Agile framework using specialized AI Agent roles (Orchestrator, PM, Architect, PO, Scrum Master, Dev & Reviewer).
- **Closed-Loop Workflow:**
  * *Planning & Sharding:* Interactively defines PRDs and Architectures, then shards documents into tiny Index chunks to isolate context and prevent LLM hallucinations.
  * *Execution & Testing:* Scrum Master manages Story approvals, Developer Agent writes precise code, and Review Agent loops testing/refactoring until errors hit zero.
- **Ecosystem & Deployment:** Expandable through modular suites (BMAD Core, Creative Suite, BMB, TEA) and locally deployable via `npx bmad-method@next install .` (integrating with Cursor, Windsurf, Claude Code). Open source code at `github.com/bmad-code-org/BMAD-METHOD`.

---

### Key Takeaways

*What I learned in the first event was about how to self-motivate for more effective studying. Although I am quite lazy and usually spend more time gaming, after listening to Mr. Long's sharing, I think I will try adding a reward system after learning some new knowledge. Additionally, I think the BMAD method is very interesting and will be useful for many people, helping everyone save time and effort in software development.*

---

### Applying to Work

*Regarding application to studying or work, I find BMAD very suitable for applying to my personal projects. Additionally, Mr. Long's sharing can also be effectively applied to my studies to help me become more addicted to studying than to gaming.*

---

### Event Experience

*Participating in this event for the first time made me feel quite nervous and a bit anxious because I am rather shy around so many people. However, after experiencing it, I think I want to attend more. Although I did not dare to stand up and share knowledge with everyone, I think participating and listening still helped me a lot.*

---

#### Event Photos

*(Add your photos from this event here)*

> *My comment on participating in this event for the first time is that it was a wonderful experience and well worth attending. I hope to join future events to hear more knowledge and experience from senior industry professionals.*
