# AI Transformation Decision Model — Solution Ladder & Value Categories

> Ready to paste into Notion → **Zipcio AI Knowledge Base & Control Center → Methods & Playbooks**.
> Blocked on 2026-09-08 by the workspace free-block limit. Set the properties below on the new row.

## Database properties to set

| Property | Value |
| --- | --- |
| Title | AI Transformation Decision Model — Solution Ladder & Value Categories |
| Category | AI Method |
| Output Format | Method |
| Status | **Approved** |
| Visibility | Internal-only |
| Owner | Matt McNulty |
| Version | 1.0 |
| Confidence Threshold | High |
| Last Reviewed | 2026-09-08 |
| Applicable Stage | Discovery, Scoping, Implementation, Optimization |
| Tool Compatibility | Claude, ChatGPT |
| Use Case | Deciding what Zipcio should actually build for a client, and whether AI belongs in the solution at all. Applies to any request where a solution shape has not yet been settled — audits, scoping conversations, architecture recommendations, and AI opportunity identification. |
| Input Requirements | The business objective stated in one sentence; the current operating process; the state of the data and system foundation; the nature of the work (deterministic vs. language/judgment vs. analysis at volume); and the volume or frequency that would justify a build. |
| Escalation Rule | Escalate to the account lead when the recommendation is to decline AI but the client is pushing for it; when the honest answer is to sequence foundation work first and that moves a client-visible date; or when the solution shape carries commercial implications (scope, hours, pricing). |
| Source Links | Surfaced operationally at https://onboarding-sa-ai.vercel.app (Judgment section). Related: SA Training — Zipcio Skill Suite + MCP Operating Model; Zipcio AI Skill Suite — Field Guide. |
| Notes | Approved as a canonical operating standard by Matt McNulty on 2026-09-08. Created to close a documentation gap surfaced while building the AI Transformation SA onboarding microsite: the model was in active use and taught to new SAs but had no canonical record. Visibility set to Internal-only pending a review for client-facing use — the ladder and value categories are presentable to clients, but they also encode how Zipcio decides what to sell and build. |

---

## Page content

> **Approved operating standard.** This is how Zipcio decides what to build. Use it as canonical, not as shorthand.

### Why this exists

Zipcio is an AI-forward practice, which is exactly why **AI is not the default answer**. A client who buys an LLM workflow to paper over a broken process has bought a faster version of the wrong thing, and they will eventually notice. The discipline is to work down the ladder and stop at the first rung that actually solves the problem.

Recommending *against* AI, when a process change or native platform capability is stronger, is a senior move and should be said out loud rather than quietly not proposed.

### The solution ladder

Work these in order. Do not skip a rung because a lower one is more interesting to build.

1. **Business objective.** What outcome is the client actually trying to move — revenue, cycle time, conversion, retention, cost, risk? If this cannot be stated in one sentence, nothing below it is designable. Go back and get it.
2. **Operating process.** What the humans do, in what order, with what handoffs. A large share of what looks like a systems problem is a process that was never agreed. Fixing the process is often the cheapest and most durable intervention available.
3. **Data and system foundation.** Object model, properties, associations, pipeline design, data quality. Automation built on a foundation that cannot represent the business will encode the confusion rather than remove it.
4. **Automation.** Native platform capability first — workflows, routing, calculated fields, lifecycle logic. Deterministic, inspectable, and supportable by the client's own team after we leave.
5. **AI, where it genuinely earns its place.** Reach here when the work requires judgment, language, classification, synthesis, or analysis that deterministic logic cannot express — not when it would merely be impressive.

### The solution might legitimately be any of these

Process change (no build at all) · CRM architecture · native platform functionality · workflow automation · integration · custom code · LLM workflow · Claude Skill · Custom GPT · analysis layer · agent · microsite or app · **a combination, which is usually the real answer**.

### The three AI value categories

AI value is claimed in one of three categories. Name which one applies, and be honest about the size of it.

| Category | What it means | Where it goes wrong |
| --- | --- | --- |
| **Time** | Reduce human effort or latency — the same output, materially faster or with materially less person-time. | Easiest to justify and easiest to overclaim. If the manual version takes eleven minutes a week, the automation is a hobby, not a solution. |
| **Accuracy** | Improve consistency, classification, analysis, or decision quality — the output is *better*, not just faster. | Often more valuable than time savings and consistently harder to sell, because the current error rate is usually invisible to the client. |
| **New capability** | Make something possible that was not — work that could not be done at all at a defensible cost. | Where the largest commercial arguments live. Requires evidence that the new thing changes a decision or a behaviour. |

**The strongest solutions combine categories.** A solution that saves time *and* raises accuracy *and* opens a capability the client did not have is not three small wins — it is the shape of the work worth productizing.

### The test sequence

Run in order. Any answer in the right-hand column stops the process and becomes the recommendation.

1. Is the business objective stated in one sentence? → If not: **not yet.** Get the objective defined. Building against an undefined objective is how a project becomes unfalsifiable.
2. Would fixing the process or using native platform capability solve it? → If yes: **recommend that instead.** Cheaper, deterministic, inspectable, client-supportable.
3. Can the data foundation represent the business accurately today? → If no: **fix the foundation first**, and say plainly what that means for the timeline.
4. What does the work actually require? → If deterministic rules: **automation, not AI.** Using a model where a rule would do adds cost, variance, and a support burden nobody asked for.
5. Does the volume or frequency justify a build? → If marginal: **probably not worth building.** Note it as a candidate if volume grows and solve the immediate case by hand.
6. Otherwise: **AI is warranted.** Now specify the shape, and state what you would explicitly *not* build — that is the part that makes the recommendation credible.

### Standing rules

- Deterministic beats probabilistic wherever it can do the job.
- Native platform capability beats custom wherever it can do the job — the client already paid for it and their team can support it.
- Every AI recommendation names its value category and its scale.
- Every AI recommendation names what it will not do.
- "The client asked for AI" is not a reason. Their objective is the reason.

### Change log

| Version | Date | Change |
| --- | --- | --- |
| 1.0 | 2026-09-08 | Approved as canonical. First written record of a model already in active use. |
