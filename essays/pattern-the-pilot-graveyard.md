# The Pilot Graveyard

**Category:** Deciding
**Wardley Stage:** Custom (pilots exist but haven't evolved into production capabilities)

## Forces

Five tensions hold the graveyard in place:

- **Pressure to demonstrate innovation vs. no path to production.** Board decks need AI slides. Competitors are announcing pilots. The CEO read something on a flight. The pressure is real — but it demands launches, not landings. There is no equivalent pressure to get a pilot into production.
- **Enthusiastic technologists vs. disconnected operations.** Pilot teams are composed of people who want to build interesting things. The operations teams who would actually run the thing in steady state are rarely involved until too late — if at all.
- **Vague success criteria vs. the need for clear decisions.** "Prove AI works" is not a success criterion. But defining real criteria means committing to a standard the pilot might fail against, and nobody wants to set themselves up for that.
- **Portfolio breadth vs. resource depth.** Starting twelve pilots feels like progress. In practice it means twelve half-staffed efforts competing for the same data engineers, none with enough momentum to reach production.
- **Innovation theatre vs. value delivery.** The organisation points to the number of active pilots as evidence of AI progress. The number is rising. Nothing is shipping.

## Context

You encounter this pattern in organisations that have 3–10 AI pilots or proofs of concept running simultaneously. Some have been running for six months or longer. None are in production. Leadership is frustrated, asking the same question every quarterly review: "When will the pilots go live?" The answer is always "soon," qualified with caveats about data quality, model accuracy, or integration complexity. Teams are demoralised — they know the work is stalling but have no mandate to change course. The organisation points to the number of active pilots as evidence of progress.

## Problem

Pilots are started to prove that AI "works" rather than to solve a specific business problem with measurable outcomes. There is no scaling criteria defined at the outset — no agreement on what "good enough" looks like, no production pathway, no ops handover plan, no capacity planning for the team that will own it in steady state. Pilots become science projects: interesting to the people working on them, invisible to the business units that were supposed to benefit.

The organisation confuses the number of pilots with progress. A portfolio of twelve pilots sounds impressive in a strategy deck. In practice, it means fragmented effort across too many fronts — every pilot under-resourced, none with enough momentum to reach production, and all of them slowly eroding confidence that AI can deliver anything real.

Meanwhile, the best people start leaving. They joined to build things, not to demo prototypes to steering committees.

## Solution

Triage ruthlessly. Take the full inventory of active pilots and evaluate each one against three dimensions using the [[AI Use Case Canvas]]: business value (is there a quantified problem worth solving?), technical feasibility (can this actually work with the data and infrastructure you have today?), and scaling readiness (is there an operational owner, a production pathway, and a maintenance plan?).

Kill the bottom half. Not "pause" — kill. Hold a formal stopping ceremony for each retired pilot. Name what was learnt. Thank the team publicly. Redeploy them to the survivors. This matters: without a clear ending, killed pilots linger as zombie projects that still consume attention.

For the surviving pilots, apply the [[Scaling Readiness Checklist]]. Identify the specific gaps between current state and production readiness. Assign an operational owner from the business — not from the data science team. Set a hard deadline: production or kill within eight weeks.

Before starting any new pilot, require a completed [[AI Use Case Canvas]] with sign-off from both the sponsoring business unit and the operational team that will own the solution. If nobody in the business will commit to owning it in production, it does not get started.

## Evidence

You know the intervention is working when:

- At least one pilot reaches production within eight weeks of triage.
- New pilots are only initiated with a completed Use Case Canvas and an identified operational owner.
- "Number of pilots" disappears as a success metric in leadership reporting, replaced by "pilots in production" or "business outcomes delivered."
- Teams can articulate the business case for their pilot in terms of the problem being solved and the value at stake, without leading with the technology.
- Stopping ceremonies become unremarkable — the organisation treats killing a pilot as a healthy discipline, not a failure.

## Anti-patterns

- **"Start more pilots to increase our chances."** This is the lottery fallacy applied to innovation. More pilots with the same structural problems just means more waste.
- **"The technology just needs more time."** If the pilot has been running for six months without a production date, time is not the constraint. Clarity is.
- **"Let's build an AI platform first and then the pilots will scale."** This is the [[The Platform Before Product]] trap. Platforms built without production workloads to serve become expensive shelfware.
- **"We need to hire more data scientists."** You do not have a talent problem. You have a direction problem. More data scientists without production pathways just means more pilots.
- **"Let's rebrand the POC as a 'Phase 1'."** Renaming does not change the underlying dynamic. If there is no Phase 2 plan with dates, owners, and budget, Phase 1 is just a pilot with better branding.

## Related Patterns

- [[The Fog of AI]] — organisations in the Fog often start pilots as a way to "figure out AI," which feeds the Graveyard.
- [[The Governance Bottleneck]] — pilots that die in governance queues contribute to the graveyard. Faster governance gives pilots a chance to reach production.
- [[The Metrics Mirage]] — pilots without clear success criteria are particularly susceptible to vanity metrics that obscure the lack of progress.
- [[The Scaling Cliff]] — pilots that succeed but can't scale end up back in the graveyard. Scaling readiness should be defined at pilot inception.
- [[The Platform Before Product]] — a common escape route from Graveyard conversations that creates a different but equally expensive problem.

## Tools

- [[AI Use Case Canvas]]
- [[Scaling Readiness Checklist]]
