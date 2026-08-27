# Eric White | PMP | CISM | ITIL | CSM

**Director-level Technical Program Manager**  
Platform Security | Infrastructure | Compliance  
San Francisco Bay Area | [edwhite@gmail.com](mailto:edwhite@gmail.com) | [LinkedIn](https://www.linkedin.com/in/edwhite)

I'm a TPM who sits at the intersection of security engineering, cloud infrastructure, compliance, and large-scale program execution.

I led platform security programs spanning 100+ engineering teams across AWS and GCP. That work included encryption modernization, PKI, TLS hardening, HSM key lifecycle, regulatory execution, and the slow practical work of keeping large groups aligned when the stakes are real.

I'm not a software engineer. I do speak the language fluently enough to challenge architectural decisions, write a useful runbook, ask the awkward risk question, and keep engineering, security, compliance, and leadership pointed at the same outcome.

The rest of the time: glass artist, chef, wine person, cat herder.

> A human being should be able to change a diaper, plan an invasion, butcher a hog,
> conn a ship, design a building, write a sonnet, balance accounts, build a wall,
> set a bone, comfort the dying, take orders, give orders, cooperate, act alone,
> solve equations, analyze a new problem, pitch manure, program a computer,
> cook a tasty meal, fight efficiently, die gallantly. Specialization is for insects.
>
> Robert A. Heinlein

The point is range: learn broadly, work competently across domains, and do not confuse narrow specialization with capability.

## About This Account

This is a working portfolio of things I have built, taught, used, or am actively turning into something reusable.

Some of it is AI-assisted by design. That is part of the point.

AI is useful for speed: drafting, structure, code, cleanup, synthesis, and repeatable workflows. It is not a replacement for taste, judgment, domain knowledge, or deciding what is worth publishing.

The bar is simple: if it would not help someone do the work better, it should not be here.

## How I Actually Work

This is the part that does not fit on a resume, so it lives here.

I run my own agent stack. Not a chatbot I ask things, a set of scheduled jobs that produce a morning briefing, triage six inboxes, stage drafts I review before anything sends, and roll the week up on Sundays. Every run logs cost, duration, token usage, step count, and a failure category into SQLite, because "did it run" and "was it any good" are different questions and only one of them is easy.

The interesting part is not the agents. It is the checking around them.

Anything an agent generates for me passes deterministic checks before I trust it. Banned phrases, house style, whether a claim can be traced to a source, whether a PDF actually parses the way an applicant tracking system will read it. Those checks are plain code with tests, not more AI. When an AI-assisted workflow goes wrong it usually goes wrong confidently, and a second model agreeing with the first is not verification.

A few working rules that came out of getting this wrong:

- **A write path that works is not evidence the read path does.** I have found several controls that were documented, believed live, and doing nothing. A checkbox in a task list is not evidence either half works.
- **A check that has never caught anything is a check nobody has verified.** Three of my columns were logging perfectly into a table nothing wrote to.
- **When a claim will not settle, check whether it is true before arguing about whether it is allowed.** Cost me three days once, on a line that turned out to describe something that never happened.
- **The rule and the mechanism both existing does not mean they cover the same ground.** I had a style rule enforced on my resume for months while the repos strangers actually read went unchecked.

Same principle as the program work: the plan is not the job, making sure the right thing actually happens is the job. Agents just made it cheaper to find out when it did not.

The stack itself is private, since it is wired into my calendar, mail, and finances. The reusable parts get published here.

## What I Work On

```text
Platform Security    Encryption-in-transit, encryption-at-rest, PKI, HSM, TLS modernization
Program Management   Cross-org delivery, OKRs, executive reporting, portfolio governance
Cloud Infrastructure AWS, GCP, multi-cloud security and compliance
AI Security          Emerging security programs for AI/ML platform initiatives
```

## What You'll Find Here

This account is where I share TPM artifacts, templates, tools, examples, and working notes built or refined through real program work.

| Repo | What It Is |
|---|---|
| [ai-automations](https://github.com/ChefPlex/ai-automations) | AI-assisted TPM prompts, workflows, examples, and review checks for safer program artifacts |
| [security-program-playbooks](https://github.com/ChefPlex/security-program-playbooks) | Security TPM guides for intake, compliance triage, evidence planning, and cross-team execution. Includes [enterprise RAG security](https://github.com/ChefPlex/security-program-playbooks/tree/main/enterprise-rag-security) - trust boundary, permission-aware retrieval, and a prompt injection threat model |
| [tpm-templates](https://github.com/ChefPlex/tpm-templates) | Program charters, RFC/ADR templates, RAID guides, communication plans, and lifecycle tools from real TPM work. Includes the [enterprise RAG program](https://github.com/ChefPlex/tpm-templates/tree/main/enterprise-rag-program) - running retrieval as a program rather than an AI experiment |
| [tpm-toolbox](https://github.com/ChefPlex/tpm-toolbox) | Lightweight TPM trackers, checklists, RAID logs, and AI-assisted workflows for program execution |
| [program-reporting-frameworks](https://github.com/ChefPlex/program-reporting-frameworks) | Status, steering committee, lessons-learned, and investment frameworks for honest program reporting |
| [learning-notes](https://github.com/ChefPlex/learning-notes) | Working notes on systems design, security, infrastructure, and TPM craft |

Outside the TPM world:

| Repo | What It Is |
|---|---|
| [food-wine-farms](https://github.com/ChefPlex/food-wine-farms) | AI-assisted regional food and wine guides built from local knowledge, solo shipping, and automated weekly updates |
| [GlassART](https://github.com/ChefPlex/GlassART) | Glassblowing notes, teaching resources, artist business tools, and studio-practice materials |
| [teaching-notes](https://github.com/ChefPlex/teaching-notes) | Teaching materials, demos, explanations, and workshops built to make technical ideas easier to understand |

## Career Snapshot

### Talamel Health Technologies

**VP of Technical Execution and Innovation (Fractional)**  
June 2026 to present

- Designed a 5-tier AI governance framework for a healthcare AI startup, covering a PHI-aware tool decision matrix and a compliance-sequenced adoption roadmap across HIPAA, SOC 2 Type I/II, and BAA chain logic
- Own parallel SOC 2 and HIPAA audit cycles end to end, from findings through to working directly with the external auditor
- Led a four-lens codebase audit of the flagship product (architecture, security, backend, QA), surfacing 21 confirmed and 5 plausible issues
- Built a 19-role, 8-phase multi-agent AI delivery framework with tier-selection logic and full audit trails, used to ship real production features

### Salesforce

**Director, TPM Platform Security**  
2018 to August 2026

- Drove encryption coverage from roughly 10 percent to 80 percent plus across 100+ engineering teams
- Led TLS 1.3 modernization and legacy TLS 1.0/1.1 removal across 100+ services
- Delivered 20 programs on time against regulatory deadlines, including the EU Digital Services Act go-live
- Cut critical-vulnerability MTTR from roughly 30 days to roughly 10 across 300+ platform services
- Ran secure key lifecycle programs across enterprise HSM infrastructure supporting 150,000+ organizations
- Coordinated and mentored TPMs across the org, and was the escalation point for a major enterprise customer's security inquiries on a program that recovered an at-risk renewal

### Taos, an IBM Company

**Senior TPM / Practice Lead**  
2011 to 2018

- Managed a $10M+ portfolio across HIPAA, PCI, and SOX programs
- Supported clients including Salesforce, City National Bank, UCSF, Dolby, and Blue Shield
- Led infrastructure, compliance, and security-oriented delivery work across client environments

### Restoration Hardware

**Manager, Technical Operations**  
2011 to 2013

- Led infrastructure modernization and vendor management for the retail technology stack
- Managed operational systems where reliability, cost, and business continuity all mattered

## Certifications

CISM &nbsp;|&nbsp; PMP &nbsp;|&nbsp; ITIL &nbsp;|&nbsp; CSM &nbsp;|&nbsp; SANS LDR553 (Cyber Incident Management)

## Currently Thinking About

- How AI/ML security programs are maturing, and where they are still chaotic
- Retrieval systems as enterprise programs, and why the permission model is the architecture decision everyone defers
- How to evaluate an agent's output when there is no gold-standard answer to compare it against
- The TPM role in platform reliability versus pure delivery execution
- Making cryptographic compliance tractable for non-security engineering teams
- How to use AI to speed up program work without outsourcing judgment
- How to build tools that people actually use when the program is messy

## Working Principle

The job is not just to write the plan.

The job is to make sure the right work happens, by the right people, at the right time, with enough clarity that everyone understands why it matters.

Open to conversations about TPM leadership, platform security, AI-assisted execution, and program management at scale.

Always happy to connect on [LinkedIn](https://www.linkedin.com/in/edwhite).
