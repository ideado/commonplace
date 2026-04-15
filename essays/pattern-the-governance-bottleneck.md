# The Governance Bottleneck

**Category:** Deciding
**Wardley Stage:** Custom (governance exists but hasn't evolved to fit AI-shaped work)

## Forces

Four tensions create the bottleneck:

- **Need for oversight vs. speed of AI deployment.** AI capabilities can be deployed in days. Governance review processes were designed for quarterly software releases. The mismatch means either governance is bypassed (risk) or deployment stalls (opportunity cost). Both outcomes are bad.
- **Existing frameworks vs. novel risks.** IT governance, change management, data governance — these frameworks exist and work for traditional technology. AI breaks their assumptions. Change management assumes a human made the change. Data governance assumes data flows are predictable. Access control assumes a human holds the credential. Nobody has rebuilt the frameworks for agent-shaped work.
- **Compliance rigour vs. innovation velocity.** Regulated industries face this most acutely. The compliance team needs to understand what the AI does, how it decides, and what data it touches — and they need that in writing, reviewed, and signed off. The AI team needs to iterate, retrain, and redeploy weekly. These cadences are incompatible.
- **Centralised control vs. distributed experimentation.** A centralised governance body that approves all AI initiatives creates a single point of failure. A distributed model where every team governs their own AI usage creates inconsistency and risk. Neither extreme works.

## Context

You encounter this pattern when the organisation has moved past initial experimentation and is trying to scale AI deployment — but the approval process has become the binding constraint.

Typical signals:

- AI initiatives sit in a review queue for weeks or months. The governance committee meets monthly and has a backlog.
- Teams have stopped submitting requests because the process takes too long. They either don't deploy or deploy without approval (feeding the [[Shadow AI Archipelago]]).
- The governance framework is a 40-page document that nobody has read, written by the compliance team without input from the AI team.
- Every AI deployment triggers a full risk assessment designed for enterprise software releases — regardless of whether the deployment is a customer-facing agent or an internal productivity tool.
- The word "governance" has become synonymous with "no" in the minds of the AI team.

## Problem

The governance process is optimised for thoroughness, not speed. It was designed for a world where technology changes were large, infrequent, and high-risk. AI deployment is small, frequent, and variable-risk. Applying the same governance process to a customer-facing autonomous agent and an internal summarisation tool is like requiring the same safety inspection for a commercial aircraft and a bicycle.

The bottleneck creates three downstream problems:

**1. Deployment paralysis.** Good AI initiatives die in the queue. By the time they're approved, the model has been superseded, the business need has shifted, or the team has been reassigned. The governance process doesn't just slow things down — it kills things.

**2. Shadow governance.** When the official process is too slow, teams create informal workarounds. A manager signs off on a deployment that should have gone through the committee. An engineer deploys a copilot and plans to submit the paperwork afterwards. These workarounds are individually rational and collectively dangerous — they mean the organisation has lost visibility of what's actually deployed.

**3. Adversarial relationship between governance and delivery.** The governance team sees themselves as the last line of defence against reckless deployment. The delivery team sees governance as an obstacle to progress. Both positions harden over time. The governance team adds more requirements. The delivery team finds more workarounds. Trust erodes in both directions.

## Solution

Replace the one-size-fits-all governance gate with a tiered, risk-proportionate process.

**Step 1: Classify AI deployments into three tiers.**

| Tier | Risk profile | Examples | Governance process |
|------|-------------|----------|-------------------|
| **Tier 1 — Low risk** | Internal use only, no sensitive data, human reviews all output | Internal meeting summariser, document search tool, code suggestion (with human review) | Team-level approval. Self-certification against a checklist. No committee review. Deploy within one week. |
| **Tier 2 — Medium risk** | Customer-adjacent or uses sensitive data, but human remains in the loop | Customer service draft responses (human sends), internal analytics on HR data, financial report generation (human validates) | Lightweight review by a designated AI governance lead (not the full committee). Standard checklist plus a one-page risk assessment. Approve within two weeks. |
| **Tier 3 — High risk** | Customer-facing autonomous action, regulated data, financial decisions, safety-critical | Autonomous customer communication, automated trading decisions, clinical decision support, autonomous agent with external access | Full governance review. Risk assessment, compliance review, trust-level assignment (see [[The Agent Trust Gap]]). Approve within four weeks — but this is the ceiling, not the average. |

**Step 2: Create a one-page governance artefact per deployment.**

Replace the 40-page policy document with a one-page template for each AI capability:
- What does it do? (two sentences)
- What data does it access? (list)
- Who uses the output? (internal / customer-adjacent / customer-facing)
- What trust level is it operating at? (Inform / Suggest / Act-and-Report / Act-Autonomously)
- What are the rollback triggers? (specific, measurable conditions)
- Who owns it in steady state? (name, not team)

This artefact lives where the team can find it — not in a SharePoint archive.

**Step 3: Appoint an AI governance lead, not a committee.**

A single named individual who can make Tier 2 decisions without convening a meeting. They attend the delivery team's standups, not the other way around. They understand both the risk and the opportunity. Their job is to enable safe deployment, not to prevent deployment.

The full governance committee still exists for Tier 3 decisions, but it meets fortnightly (not monthly) and has a standing agenda slot for AI reviews so teams don't wait for a "special session."

**Step 4: Measure governance speed alongside governance rigour.**

Track two metrics:
- **Time from submission to decision** — for each tier. If Tier 1 decisions are taking more than a week, the process is broken.
- **Deployments that bypassed governance** — if this number is rising, the process is too slow and teams are routing around it. This is a leading indicator of governance failure.

## Evidence

- Tier 1 deployments go live within one week of request. No queue.
- Tier 2 deployments go live within two weeks. The governance lead is embedded enough in delivery that reviews happen in flow, not as a separate gate.
- Tier 3 deployments have a clear, predictable timeline. Teams know what's required and don't treat the process as adversarial.
- The number of deployments bypassing governance drops to near zero — because the official process is faster than the workaround.
- The governance team and the delivery team describe each other as allies, not obstacles.

## Anti-patterns

- **"We need a comprehensive AI policy before anyone can deploy anything."** A comprehensive policy written before you understand your deployment landscape will be wrong in the details and right only in the generalities. Start with the tiered checklist. Write the comprehensive policy after you've run through 20 deployments and know what actually matters.
- **"Every AI deployment needs a full risk assessment."** This is the core of the bottleneck. A full risk assessment for an internal meeting summariser is governance theatre. It doesn't reduce risk — it consumes resources and creates delay.
- **"We'll set up an AI Ethics Board."** Ethics boards are valuable for Tier 3 decisions. For Tier 1 and 2, they are a bottleneck by design. Don't route everything through a body designed for the hardest decisions.
- **"The governance process is fine — teams just need to plan better."** If teams are consistently failing to plan for a six-week governance review, the problem is the six-week review, not the planning.
- **"We can't move faster without increasing risk."** Risk-proportionate governance moves faster for low-risk deployments and maintains rigour for high-risk ones. Speed and safety are not in opposition when the process is tiered appropriately.

## Related Patterns

- [[The Agent Trust Gap]] — the trust level framework provides the vocabulary for governance decisions. Tier assignment should align with trust levels.
- [[Shadow AI Archipelago]] — the archipelago is what grows when governance is too slow. Fixing the bottleneck is the most effective way to reduce shadow AI.
- [[The Pilot Graveyard]] — pilots that die in governance queues contribute to the graveyard. Faster governance gives pilots a chance to reach production.

## Tools

- [[AI Governance Scaffold]] — the one-page governance artefact template for each AI capability.
- [[Trust Calibration Framework]] — trust levels inform the governance tier assignment.
