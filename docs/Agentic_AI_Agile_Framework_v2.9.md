# Agentic AI Agile Framework v 2.9 -- A Comprehensive "People and Process‑First" Playbook

**Release Date: May 2025 License: CC BY 4.0**

**Author: Devashish Saxena (devashishsaxena@gmail.com)**

**Purpose:** End‑to‑end operating model for conceiving, designing,
testing, and governing enterprise‑grade agentic AI systems. Assumes the
prioritization of use cases has already been done as a separate
exercise.\
**Audience:** CDO / CIO, Product & Engineering Leaders, Transformation
PMOs.

## Phase 0: People and Process Discovery (Starting Point)

**Purpose**: Deeply understand the current state: who are the end users,
who are the internal actors, what is the current process, how does it
perform today, what works well, where are the friction points?

  -------------------------------------------------------------------------------------
  Activity                   Description          Key Questions    Key Outputs
  -------------------------- -------------------- ---------------- --------------------
  End user journey mapping   For customer facing  Who are the end  End user journey map
                             use cases (e.g.      users? What is   by phases for
                             customer support)    their journey    different personas:
                             define current end   today? What do   what tasks are
                             user journey and     they like about  performed, where are
                             understand the       the current      current friction
                             different personas   journey? Where   points,
                             and especially where are their        change-impact matrix
                             the current friction friction points? 
                             points are                            

  Current state Process      Build a common       Current          Swim‑lane map,
  Mapping                    visual baseline of   end‑to‑end flow? pain‑point heat‑map
                             the current business Bottlenecks,     
                             process(es)          decision points, 
                                                  hand‑offs?       

  Business/Internal          With the process map Who does what?   RACI of employee
  Stakeholder & Role         in place, capture    KPIs,            actors, current pain
  Analysis                   who (internally)     incentives,      points,
                             touches each step    friction?        change‑impact matrix
                             and their                             
                             incentives/KPIs                       

  Baseline Metrics Capture   With roles           Current "impact" Baseline KPI
                             understood, pull in  metrics revenue, dashboard (proof of
                             baseline hard        NPS or outcome   impact), Data
                             numbers, understand  satisfaction and quality
                             trends               unit service     
                                                  cost             

  Waste‑to‑Zero Workshop     Run a fast kaizen    Which manual     Simplified
                             workshop -- cross    steps can be     future‑state flow
                             functional session   eliminated       with "zero waste",
                             designed to identify before           waste log
                             and eliminate every  automation?      
                             non-value-added step                  

  Knowledge Codification     In cleaned up        What is the      Canonical SOP deck
                             process, identify    "golden path"    for prompt/agent
                             the fastest,         SOP for this     design, decision
                             simplest error-free  workflow?        trees
                             sequence of steps                     
                             that achieves the                     
                             desired business                      
                             outcome                               

  Feature Opportunity Sizing Size the steps for   Where could      Impact‑feasibility
                             agentic lift (speed, autonomous       matrix, prioritized
                             experience quality,  agents lift      use-case/feature
                             risk reduction)      speed,           backlog
                             using chance-impact  experience       
                             or                   quality, risk?   
                             impact-feasibility                    
                             scoring                               

  Target‑State Co‑Design     With waste removed,  How must the     Future‑state
                             SOPs codified, and   process evolve   blueprint,
                             opportunities        for autonomy &   re‑engineered
                             ranked, design the   observability?   workflows
                             future-state process                  
                             that agents will                      
                             inhabit.                              
  -------------------------------------------------------------------------------------

**Outcome**: Bundle all Phase 0 artifacts into a **Process‑First Charter
with baseline KPIs** that feeds Phase 1.

**Trust‑Posture Snapshot (read this first)**

- Security grade: **ISO 27001 mapped**, zero hard‑coded secrets.

- Privacy: **PII redacted at RAG retrieval**; row‑level ACL.

- Kill‑switch SLA: **\< 30 s** tested quarterly.

- Model lifecycle: registry with upgrade checklist.

**KPI Dictionary (enterprise‑agnostic)**

  ----------------------------------------------------------------------------
  ** Metric **        ** Definition **                  ** Why it matters **
  ------------------- --------------------------------- ----------------------
  North‑Star KPI      Single headline outcome (revenue, Aligns agent design to
                      risk, experience)                 business value

  SSAT / NPS          Stakeholder‑Satisfaction score    Proxy for adoption &
                      (1‑5) or Net Promoter Score       quality

  Autonomy %          Interactions fully handled by     Shows ROI realisation
                      agent                             

  Unit Service Cost   OPEX per completed interaction    Cost baseline &
                                                        forecast

  Escalation Rate     \% routed to human oversight      Balance safety vs
                                                        autonomy

  Latency p95         95th percentile end‑to‑end time   Experience SLO

  Policy Violations   Guard‑rail breaches per 1k calls  Ethics & compliance
                                                        health
  ----------------------------------------------------------------------------

**Phase‑Gate Calendar (typical 16‑week pilot)**

Wk 0‑4 Phase 0 ──►

Wk 5 Mission Definition Gate ✔

Wk 6‑9 Phase 2 ──► Cost‑to‑Serve Gate ✔

Wk 10‑12 Phase 3 ──► Ethics Gate ✔

Wk 13‑14 Phase 4 ──► Prod Go / No‑Go Gate ✔

Wk 15‑16 Hyper‑care roll‑out

## 

## Phase 1. Mission Definition

**Purpose**: Turn the "Process-First Charter" from Phase 0 into a
crystal-clear, metrics-anchored direction for the first set of agents to
be built.

+------------------+---------------------------+---------------------------------------------------------------------------+----------------+
| **Key Activity** | **Description**           | **Primary Roles**                                                         | **Key          |
|                  |                           |                                                                           | Outputs**      |
+==================+===========================+===========================================================================+================+
| **Draft Agentic  | Convert each              |   ----------------------------------------------------------------------- | Set of         |
| Epics**          | high-priority workflow    |   AI Product Owner + Process Owner                                        | Epics---one    |
|                  | into a single *Agentic    |   ----------------------------------------------------------------------- | per candidate  |
|                  | Epic* statement:          |                                                                           | agent          |
|                  |                           |   ----------------------------------------------------------------------- |                |
|                  | • Role (Sales-Assist      |                                                                           |                |
|                  | Agent)\                   |   ----------------------------------------------------------------------- |                |
|                  | • Goal (qualify and route |                                                                           |                |
|                  | inbound leads)\           |   ----------------------------------------------------------------------- |                |
|                  | • Tools/Data (CRM API,    |                                                                           |                |
|                  | pricing DB)\              |                                                                           |                |
|                  | • Constraints (privacy    |                                                                           |                |
|                  | tier, SLA)\               |                                                                           |                |
|                  | • North-Star KPI          |                                                                           |                |
|                  | (lead-conversion rate)\   |                                                                           |                |
|                  | • Optimization metric     |                                                                           |                |
|                  | (cycle time)              |                                                                           |                |
+------------------+---------------------------+---------------------------------------------------------------------------+----------------+
| **Define Success | • Quantify **North-Star   | AI Product Owner, Ethics Partner, Risk Lead                               | **KPI &        |
| and              | KPI (revenue, cost, risk  |                                                                           | Guard-Rail     |
| Guard-Rails**    | or customer/stakeholder   |                                                                           | Matrix** (one  |
|                  | experience) baseline vs   |                                                                           | row per KPI,   |
|                  | target** \                |                                                                           | one row per    |
|                  | • Select 2-4              |                                                                           | guard-rail;    |
|                  | supporting/operating KPIs |                                                                           | includes       |
|                  | (cost-per-unit, SSAT,     |                                                                           | target, owner, |
|                  | error rate)\              |                                                                           | data source).  |
|                  | • Establish guard rails - |                                                                           |                |
|                  | document policy, legal,   |                                                                           | **Escalation & |
|                  | ethical, safety,          |                                                                           | Confidence     |
|                  | brand/tone and            |                                                                           | Threshold      |
|                  | performance/cost          |                                                                           | Table** (links |
|                  | constraints (e.g., no PII |                                                                           | each trigger   |
|                  | spill)\                   |                                                                           | to the         |
|                  | • Specify escalation      |                                                                           | Responsibility |
|                  | rules (route to human) if |                                                                           | Contract       |
|                  | confidence thresholds not |                                                                           | owner)         |
|                  | met                       |                                                                           |                |
+------------------+---------------------------+---------------------------------------------------------------------------+----------------+
| **Responsibility | For each Epic assign: \   | Product Owner + Ops Lead                                                  | Updated Risk   |
| Contracts**      | • **Agent                 |                                                                           | Register w/    |
|                  | Owner** (accountable      |                                                                           | contracts      |
|                  | exec)\                    |                                                                           |                |
|                  | • Human On-Call           |                                                                           |                |
|                  | (real-time override)\     |                                                                           |                |
|                  | • Failure Action          |                                                                           |                |
|                  | (auto-pause, reroute)     |                                                                           |                |
+------------------+---------------------------+---------------------------------------------------------------------------+----------------+
| **Solution       | Align on high-level       | Agent Architect, Prompt Engineer, AgentOps Lead                           | Feasibility    |
| Architecture and | architecture (single      |                                                                           | memo; rough    |
| Tech Feasibility | agent vs multi-agent, RAG |                                                                           | infra sizing   |
| Check**          | vs no-RAG, required tool  |                                                                           |                |
|                  | integrations). Quick      |                                                                           |                |
|                  | spike to confirm          |                                                                           |                |
|                  | technical viability and   |                                                                           |                |
|                  | token cost ballpark.      |                                                                           |                |
+------------------+---------------------------+---------------------------------------------------------------------------+----------------+
| **Resource and   | Map required FTEs, sprint | Program PMO, CFO rep, Product Owner                                       | Updated        |
| Budget           | count, and infra spend.   |                                                                           | Cost-to-Serve  |
| Alignment**      | Ensure                    |                                                                           | model          |
|                  | the **10-20-70** resource |                                                                           |                |
|                  | mix is still sensible     |                                                                           |                |
|                  | (ensuring ongoing         |                                                                           |                |
|                  | change/adoption           |                                                                           |                |
|                  | activities)               |                                                                           |                |
+------------------+---------------------------+---------------------------------------------------------------------------+----------------+
| **Ethics and     | Ethics Partner reviews    | Ethics Partner                                                            | Pre-check      |
| Alignment        | Epics and guard-rails for |                                                                           | sign-off or    |
| Pre-Check**      | bias, fairness,           |                                                                           | action items   |
|                  | compliance. Flags items   |                                                                           |                |
|                  | that must go              |                                                                           |                |
|                  | through **Ethics Gate**   |                                                                           |                |
|                  | later.                    |                                                                           |                |
+------------------+---------------------------+---------------------------------------------------------------------------+----------------+

**Outcome**: A formally approved **Mission Definition Deck** comprising
of agentic epic 1-pagers, target KPIs, key guard-rails, responsibility
contracts, solution architecture, technical feasibility, resource, and
budget ballparks.

## Phase 2. Agent Design & Tool Wiring

**Purpose**: Turn the approved "Mission Definition" from Phase 1 into a
detailed, build-ready blueprint (prompts, memory design, data/tool
wiring, security guard rails, and a validated cost-to-serve forecast).

+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Key           | **Description**      | **Primary Roles**                                                         | **Key          |
| Activity**      |                      |                                                                           | Outputs**      |
+=================+======================+===========================================================================+================+
| **Platform and  | Evaluate commercial  |   ----------------------------------------------------------------------- | • Platform     |
| Buy-vs-Build    | / OSS agent          |   Agent Architect, AgentOps Lead, Security                                | decision       |
| Decision**      | frameworks (e.g.,    |   ----------------------------------------------------------------------- | note \         |
|                 | CrewAI, LangGraph,   |                                                                           | • Risk         |
|                 | AutoGen) vs bespoke  |   ----------------------------------------------------------------------- | acceptance if  |
|                 | option. Select the   |                                                                           | bespoke        |
|                 | stack that meets     |   ----------------------------------------------------------------------- |                |
|                 | guard-rails,         |                                                                           |                |
|                 | latency,             |   ----------------------------------------------------------------------- |                |
|                 | extensibility, and   |                                                                           |                |
|                 | TCO targets.         |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **High-level    | Choose cognition     | Agent Architect, Data Engineer                                            | • Architecture |
| Architecture    | pattern (single      |                                                                           | diagram        |
| and Memory      | agent,               |                                                                           | (planner,      |
| Design**        | planner-executor,    |                                                                           | executor,      |
|                 | multi-agent). Define |                                                                           | memory tiers,  |
|                 | memory tiers         |                                                                           | tools,         |
|                 | (short-term token    |                                                                           | observability, |
|                 | window, episodic DB, |                                                                           | security)\     |
|                 | long-term vector DB, |                                                                           | • Memory       |
|                 | audit log) and       |                                                                           | schema •       |
|                 | planning loop/flow.  |                                                                           | Planning loop  |
|                 |                      |                                                                           | spec (plan,    |
|                 |                      |                                                                           | act/execute,   |
|                 |                      |                                                                           | evaluate,      |
|                 |                      |                                                                           | record)        |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Tool and Data | List every external  | Prompt / Tooling Engineer, System SMEs                                    | • Toolchain    |
| Integration     | API, data product,   |                                                                           | map \          |
| Spec**          | or RAG corpus the    |                                                                           | • Security     |
|                 | agent will invoke.   |                                                                           | data-flow      |
|                 | Document endpoints,  |                                                                           | diagram        |
|                 | auth, expected       |                                                                           |                |
|                 | latency, cost        |                                                                           |                |
|                 | limits, and          |                                                                           |                |
|                 | observability hooks. |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Prompt and    | Draft prompt         | Prompt Engineer, Ethics Partner                                           | • Prompt       |
| Policy          | taxonomy - system    |                                                                           | library        |
| Engineering**   | prompt, role/persona |                                                                           | (version       |
|                 | prompt, task prompt, |                                                                           | controlled)    |
|                 | function/tool        |                                                                           |                |
|                 | wrappers, fallback   |                                                                           |                |
|                 | prompts, tone guide, |                                                                           |                |
|                 | policy prompts (PII, |                                                                           |                |
|                 | ethics constraints). |                                                                           |                |
|                 | Include inline tags  |                                                                           |                |
|                 | for confidence       |                                                                           |                |
|                 | thresholds and       |                                                                           |                |
|                 | escalation cues.     |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Reusable      | Store new prompts,   | Cross-Pod Guild delegate                                                  | Updated        |
| Asset Library   | wrappers, eval       |                                                                           | enterprise     |
| Contribution**  | configs in a shared  |                                                                           | asset catalog  |
|                 | Cross-Pod            |                                                                           |                |
|                 | repository; tag with |                                                                           |                |
|                 | metadata for         |                                                                           |                |
|                 | searchability.       |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Security and  | Threat-model the     | Security Architect, Ethics Partner                                        | • Threat model |
| Compliance      | agent: auth scopes,  |                                                                           | matrix         |
| Design**        | rate limits, data    |                                                                           |                |
|                 | classification,      |                                                                           | • Security     |
|                 | audit fields. Map to |                                                                           | requirements   |
|                 | guard-rails and SOC2 |                                                                           | doc \          |
|                 | / ISO / HIPAA        |                                                                           | • Compliance   |
|                 | controls as needed.  |                                                                           | mapping matrix |
|                 |                      |                                                                           |                |
|                 |                      |                                                                           | • Ongoing      |
|                 |                      |                                                                           | security test  |
|                 |                      |                                                                           | plan           |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Evaluation    | Build an automated   | Simulation/Test Engineer, AgentOps Lead                                   | • Eval-config  |
| Harness Set-up  | test bed that        |                                                                           | YAML /         |
| (a repeatable   | objectively scores   |                                                                           | notebook       |
| test case       | every new agent      |                                                                           |                |
| pipeline)**     | build against the    |                                                                           |                |
|                 | KPIs and guard-rails |                                                                           |                |
|                 | defined in Phase     |                                                                           |                |
|                 | 1---so failures are  |                                                                           |                |
|                 | caught prior to      |                                                                           |                |
|                 | production.          |                                                                           |                |
|                 |                      |                                                                           |                |
|                 | Configure open       |                                                                           |                |
|                 | harnesses            |                                                                           |                |
|                 | (agentbench,         |                                                                           |                |
|                 | AutoGen-eval, custom |                                                                           |                |
|                 | test suites) aligned |                                                                           |                |
|                 | to KPIs &            |                                                                           |                |
|                 | guard-rails. Draft   |                                                                           |                |
|                 | baseline scenarios.  |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Prototype     | Build a thin         | Architect, Prompt Eng, Ops                                                | •              |
| Spike and Cost  | vertical slice       |                                                                           | Cost-per-call  |
| Profiling**     | (happy path only)    |                                                                           | range \        |
|                 | and run through      |                                                                           | • Latency      |
|                 | evaluation harness   |                                                                           | histogram      |
|                 | to sample token,     |                                                                           |                |
|                 | latency, and infra   |                                                                           |                |
|                 | cost. Iteratively    |                                                                           |                |
|                 | tune prompts / RAG   |                                                                           |                |
|                 | chunking             |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Cost-to-Serve | Aggregate infra      | Product Owner, CFO rep, Ops Lead                                          | • Cost         |
| Forecast and    | pricing, Ops FTE,    |                                                                           | Forecast       |
| Stage-Gate      | 10-20-70 change mix. |                                                                           | model \        |
| Pack**          | Verify data-quality  |                                                                           | • Stage-gate   |
|                 | readiness and        |                                                                           | deck           |
|                 | produce "go / fix /  |                                                                           |                |
|                 | defer"               |                                                                           |                |
|                 | recommendation.      |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+

**Phase 2 Critical Success Factors**

1.  **Prompt & tool wrappers checked into version control** with lint
    rules (no hard-coded API keys, no disallowed phrases).

2.  **Security patterns baked-in early**---waiting until Phase 3 will
    create re-work.

3.  **Cost-to-serve gate** signed off before heavy RLHF or large-scale
    data ingestion begins.

4.  **Reusable assets pushed to the guild repo**---prevents each pod
    reinventing wrappers and eval configs.

5.  **Evaluation harness covers the North-Star KPI and every
    guard-rail** (e.g., adverse prompt tests for policy).

## Phase 3: Simulation & Safety Testing

**Purpose**: Validate agent behavior against functional KPIs and
guard-rails in a fully sandboxed, risk-tiered environment before any
end-user exposure.

+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Key           | **Description**      | **Primary Roles**                                                         | **Key          |
| Activity**      |                      |                                                                           | Outputs**      |
+=================+======================+===========================================================================+================+
| **Simulation    | Spin up sandbox      |   ----------------------------------------------------------------------- | Sandbox        |
| Environment     | infra, load snapshot |   Test Eng, DevOps                                                        | environment    |
| Boot-up**       | RAG, install mocks;  |   ----------------------------------------------------------------------- |                |
|                 | seed synthetic user  |                                                                           |                |
|                 | IDs.                 |   ----------------------------------------------------------------------- |                |
|                 |                      |                                                                           |                |
|                 |                      |   ----------------------------------------------------------------------- |                |
|                 |                      |                                                                           |                |
|                 |                      |   ----------------------------------------------------------------------- |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Risk-Tiered   | Map each tool/data   | Test Eng, Security                                                        | Tiered test    |
| Test Plan**     | call to Tier 1/2/3;  |                                                                           | matrix         |
|                 | assign entry/exit    |                                                                           |                |
|                 | gates                |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Synthetic and | Generate happy-path, | Domain SME, Test Eng                                                      | tests/\*.jsonl |
| Edge-Case       | edge, and stress     |                                                                           |                |
| Dataset Build** | datasets; include    |                                                                           |                |
|                 | policy-violation     |                                                                           |                |
|                 | probes.              |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Harness       | Run evaluation       | AgentOps Lead                                                             | Raw run logs,  |
| Execution and   | harness across all   |                                                                           | metric CSV     |
| Metrics         | tiers; collect       |                                                                           |                |
| Capture**       | accuracy, policy,    |                                                                           |                |
|                 | latency, cost.       |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Red-Team /    | Human red-teamers    | Red-Teamers, Ethics Partner                                               | Red-team       |
| Adversarial     | attempt jailbreak,   |                                                                           | report, CVE    |
| Blitz**         | PII extraction, cost |                                                                           | list           |
|                 | abuse.               |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Fallback-Path | Force tool failures, | Architect, Test Eng                                                       | Escalation     |
| and Escalation  | low-confidence       |                                                                           | drill report   |
| Rehearsal**     | outputs; ensure      |                                                                           |                |
|                 | escalation triggers  |                                                                           |                |
|                 | fire.                |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Reinforcement | SMEs label 200--500  | Prompt Eng, SME                                                           | Fine-tuned     |
| Learning from   | interaction pairs;   |                                                                           | checkpoint /   |
| Human Feedback  | tune model or        |                                                                           | prompt v1.1    |
| (RLHF)          | prompt.              |                                                                           |                |
| Micro-Sprint    |                      |                                                                           |                |
| (optional)**    |                      |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Safety        | Consolidate results; | Product Owner, Ethics Partner                                             | Scorecard PDF; |
| Scorecard &     | tag blockers vs      |                                                                           | JIRA backlog   |
| Remediation     | must-fix-later       |                                                                           |                |
| Backlog**       | items.               |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+
| **Ethics Gate   | Present scorecard:   | Ethics Board, Security, Product Owner                                     | Formal Ethics  |
| Review**        | sign-off,            |                                                                           | approval       |
|                 | conditional go, or   |                                                                           |                |
|                 | reject.              |                                                                           |                |
+-----------------+----------------------+---------------------------------------------------------------------------+----------------+

**Outcome**: Signed Ethics-Gate approval plus a Safety Scorecard showing
accuracy, policy compliance, latency, and cost all within
thresholds---clearing the way for limited human-feedback rollout.

## Phase 4: Human Feedback & Iteration

**Purpose**: Expose the agent to real users in shadow or co-pilot mode,
capture subjective trust signals, refine prompts/tools, and prove
North-Star KPI lift without compromising safety.

+----------------+----------------------+---------------------------------------------------------------------------+--------------+
| **Key          | **Description**      | **Primary Roles**                                                         | **Key        |
| Activity**     |                      |                                                                           | Outputs**    |
+================+======================+===========================================================================+==============+
| **Shadow-Mode  | Agent runs in        |   ----------------------------------------------------------------------- | Shadow log   |
| Launch**       | parallel to humans;  |   Ops Lead, Process Owner                                                 |              |
|                | outputs logged but   |   ----------------------------------------------------------------------- |              |
|                | not shown.           |                                                                           |              |
|                |                      |   ----------------------------------------------------------------------- |              |
|                |                      |                                                                           |              |
|                |                      |   ----------------------------------------------------------------------- |              |
|                |                      |                                                                           |              |
|                |                      |   ----------------------------------------------------------------------- |              |
+----------------+----------------------+---------------------------------------------------------------------------+--------------+
| **Trust UX and | Inject confidence    | Interaction Designer                                                      | Updated UI   |
| Explainability | score, "why" button, |                                                                           | spec         |
| Touchpoints**  | tool call preview    |                                                                           |              |
|                | into UI.             |                                                                           |              |
+----------------+----------------------+---------------------------------------------------------------------------+--------------+
| **User         | 5-min explainer      | Change-Enablement, Process Owner                                          | Training     |
| Education      | videos, FAQ, slack   |                                                                           | artefacts    |
| Bursts**       | posts.               |                                                                           |              |
+----------------+----------------------+---------------------------------------------------------------------------+--------------+
| **Weekly       | Process Owner, Ops,  | Change-Enablement, Process Owner                                          | Huddle       |
| Adoption       | Product review SSAT, |                                                                           | minutes,     |
| Huddle**       | override count,      |                                                                           | tweak list   |
|                | North-Star           |                                                                           |              |
|                | trajectory.          |                                                                           |              |
+----------------+----------------------+---------------------------------------------------------------------------+--------------+
| **Prompt /     | Apply tweaks from    | Prompt Eng, Architect                                                     | Updated      |
| Tool           | logs + huddle; bump  |                                                                           | prompts file |
| Refinement**   | prompt version.      |                                                                           |              |
+----------------+----------------------+---------------------------------------------------------------------------+--------------+
| **KPI Delta    | Compare live shadow  | Product Analyst                                                           | Delta sheet  |
| Assessment**   | KPIs vs baseline;    |                                                                           |              |
|                | update Cost-to-Serve |                                                                           |              |
|                | forecast if needed.  |                                                                           |              |
+----------------+----------------------+---------------------------------------------------------------------------+--------------+
| **Prod Go /    | Steering committee   | Exec Sponsor, Product, Security                                           | Signed Go /  |
| No-Go Review** | checks KPI deltas,   |                                                                           | rollback     |
|                | user-trust signals,  |                                                                           | plan         |
|                | open risks; decide.  |                                                                           |              |
+----------------+----------------------+---------------------------------------------------------------------------+--------------+

**Success factors:** SSAT ≥ baseline, override count trending down,
trust cues understood, no unresolved Sev-1 issues.

**Outcome**: Production Go/No-Go decision backed by live SSAT, override,
and cost data; updated prompt/tool version frozen for GA rollout.

## Phase 5: Deployment, Monitoring & Drift Management

**Purpose**: Gradually roll out full autonomy, operate the agent under
defined SLOs, and maintain performance through continuous drift
detection, value realization reviews, and model lifecycle governance.

+-------------------+----------------------+---------------------------------------------------------------------------+--------------+
| **Key Activity**  | **Description**      | **Primary Roles**                                                         | **Key        |
|                   |                      |                                                                           | Outputs**    |
+===================+======================+===========================================================================+==============+
| **Gradual         | 5 % → 25 % → 50 % →  |   ----------------------------------------------------------------------- | Roll-out     |
| Roll-Out Plan**   | 100 % traffic over   |   AgentOps Lead, Process Owner                                            | program plan |
|                   | "n" weeks with       |   ----------------------------------------------------------------------- |              |
|                   | rollback             |                                                                           |              |
|                   | checkpoints.         |   ----------------------------------------------------------------------- |              |
|                   |                      |                                                                           |              |
|                   |                      |   ----------------------------------------------------------------------- |              |
|                   |                      |                                                                           |              |
|                   |                      |   ----------------------------------------------------------------------- |              |
+-------------------+----------------------+---------------------------------------------------------------------------+--------------+
| **Observability   | Build observability  | Ops, DevOps                                                               | Live         |
| Dashboard         | dashboard using e.g. |                                                                           | dashboard    |
| Go-Live**         | Grafana/Datadog      |                                                                           | URL          |
|                   | monitoring: latency, |                                                                           |              |
|                   | cost, autonomy       |                                                                           |              |
|                   | score, policy        |                                                                           |              |
|                   | violations.          |                                                                           |              |
+-------------------+----------------------+---------------------------------------------------------------------------+--------------+
| **Alert & SLO     | Define p95 latency,  | Ops, Security                                                             | Runbook &    |
| Configuration**   | cost per             |                                                                           | alert rules  |
|                   | interaction,         |                                                                           |              |
|                   | violation count      |                                                                           |              |
|                   | SLOs; hook to        |                                                                           |              |
|                   | incident management  |                                                                           |              |
|                   | systems (e.g.        |                                                                           |              |
|                   | PagerDuty/Opsgenie). |                                                                           |              |
+-------------------+----------------------+---------------------------------------------------------------------------+--------------+
| **Drift Detection | Weekly run: eval     | Ops, ML Eng                                                               | Drift        |
| and Re-alignment  | harness on fresh     |                                                                           | report;      |
| Loop**            | data measuring agent |                                                                           | retrain      |
|                   | accuracy, cost and   |                                                                           | tickets      |
|                   | tone on fresh        |                                                                           |              |
|                   | production logs      |                                                                           |              |
|                   | flagging             |                                                                           |              |
|                   | statistically        |                                                                           |              |
|                   | significant          |                                                                           |              |
|                   | degradation (compare |                                                                           |              |
|                   | to baseline;         |                                                                           |              |
|                   | auto-ticket if KPI   |                                                                           |              |
|                   | drop \> accepted     |                                                                           |              |
|                   | threshold)           |                                                                           |              |
+-------------------+----------------------+---------------------------------------------------------------------------+--------------+
| **Kill-Switch and | Quarterly test of    | Ops, Ethics Partner                                                       | Drill report |
| Escalation        | manual and auto      |                                                                           |              |
| Drills**          | shutdown;            |                                                                           |              |
|                   | post-mortem.         |                                                                           |              |
+-------------------+----------------------+---------------------------------------------------------------------------+--------------+
| **Regular Ongoing | Baseline vs live KPI | Product Owner, CFO rep, Steering Committee                                | NorthStar    |
| (e.g. Quarterly)  | gap; ROI update.     |                                                                           | KPIs actual  |
| Value-Realization |                      |                                                                           | vs target    |
| Review**          |                      |                                                                           | trend        |
+-------------------+----------------------+---------------------------------------------------------------------------+--------------+
| **Underlying Base | Governance and       | Simulation/Test Engineer, AgentOps Lead                                   | Model        |
| Model Lifecycle   | tooling              |                                                                           | registry     |
| Management**      | to **version,        |                                                                           | entries      |
|                   | monitor, upgrade, or |                                                                           | (e.g.        |
|                   | deprecate** the      |                                                                           | MLflow)      |
|                   | underlying LLM or    |                                                                           |              |
|                   | fine-tuned           |                                                                           |              |
|                   | checkpoints.         |                                                                           |              |
+-------------------+----------------------+---------------------------------------------------------------------------+--------------+

**Outcome**: Agent in steady-state production with SLOs met, quarterly
ROI verified, and active processes in place for drift re-alignment and
future model upgrades.

## Stage‑Gates

1.  Cost‑to‑Serve Forecast (after Design).

2.  Ethics‑Gate Approval (post Tier‑2/3 Simulation).

3.  Production Go / No‑Go (post Feedback sprint).

**RACI Heat‑Map -- Stage‑Gates**

  -------------------------------------------------------------------------------------------------------------------------------
  ** Gate **             ** Product **   ** CISO **   ** CFO **   ** Process Owner **   ** AgentOps Lead **   ** Exec Sponsor **
  --------------------- --------------- ------------ ----------- --------------------- --------------------- --------------------
  Mission Definition           A             C            I                R                     I                    A

  Cost‑to‑Serve                A             C            A                R                     C                    I

  Ethics Gate                  C             A            I                R                     C                    A

  Prod Go/No‑Go                R             C            A                A                     R                    A
  -------------------------------------------------------------------------------------------------------------------------------

*A=Approver, R=Responsible, C=Consult, I=Inform*

**References & Lineage**

1.  PwC (2024) *Agentic AI: The New Frontier*

2.  McKinsey (2025) COO article on agentic pilots

3.  BCG (2025) *AI Agents as the All‑Stars*

4.  AOSE literature (Wooldridge et al.)

5.  OSS tool communities -- LangChain, CrewAI, AutoGen, agentbench

**Publication & Community Roadmap (appendix)**

*Steps 1‑9 as outlined in prior guidance, including license, repo
structure, CHANGELOG, first community call.*

*End of Playbook v 2.9*
