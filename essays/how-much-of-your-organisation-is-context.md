# How Much of Your Organisation is Context?

**Platform:** LinkedIn article
**Status:** Draft
**Source notes:** [[The Metadata Layer - Enterprise Context Graphs]]

---

## The Article

How Much of Your Organisation is Context?

Martin Casado of a16z recently posed a question that the entire AI industry is wrestling with: does AI lead to infinite fragmentation (many specialised companies win) or oligopoly (a few frontier models consume everything)?

Swaroop Jagadish offered a compelling answer: regardless of which future materialises, the metadata layer endures. Enterprise AI agents need contextual understanding — data lineage, ownership, governance rules — that no foundation model can replicate on its own.

He called context graphs the "connective tissue" of AI-era organisations.

I think he's right. But I also think we massively underestimate how much of an organisation is connective tissue.

---

In biology, when people hear "connective tissue," they think tendons and ligaments. The obvious stuff. But connective tissue also includes bone, fat, and blood. It's not a minor structural component — it's the majority of what holds a body together.

Organisations are the same.

The obvious context is the documented stuff. Org charts. Data dictionaries. Governance rules. Metric definitions. That's the tendons and ligaments — visible, well-understood, and what most "context graph" products are built to capture.

But the real context? The kind that makes a 10-year employee invaluable? That's the rest of the connective tissue.

---

**Bone — structural, load-bearing, invisible.**

Decision archaeology. Not *what* was decided, but *why*. The rejected alternatives. The political trade-offs. The "we tried that in 2019 and it failed because the VP of Sales vetoed it."

Real ownership — who actually owns what, versus the RACI chart. Real approval chains — versus the documented ones. Which systems are untouchable and why (usually a person, not a technical reason).

This is the structural context that bears weight every single day but is almost never written down.

**Fat — stored energy, looks like waste, but is essential.**

The people who "don't do much" but are the ones everyone calls when something breaks. Tribal customer knowledge that never makes it into the CRM: "They always threaten to leave in Q4 but never do."

Informal networks — Slack DMs, coffee chats, the smoking area — where information actually moves. Institutional taste — why this company builds things *this way* and not that way. It's never documented because nobody thinks it needs to be.

This is the context that looks like inefficiency from the outside but is actually stored organisational intelligence.

**Blood — circulation, connecting everything, carrying signals.**

How information actually flows through the organisation. Not the org chart — the reality. The translation layers: people who speak both "business" and "tech" and broker meaning between teams.

Implicit feedback loops: "When this metric drops, that team panics, so we preempt by adjusting our release schedule." Emotional context: which teams trust each other, which ones have history, where the scar tissue is.

This is the context that keeps the organisation alive and responsive. Remove it and everything stops, even if every system is still technically running.

---

Here's the uncomfortable implication:

An AI agent with access to every document, dashboard, and database in your organisation still can't operate like a 10-year employee. Because it's missing all of this. And most of it was never written down because humans carry it unconsciously.

Like connective tissue, you don't notice it until it's injured.

---

The irony is that one company may already have more organisational context than anyone realises — and it isn't a metadata startup.

Salesforce spent $8 billion acquiring Informatica last November. Their framing was explicit: "Models are incredibly intelligent, but they tend to be corporate stupid."

But the Informatica deal isn't even the interesting part. The interesting part is what Salesforce already had.

Think about what sits in Salesforce across most enterprises: customer relationships, transaction histories, account hierarchies, opportunity records, support tickets, approval chains, escalation rules, workflow logic. Every custom field a company ever created is a piece of organisational context that someone externalised into the platform. Every validation rule captures business logic that once lived only in someone's head.

That's not metadata about data. That's 20 years of companies encoding their bone and fat into a system — without calling it a context graph.

Informatica extends this beyond CRM — master data management, lineage, governance across ERP, warehouses, and other systems. MuleSoft provides the real-time integration. Together, Salesforce is arguing they already own the context layer. They just needed to connect it.

The pure-play metadata companies — DataHub, Atlan, Alation — are building context graphs about data assets. Salesforce is sitting on a context graph about how organisations actually work. Those are very different things.

Which raises a question for every enterprise: is your most valuable context already captured somewhere you haven't thought to look?

---

But even Salesforce can't capture everything. There's a deeper tension here that nobody in the context graph space is talking about openly.

The most valuable organisational context is exactly the stuff organisations *can't* systematically capture — and arguably *shouldn't*.

Public Slack channels, Jira tickets, decision logs, code reviews — these are fair game. Meeting transcripts are increasingly captured with consent. But the richest context lives in private DMs, in hallway conversations, in the instinct a veteran has about which battles to pick.

You could mine email. You could surveil Slack DMs. You could map calendar patterns to infer who really influences whom. Companies legally can do all of this.

But the moment you do, you destroy the very trust that produces the context you're trying to capture. People stop being candid in writing. The smoking area conversation doesn't stop — it just moves somewhere you can't hear it.

This is the privacy paradox of context graphs: the most valuable organisational knowledge is the kind you can't ethically capture at scale.

---

I think the resolution is a shift in framing.

The context graph doesn't need to capture private communications. It needs to capture the *outputs* — the decisions, the patterns, the documented rationale. The challenge isn't surveillance. It's building a culture where people externalise their reasoning.

That's a fundamentally different problem. It's not a technology problem. It's an organisational design problem.

The companies that figure this out — that build cultures where context naturally flows into shared, structured, machine-readable form — will have a genuine competitive advantage. Not because they have better AI. Because they have better context.

And context is the one thing you can't replicate by training a bigger model.

---

*Inspired by Swaroop Jagadish's post on the enterprise context graph and the Latent Space podcast with Martin Casado and Sarah Wang of a16z.*

---

## Publishing Notes

- **Hook:** Opens with a16z credibility + a question, then pivots to the biological metaphor
- **Structure:** Metaphor framework (bone/fat/blood) → Salesforce as hidden context graph → privacy paradox → resolution
- **CTA implicit:** Positions author as someone who thinks at the intersection of AI, enterprise, and org design
- **Tags:** #AI #EnterpriseAI #DataStrategy #OrganisationalDesign #ContextEngineering #Salesforce #Agentforce
- **Mention/tag:** Swaroop Jagadish, Martin Casado (optional), Latent Space
- **Length:** ~1,200 words — still within LinkedIn article range
