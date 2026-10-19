# Eric White | PMP | CISM | ITIL | CSM

**Director-level Technical Program Manager (TPM)**  
Platform Security | AI Governance | Infrastructure | Compliance  
San Francisco Bay Area | [edwhite@gmail.com](mailto:edwhite@gmail.com) | [LinkedIn](https://www.linkedin.com/in/edwhite)

I'm a TPM who sits at the intersection of security engineering, cloud infrastructure, compliance, and large-scale program execution.

I led platform security programs spanning 100+ engineering teams across AWS and GCP. That work included encryption modernization, PKI, TLS hardening, HSM key lifecycle, regulatory execution, and the slow practical work of keeping large groups aligned when the stakes are real. Before that, more than ten years of infrastructure delivery: data centers, server and storage migrations, and network rollouts.

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

I run my own agent stack. Not a chatbot I ask things, a set of scheduled jobs that produce a morning briefing, triage seven inboxes, stage drafts I review before anything sends, and roll the week up on Sundays. Every run logs cost, duration, token usage, step count, and a failure category into SQLite, because "did it run" and "was it any good" are different questions and only one of them is easy.

The interesting part is not the agents. It is the checking around them.

Anything an agent generates for me passes deterministic checks before I trust it. Banned phrases, house style, whether a claim can be traced to a source, whether a PDF actually parses the way an applicant tracking system will read it. Those checks are plain code with tests, not more AI. When an AI-assisted workflow goes wrong it usually goes wrong confidently, and a second model agreeing with the first is not verification.

A few working rules that came out of getting this wrong:

- **A write path that works is not evidence the read path does.** I have found several controls that were documented, believed live, and doing nothing. A checkbox in a task list is not evidence either half works.
- **A check that has never caught anything is a check nobody has verified.** Three of my columns were read faithfully every day from a table nothing ever wrote to, so the check on them never once failed.
- **When a claim will not settle, check whether it is true before arguing about whether it is allowed.** Cost me three days once, on a line that turned out to describe something that never happened.
- **The rule and the mechanism both existing does not mean they cover the same ground.** I had a style rule enforced on my resume for months while the repos strangers actually read went unchecked.

Same principle as the program work: the plan is not the job, making sure the right thing actually happens is the job. Agents just made it cheaper to find out when it did not.

The stack itself is private, since it is wired into my calendar, mail, and finances. The reusable parts get published here. Three of those checks are in [agent-guardrails](https://github.com/ChefPlex/agent-guardrails).

## What I Work On

```text
Program Management   Building the TPM function, cross-org delivery across 100+ teams, executive reporting, portfolio governance
Infrastructure       Data center and site build-out, server and storage migration, network rollouts, Active Directory and LDAP
Cloud & Platform     AWS, GCP, multi-cloud security, platform adoption and enablement
Platform Security    Encryption in transit and at rest, PKI, HSM, TLS modernization
AI                   AI readiness and governance programs, hands-on AI-native delivery and automation
Trust & Compliance   SOC 2, HIPAA, EU Digital Services Act, Election Support
```

## What You'll Find Here

This account is where I share TPM artifacts, templates, tools, examples, and working notes built or refined through real program work.

| Repo | What It Is |
|:---|:---|
| [agent-guardrails](https://github.com/ChefPlex/agent-guardrails) | Three checks for AI agent workflows that refuse to report a pass they did not earn. A prompt-injection alarm that says plainly it is an alarm and not a defense, a way to catch what a coverage check never counted, and a wrapper around an eval runner (promptfoo) that reports the spread instead of one number |
| [ai-automations](https://github.com/ChefPlex/ai-automations) | Prompts I actually use, and the frameworks for deciding how much AI belongs in a piece of work at all. Includes [frameworks](https://github.com/ChefPlex/ai-automations/tree/main/frameworks) - a 5-tier AI execution maturity model, from human-only to AI-only, for deciding how much AI belongs in a given activity, the method for mapping a company's work against it, a 19-role 8-phase multi-agent delivery framework, and a tool decision matrix sequenced by return rather than hype |
| [infrastructure-program-playbooks](https://github.com/ChefPlex/infrastructure-program-playbooks) | What I'd hand a TPM taking over a data center, migration, directory or network program in their first week |
| [learning-notes](https://github.com/ChefPlex/learning-notes) | A public notebook. Some of it will turn out to be wrong, which is rather the point |
| [program-reporting-frameworks](https://github.com/ChefPlex/program-reporting-frameworks) | How to write a status report an executive can act on, and a steering deck that forces a decision |
| [security-program-playbooks](https://github.com/ChefPlex/security-program-playbooks) | What I'd hand a TPM taking over an encryption or compliance program in their first week. Includes [enterprise RAG security](https://github.com/ChefPlex/security-program-playbooks/tree/main/enterprise-rag-security) - trust boundary, permission-aware retrieval, and a prompt injection threat model |
| [tpm-templates](https://github.com/ChefPlex/tpm-templates) | The documents a program actually needs, with notes on how each one usually fails. Includes the [enterprise RAG program](https://github.com/ChefPlex/tpm-templates/tree/main/enterprise-rag-program) - running retrieval as a program rather than an AI experiment |
| [tpm-toolbox](https://github.com/ChefPlex/tpm-toolbox) | The things I kept using after the program ended. Includes the Slack crawler |

Outside the TPM world:

| Repo | What It Is |
|:---|:---|
| [food-wine-farms](https://github.com/ChefPlex/food-wine-farms) | Regional food and wine guides, built and shipped solo. Chef-curated, not scraped |
| [GlassART](https://github.com/ChefPlex/GlassART) | The shop table at Public Glass, written down. The finished work is at artglasssf.com |
| [teaching-notes](https://github.com/ChefPlex/teaching-notes) | Explaining technical things to people who don't do them for a living. Slides, handouts, and what actually landed |

## Career Snapshot

### Talamel Health Technologies

**VP of Technical Execution and Innovation (Fractional)**  
June 2026 to present

- Designed a 5-tier AI governance framework for a healthcare AI startup, covering a PHI-aware tool decision matrix and a compliance-sequenced adoption roadmap across HIPAA, SOC 2 Type I/II, and BAA chain logic
- Own parallel SOC 2 and HIPAA audit cycles end to end, from findings through to working directly with the external auditor: SOC 2 went from scoping to a signed Type I report and a delivered Type II attestation, and a stalled HIPAA effort that had no owner was recovered and completed
- Led a four-lens codebase audit of the flagship product (architecture, security, backend, QA). Its top-priority defects were later confirmed independently by the external audit
- Independently built a 19-role, 8-phase multi-agent AI software delivery framework with tier-selection logic and full audit trails, and deployed it at the startup, where its QA roles audit requirements-to-code traceability across three systems

### Salesforce

**Director, Technical Program Management**  
April 2018 to August 2026

- Drove platform-wide encryption coverage from 10% to 80%+ across 100+ engineering teams and 300+ distributed services
- Led TLS 1.3 modernization, retiring 90% of legacy TLS 1.0/1.1 endpoints across 100+ services
- Ran Platform Security's program governance across 20 programs, 100+ engineering teams and 300+ distributed services, coordinated without direct authority
- Established program management from the ground up in the cryptography group, which had none, and moved it to on-time delivery within 6 months
- Defined the TPM operating model adopted across 10+ engineering orgs, covering intake, status, risk, dependency and escalation
- Drove email domain verification controls with a very small engineering team, owning the customer communication needed to land a required control on an existing customer base, highest-risk accounts first
- Directed the EU Digital Services Act (DSA) program to go-live ahead of the February 2024 enforcement deadline, holding response SLAs of 24 hours to 7 days by item type and reporting to the board of directors
- Ran Election Support readiness programs across several federal and international election cycles
- Cut mean time to remediate (MTTR) for critical vulnerabilities from ~30 days to ~10 across 300+ platform services
- Ran certificate issuance and secure key lifecycle programs on enterprise HSM infrastructure for a global customer base of 150,000+ organizations
- Mentored and onboarded 8 to 10 technical program managers across Salesforce
- Recovered an at-risk contract renewal with a major enterprise customer as the escalation point for their security inquiries. The customer renewed

### Taos, an IBM Company

**Senior Technical Program Manager (TPM) / Practice Lead**  
2011 to 2018

- Led the Technical Program Manager (TPM) practice: 15+ senior consultant TPMs across multiple clients, owning annual reviews, compensation recommendations and the escalation path
- Managed a $10M+ portfolio across HIPAA, PCI, and SOX programs
- Supported clients including Salesforce, City National Bank, UCSF, Dolby, Restoration Hardware, and Blue Shield
- Led infrastructure, compliance, and security-oriented delivery work across client environments
- Hired from the engagement by Restoration Hardware as IT Operations Manager (2011 to 2013), directing technical operations across infrastructure, enterprise applications and security and managing a team of 5, then returned to Taos

### Safeway

**Technical Project Manager 4**  
2009 to 2011

- Delivered a $2M+ data center storage modernization across SAN infrastructure and fabric upgrades (Brocade, EMC VMAX/VPLEX) in two data centers
- Delivered $1.5M in enterprise network upgrades supporting a 1,100-store electronic pharmacy rollout
- Integrated Safeway.com infrastructure into the primary and disaster-recovery data centers

### Bar Association of San Francisco

**Director of Information Technology**  
2005 to 2009

- Led enterprise IT operations, infrastructure architecture, vendor management, and strategic technology planning, managing a team of 3

### Theory and Practice

**Owner**  
2002 to 2005

- Delivered enterprise networking, data architecture, and e-commerce technology programs for Fortune 500 and emerging organizations, managing a team of 10

### Red Herring

**Information Technology Manager**  
2000 to 2001

- Led a team of 4 that designed, built, and supported an intranet/extranet portal (Plumtree) and enterprise application integration programs serving employees and customers, integrating legacy and third-party data sources behind it

## Certifications

CISM &nbsp;|&nbsp; PMP &nbsp;|&nbsp; ITIL &nbsp;|&nbsp; CSM

## Training

SANS LDR553, Cyber Incident Management ([course notes](https://github.com/ChefPlex/learning-notes/blob/main/sans-ldr553-course-notes.md))

## Currently Thinking About

- How AI/ML security programs are maturing, and where they are still chaotic
- Retrieval systems as enterprise programs, and why the permission model is the architecture decision everyone defers
- How to evaluate an agent's output when there is no gold-standard answer to compare it against
- The TPM role in platform reliability versus pure delivery execution
- Making cryptographic compliance tractable for non-security engineering teams
- How to run the post-quantum migration across a very large enterprise, and how to turn around a PMO a company does not value
- How to use AI to speed up program work without outsourcing judgment
- How to build tools that people actually use when the program is messy

## Working Principle

The job is not just to write the plan.

The job is to make sure the right work happens, by the right people, at the right time, with enough clarity that everyone understands why it matters.

Open to conversations about TPM leadership, platform security, AI-assisted execution, and program management at scale.

Always happy to connect on [LinkedIn](https://www.linkedin.com/in/edwhite).
