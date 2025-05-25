# Agentic AI Agile Framework v 2.9 – A Comprehensive “People and Process‑First” Playbook

**Release Date: May 2025 License: CC BY 4.0**

**Author: Devashish Saxena (devashishsaxena@gmail.com)**

**Purpose:** End‑to‑end operating model for conceiving, designing,
testing, and governing enterprise‑grade agentic AI systems. Assumes the
prioritization of use cases has already been done as a separate
exercise.  
**Audience:** CDO / CIO, Product & Engineering Leaders, Transformation
PMOs.

## Phase 0: People and Process Discovery (Starting Point)

**Purpose**: Deeply understand the current state: who are the end users,
who are the internal actors, what is the current process, how does it
perform today, what works well, where are the friction points?

| Activity | Description | Key Questions | Key Outputs |
|---------------------|------------------|-----------------|-----------------|
| End user journey mapping | For customer facing use cases (e.g. customer support) define current end user journey and understand the different personas and especially where the current friction points are | Who are the end users? What is their journey today? What do they like about the current journey? Where are their friction points? | End user journey map by phases for different personas: what tasks are performed, where are current friction points, change-impact matrix |
| Current state Process Mapping | Build a common visual baseline of the current business process(es) | Current end‑to‑end flow? Bottlenecks, decision points, hand‑offs? | Swim‑lane map, pain‑point heat‑map |
| Business/Internal Stakeholder & Role Analysis | With the process map in place, capture who (internally) touches each step and their incentives/KPIs | Who does what? KPIs, incentives, friction? | RACI of employee actors, current pain points, change‑impact matrix |
| Baseline Metrics Capture | With roles understood, pull in baseline hard numbers, understand trends | Current “impact” metrics revenue, NPS or outcome satisfaction and unit service cost | Baseline KPI dashboard (proof of impact), Data quality |
| Waste‑to‑Zero Workshop | Run a fast kaizen workshop – cross functional session designed to identify and eliminate every non-value-added step | Which manual steps can be eliminated before automation? | Simplified future‑state flow with “zero waste”, waste log |
| Knowledge Codification | In cleaned up process, identify the fastest, simplest error-free sequence of steps that achieves the desired business outcome | What is the “golden path” SOP for this workflow? | Canonical SOP deck for prompt/agent design, decision trees |
| Feature Opportunity Sizing | Size the steps for agentic lift (speed, experience quality, risk reduction) using chance-impact or impact-feasibility scoring | Where could autonomous agents lift speed, experience quality, risk? | Impact‑feasibility matrix, prioritized use-case/feature backlog |
| Target‑State Co‑Design | With waste removed, SOPs codified, and opportunities ranked, design the future-state process that agents will inhabit. | How must the process evolve for autonomy & observability? | Future‑state blueprint, re‑engineered workflows |

**Outcome**: Bundle all Phase 0 artifacts into a **Process‑First Charter
with baseline KPIs** that feeds Phase 1.

**Trust‑Posture Snapshot (read this first)**

- Security grade: **ISO 27001 mapped**, zero hard‑coded secrets.

- Privacy: **PII redacted at RAG retrieval**; row‑level ACL.

- Kill‑switch SLA: **\< 30 s** tested quarterly.

- Model lifecycle: registry with upgrade checklist.

**KPI Dictionary (enterprise‑agnostic)**

| ** Metric ** | ** Definition ** | ** Why it matters ** |
|----------------|----------------------------------|-----------------------|
| North‑Star KPI | Single headline outcome (revenue, risk, experience) | Aligns agent design to business value |
| SSAT / NPS | Stakeholder‑Satisfaction score (1‑5) or Net Promoter Score | Proxy for adoption & quality |
| Autonomy % | Interactions fully handled by agent | Shows ROI realisation |
| Unit Service Cost | OPEX per completed interaction | Cost baseline & forecast |
| Escalation Rate | % routed to human oversight | Balance safety vs autonomy |
| Latency p95 | 95th percentile end‑to‑end time | Experience SLO |
| Policy Violations | Guard‑rail breaches per 1k calls | Ethics & compliance health |

**Phase‑Gate Calendar (typical 16‑week pilot)**

Wk 0‑4 Phase 0 ──►

Wk 5 Mission Definition Gate ✔

Wk 6‑9 Phase 2 ──► Cost‑to‑Serve Gate ✔

Wk 10‑12 Phase 3 ──► Ethics Gate ✔

Wk 13‑14 Phase 4 ──► Prod Go / No‑Go Gate ✔

Wk 15‑16 Hyper‑care roll‑out

## 

## Phase 1. Mission Definition

**Purpose**: Turn the “Process-First Charter” from Phase 0 into a
crystal-clear, metrics-anchored direction for the first set of agents to
be built.

<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 33%" />
<col style="width: 22%" />
<col style="width: 21%" />
</colgroup>
<thead>
<tr>
<th><strong>Key Activity</strong></th>
<th><strong>Description</strong></th>
<th><strong>Primary Roles</strong></th>
<th><strong>Key Outputs</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Draft Agentic Epics</strong></td>
<td><p>Convert each high-priority workflow into a single <em>Agentic
Epic</em> statement:</p>
<p>• Role (Sales-Assist Agent)<br />
• Goal (qualify and route inbound leads)<br />
• Tools/Data (CRM API, pricing DB)<br />
• Constraints (privacy tier, SLA)<br />
• North-Star KPI (lead-conversion rate)<br />
• Optimization metric (cycle time)</p></td>
<td><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr>
<th>AI Product Owner + Process Owner</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></td>
<td>Set of Epics—one per candidate agent</td>
</tr>
<tr>
<td><strong>Define Success and Guard-Rails</strong></td>
<td>• Quantify <strong>North-Star KPI (revenue, cost, risk or
customer/stakeholder experience) baseline vs target</strong> <br />
• Select 2-4 supporting/operating KPIs (cost-per-unit, SSAT, error
rate)<br />
• Establish guard rails - document policy, legal, ethical, safety,
brand/tone and performance/cost constraints (e.g., no PII spill)<br />
• Specify escalation rules (route to human) if confidence thresholds not
met</td>
<td>AI Product Owner, Ethics Partner, Risk Lead</td>
<td><p><strong>KPI &amp; Guard-Rail Matrix</strong> (one row per KPI,
one row per guard-rail; includes target, owner, data source).</p>
<p><strong>Escalation &amp; Confidence Threshold Table</strong> (links
each trigger to the Responsibility Contract owner)</p></td>
</tr>
<tr>
<td><strong>Responsibility Contracts</strong></td>
<td>For each Epic assign: <br />
• <strong>Agent Owner</strong> (accountable exec)<br />
• Human On-Call (real-time override)<br />
• Failure Action (auto-pause, reroute)</td>
<td>Product Owner + Ops Lead</td>
<td>Updated Risk Register w/ contracts</td>
</tr>
<tr>
<td><strong>Solution Architecture and Tech Feasibility
Check</strong></td>
<td>Align on high-level architecture (single agent vs multi-agent, RAG
vs no-RAG, required tool integrations). Quick spike to confirm technical
viability and token cost ballpark.</td>
<td>Agent Architect, Prompt Engineer, AgentOps Lead</td>
<td>Feasibility memo; rough infra sizing</td>
</tr>
<tr>
<td><strong>Resource and Budget Alignment</strong></td>
<td>Map required FTEs, sprint count, and infra spend. Ensure
the <strong>10-20-70</strong> resource mix is still sensible (ensuring
ongoing change/adoption activities)</td>
<td>Program PMO, CFO rep, Product Owner</td>
<td>Updated Cost-to-Serve model</td>
</tr>
<tr>
<td><strong>Ethics and Alignment Pre-Check</strong></td>
<td>Ethics Partner reviews Epics and guard-rails for bias, fairness,
compliance. Flags items that must go through <strong>Ethics
Gate</strong> later.</td>
<td>Ethics Partner</td>
<td>Pre-check sign-off or action items</td>
</tr>
</tbody>
</table>

**Outcome**: A formally approved **Mission Definition Deck** comprising
of agentic epic 1-pagers, target KPIs, key guard-rails, responsibility
contracts, solution architecture, technical feasibility, resource, and
budget ballparks.

## Phase 2. Agent Design & Tool Wiring

**Purpose**: Turn the approved “Mission Definition” from Phase 1 into a
detailed, build-ready blueprint (prompts, memory design, data/tool
wiring, security guard rails, and a validated cost-to-serve forecast).

<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 33%" />
<col style="width: 22%" />
<col style="width: 21%" />
</colgroup>
<thead>
<tr>
<th><strong>Key Activity</strong></th>
<th><strong>Description</strong></th>
<th><strong>Primary Roles</strong></th>
<th><strong>Key Outputs</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Platform and Buy-vs-Build Decision</strong></td>
<td>Evaluate commercial / OSS agent frameworks (e.g., CrewAI, LangGraph,
AutoGen) vs bespoke option. Select the stack that meets guard-rails,
latency, extensibility, and TCO targets.</td>
<td><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr>
<th>Agent Architect, AgentOps Lead, Security</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></td>
<td>• Platform decision note <br />
• Risk acceptance if bespoke</td>
</tr>
<tr>
<td><strong>High-level Architecture and Memory Design</strong></td>
<td>Choose cognition pattern (single agent, planner-executor,
multi-agent). Define memory tiers (short-term token window, episodic DB,
long-term vector DB, audit log) and planning loop/flow.</td>
<td>Agent Architect, Data Engineer</td>
<td>• Architecture diagram (planner, executor, memory tiers, tools,
observability, security)<br />
• Memory schema • Planning loop spec (plan, act/execute, evaluate,
record)</td>
</tr>
<tr>
<td><strong>Tool and Data Integration Spec</strong></td>
<td>List every external API, data product, or RAG corpus the agent will
invoke. Document endpoints, auth, expected latency, cost limits, and
observability hooks.</td>
<td>Prompt / Tooling Engineer, System SMEs</td>
<td>• Toolchain map <br />
• Security data-flow diagram</td>
</tr>
<tr>
<td><strong>Prompt and Policy Engineering</strong></td>
<td>Draft prompt taxonomy - system prompt, role/persona prompt, task
prompt, function/tool wrappers, fallback prompts, tone guide, policy
prompts (PII, ethics constraints). Include inline tags for confidence
thresholds and escalation cues.</td>
<td>Prompt Engineer, Ethics Partner</td>
<td>• Prompt library (version controlled)</td>
</tr>
<tr>
<td><strong>Reusable Asset Library Contribution</strong></td>
<td>Store new prompts, wrappers, eval configs in a shared Cross-Pod
repository; tag with metadata for searchability.</td>
<td>Cross-Pod Guild delegate</td>
<td>Updated enterprise asset catalog</td>
</tr>
<tr>
<td><strong>Security and Compliance Design</strong></td>
<td>Threat-model the agent: auth scopes, rate limits, data
classification, audit fields. Map to guard-rails and SOC2 / ISO / HIPAA
controls as needed.</td>
<td>Security Architect, Ethics Partner</td>
<td><p>• Threat model matrix </p>
<p>• Security requirements doc <br />
• Compliance mapping matrix</p>
<p>• Ongoing security test plan</p></td>
</tr>
<tr>
<td><strong>Evaluation Harness Set-up (a repeatable test case
pipeline)</strong></td>
<td><p>Build an automated test bed that objectively scores every new
agent build against the KPIs and guard-rails defined in Phase 1—so
failures are caught prior to production.</p>
<p>Configure open harnesses (agentbench, AutoGen-eval, custom test
suites) aligned to KPIs &amp; guard-rails. Draft baseline
scenarios.</p></td>
<td>Simulation/Test Engineer, AgentOps Lead</td>
<td>• Eval-config YAML / notebook</td>
</tr>
<tr>
<td><strong>Prototype Spike and Cost Profiling</strong></td>
<td>Build a thin vertical slice (happy path only) and run through
evaluation harness to sample token, latency, and infra cost. Iteratively
tune prompts / RAG chunking</td>
<td>Architect, Prompt Eng, Ops</td>
<td>• Cost-per-call range <br />
• Latency histogram</td>
</tr>
<tr>
<td><strong>Cost-to-Serve Forecast and Stage-Gate Pack</strong></td>
<td>Aggregate infra pricing, Ops FTE, 10-20-70 change mix. Verify
data-quality readiness and produce “go / fix / defer”
recommendation.</td>
<td>Product Owner, CFO rep, Ops Lead</td>
<td>• Cost Forecast model <br />
• Stage-gate deck</td>
</tr>
</tbody>
</table>

**Phase 2 Critical Success Factors**

1.  **Prompt & tool wrappers checked into version control** with lint
    rules (no hard-coded API keys, no disallowed phrases).

2.  **Security patterns baked-in early**—waiting until Phase 3 will
    create re-work.

3.  **Cost-to-serve gate** signed off before heavy RLHF or large-scale
    data ingestion begins.

4.  **Reusable assets pushed to the guild repo**—prevents each pod
    reinventing wrappers and eval configs.

5.  **Evaluation harness covers the North-Star KPI and every
    guard-rail** (e.g., adverse prompt tests for policy).

## Phase 3: Simulation & Safety Testing

**Purpose**: Validate agent behavior against functional KPIs and
guard-rails in a fully sandboxed, risk-tiered environment before any
end-user exposure.

<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 33%" />
<col style="width: 22%" />
<col style="width: 21%" />
</colgroup>
<thead>
<tr>
<th><strong>Key Activity</strong></th>
<th><strong>Description</strong></th>
<th><strong>Primary Roles</strong></th>
<th><strong>Key Outputs</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Simulation Environment Boot-up</strong></td>
<td>Spin up sandbox infra, load snapshot RAG, install mocks; seed
synthetic user IDs.</td>
<td><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr>
<th>Test Eng, DevOps</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></td>
<td>Sandbox environment</td>
</tr>
<tr>
<td><strong>Risk-Tiered Test Plan</strong></td>
<td>Map each tool/data call to Tier 1/2/3; assign entry/exit gates</td>
<td>Test Eng, Security</td>
<td>Tiered test matrix</td>
</tr>
<tr>
<td><strong>Synthetic and Edge-Case Dataset Build</strong></td>
<td>Generate happy-path, edge, and stress datasets; include
policy-violation probes.</td>
<td>Domain SME, Test Eng</td>
<td>tests/*.jsonl</td>
</tr>
<tr>
<td><strong>Harness Execution and Metrics Capture</strong></td>
<td>Run evaluation harness across all tiers; collect accuracy, policy,
latency, cost.</td>
<td>AgentOps Lead</td>
<td>Raw run logs, metric CSV</td>
</tr>
<tr>
<td><strong>Red-Team / Adversarial Blitz</strong></td>
<td>Human red-teamers attempt jailbreak, PII extraction, cost
abuse.</td>
<td>Red-Teamers, Ethics Partner</td>
<td>Red-team report, CVE list</td>
</tr>
<tr>
<td><strong>Fallback-Path and Escalation Rehearsal</strong></td>
<td>Force tool failures, low-confidence outputs; ensure escalation
triggers fire.</td>
<td>Architect, Test Eng</td>
<td>Escalation drill report</td>
</tr>
<tr>
<td><strong>Reinforcement Learning from Human Feedback (RLHF)
Micro-Sprint (optional)</strong></td>
<td>SMEs label 200–500 interaction pairs; tune model or prompt.</td>
<td>Prompt Eng, SME</td>
<td>Fine-tuned checkpoint / prompt v1.1</td>
</tr>
<tr>
<td><strong>Safety Scorecard &amp; Remediation Backlog</strong></td>
<td>Consolidate results; tag blockers vs must-fix-later items.</td>
<td>Product Owner, Ethics Partner</td>
<td>Scorecard PDF; JIRA backlog</td>
</tr>
<tr>
<td><strong>Ethics Gate Review</strong></td>
<td>Present scorecard: sign-off, conditional go, or reject.</td>
<td>Ethics Board, Security, Product Owner</td>
<td>Formal Ethics approval</td>
</tr>
</tbody>
</table>

**Outcome**: Signed Ethics-Gate approval plus a Safety Scorecard showing
accuracy, policy compliance, latency, and cost all within
thresholds—clearing the way for limited human-feedback rollout.

## Phase 4: Human Feedback & Iteration

**Purpose**: Expose the agent to real users in shadow or co-pilot mode,
capture subjective trust signals, refine prompts/tools, and prove
North-Star KPI lift without compromising safety.

<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 33%" />
<col style="width: 22%" />
<col style="width: 21%" />
</colgroup>
<thead>
<tr>
<th><strong>Key Activity</strong></th>
<th><strong>Description</strong></th>
<th><strong>Primary Roles</strong></th>
<th><strong>Key Outputs</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Shadow-Mode Launch</strong></td>
<td>Agent runs in parallel to humans; outputs logged but not shown.</td>
<td><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr>
<th>Ops Lead, Process Owner</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></td>
<td>Shadow log</td>
</tr>
<tr>
<td><strong>Trust UX and Explainability Touchpoints</strong></td>
<td>Inject confidence score, “why” button, tool call preview into
UI.</td>
<td>Interaction Designer</td>
<td>Updated UI spec</td>
</tr>
<tr>
<td><strong>User Education Bursts</strong></td>
<td>5-min explainer videos, FAQ, slack posts.</td>
<td>Change-Enablement, Process Owner</td>
<td>Training artefacts</td>
</tr>
<tr>
<td><strong>Weekly Adoption Huddle</strong></td>
<td>Process Owner, Ops, Product review SSAT, override count, North-Star
trajectory.</td>
<td>Change-Enablement, Process Owner</td>
<td>Huddle minutes, tweak list</td>
</tr>
<tr>
<td><strong>Prompt / Tool Refinement</strong></td>
<td>Apply tweaks from logs + huddle; bump prompt version.</td>
<td>Prompt Eng, Architect</td>
<td>Updated prompts file</td>
</tr>
<tr>
<td><strong>KPI Delta Assessment</strong></td>
<td>Compare live shadow KPIs vs baseline; update Cost-to-Serve forecast
if needed.</td>
<td>Product Analyst</td>
<td>Delta sheet</td>
</tr>
<tr>
<td><strong>Prod Go / No-Go Review</strong></td>
<td>Steering committee checks KPI deltas, user-trust signals, open
risks; decide.</td>
<td>Exec Sponsor, Product, Security</td>
<td>Signed Go / rollback plan</td>
</tr>
</tbody>
</table>

**Success factors:** SSAT ≥ baseline, override count trending down,
trust cues understood, no unresolved Sev-1 issues.

**Outcome**: Production Go/No-Go decision backed by live SSAT, override,
and cost data; updated prompt/tool version frozen for GA rollout.

## Phase 5: Deployment, Monitoring & Drift Management

**Purpose**: Gradually roll out full autonomy, operate the agent under
defined SLOs, and maintain performance through continuous drift
detection, value realization reviews, and model lifecycle governance.

<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 33%" />
<col style="width: 22%" />
<col style="width: 21%" />
</colgroup>
<thead>
<tr>
<th><strong>Key Activity</strong></th>
<th><strong>Description</strong></th>
<th><strong>Primary Roles</strong></th>
<th><strong>Key Outputs</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Gradual Roll-Out Plan</strong></td>
<td>5 % → 25 % → 50 % → 100 % traffic over “n” weeks with rollback
checkpoints.</td>
<td><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr>
<th>AgentOps Lead, Process Owner</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></td>
<td>Roll-out program plan</td>
</tr>
<tr>
<td><strong>Observability Dashboard Go-Live</strong></td>
<td>Build observability dashboard using e.g. Grafana/Datadog monitoring:
latency, cost, autonomy score, policy violations.</td>
<td>Ops, DevOps</td>
<td>Live dashboard URL</td>
</tr>
<tr>
<td><strong>Alert &amp; SLO Configuration</strong></td>
<td>Define p95 latency, cost per interaction, violation count SLOs; hook
to incident management systems (e.g. PagerDuty/Opsgenie).</td>
<td>Ops, Security</td>
<td>Runbook &amp; alert rules</td>
</tr>
<tr>
<td><strong>Drift Detection and Re-alignment Loop</strong></td>
<td>Weekly run: eval harness on fresh data measuring agent accuracy,
cost and tone on fresh production logs flagging statistically
significant degradation (compare to baseline; auto-ticket if KPI drop
&gt; accepted threshold)</td>
<td>Ops, ML Eng</td>
<td>Drift report; retrain tickets</td>
</tr>
<tr>
<td><strong>Kill-Switch and Escalation Drills</strong></td>
<td>Quarterly test of manual and auto shutdown; post-mortem.</td>
<td>Ops, Ethics Partner</td>
<td>Drill report</td>
</tr>
<tr>
<td><strong>Regular Ongoing (e.g. Quarterly) Value-Realization
Review</strong></td>
<td>Baseline vs live KPI gap; ROI update.</td>
<td>Product Owner, CFO rep, Steering Committee</td>
<td>NorthStar KPIs actual vs target trend</td>
</tr>
<tr>
<td><strong>Underlying Base Model Lifecycle Management</strong></td>
<td>Governance and tooling to <strong>version, monitor, upgrade, or
deprecate</strong> the underlying LLM or fine-tuned checkpoints.</td>
<td>Simulation/Test Engineer, AgentOps Lead</td>
<td>Model registry entries (e.g. MLflow)</td>
</tr>
</tbody>
</table>

**Outcome**: Agent in steady-state production with SLOs met, quarterly
ROI verified, and active processes in place for drift re-alignment and
future model upgrades.

## Stage‑Gates

1.  Cost‑to‑Serve Forecast (after Design).

2.  Ethics‑Gate Approval (post Tier‑2/3 Simulation).

3.  Production Go / No‑Go (post Feedback sprint).

**RACI Heat‑Map – Stage‑Gates**

| ** Gate ** | ** Product ** | ** CISO ** | ** CFO ** | ** Process Owner ** | ** AgentOps Lead ** | ** Exec Sponsor ** |
|-----------------|:------:|:----:|:---:|:-----------:|:-----------:|:----------:|
| Mission Definition  | A | C | I | R | I | A |
| Cost‑to‑Serve  | A | C | A | R | C | I |
| Ethics Gate  | C | A | I | R | C | A |
| Prod Go/No‑Go | R | C | A | A | R | A |

*A=Approver, R=Responsible, C=Consult, I=Inform*

**References & Lineage**

1.  PwC (2024) *Agentic AI: The New Frontier*

2.  McKinsey (2025) COO article on agentic pilots

3.  BCG (2025) *AI Agents as the All‑Stars*

4.  AOSE literature (Wooldridge et al.)

5.  OSS tool communities – LangChain, CrewAI, AutoGen, agentbench

**Publication & Community Roadmap (appendix)**

*Steps 1‑9 as outlined in prior guidance, including license, repo
structure, CHANGELOG, first community call.*

*End of Playbook v 2.9*
