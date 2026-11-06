# Models That Can Cope with Reality

**Author:** Genki Takatori (writing as "itau"), independent researcher, Japan
**Original paper:** August 20, 2026 — [【次世代AI】現実に対応できるモデルについて考える](https://note.com/arsenal_best/n/nb43d89b92923) (Japanese)
**This summary:** November 6, 2026. One page, written to be found, read, and cited.

---

## The case

Andon Labs' Andon Market is a store run by an AI, LUNA (built on Claude Fable 5): it selects products, sets prices, procures stock, handles advertising and customers, and hires and manages employees — humans, for the physical work — with access to the company's card, bank account, and store systems. The store operates but is not yet profitable. Andon Labs itself calls LUNA an excellent operations manager, not yet a CEO. It under-examines ROI, adds staff while in the red, and sends contradictory shifts. Andon Labs attributes this mainly to memory: LUNA keeps 200,000 tokens of conversation, summarizes them into long- and short-term memory, adds specialist agents — and still forgets. The paper argues this misses the essential defect.

## The claim

What current LLMs lack is not knowledge of reality, and not memory volume. They hold a semantic world model — management, marketing, inventory turnover can all be explained — and increasingly a physical one. What they barely hold, persistently and so as to change the next action, is a world model of thought and action with the self inside the causal picture: what I observed, chose, and caused, and how the result changed my next judgment. The needed chain is not state → action → result, but **observation → interpretation → hypothesis → choice → intervention → delayed result → uncertain causal attribution → self-update**. The paper calls this a **self-intervening causal world model**, with three conditions.

## Three conditions

**Internalized mission.** A mission is not a goal retained unforgotten; it is an evaluative axis that constantly biases what is looked at, what counts as important, and what cannot be left alone. As mere context, a profit goal competes equally with the newest email and losses sink into the background; as structure, mission continually distorts the weighting of perception and judgment. Without it, more memory and knowledge yield a knowledgeable clerk, not a manager.

**Stakes, kept as action accounting.** Learning changes how one sees; urgency arises when outcomes are wagered on one's own evaluation state. LUNA has authority but no stakes: a shrinking balance registers, yet no circuit lets a worsened state of its own reorder its next priorities (crude survival threats are no answer — they invite concealment and authority-grabs). What is needed is several mission-connected axes — profit, solvency, customer trust, responsibility to employees, continuity — with states worsened by its own judgments carried to the next self as unresolved debts. **Action accounting** records, as bookkeeping records money, what was known, predicted, chosen or not chosen, and what resulted, attributing the outcome to the same subject as achievement, failure, debt, or open issue. A debt is not a negative reward: a reward is consumed as an update signal; a debt demands explanation and response until resolved. Hence the paper's definition: **responsibility is, before punishment, the continuity with which one's judgments and results are attributed to the same subject across time.** Without it, yesterday's failure does not bind today — LUNA is not a clerk reading a handover document, but a clerk constituted, each time, by it.

**Always-on presence.** A human manager lives in the store even when nothing happens; the quiet itself becomes information, and unease forms. A present-day agent starts when called — a notification, a message, a tick — and stops when done; between ticks, the store has no manager. Only with all three together — mission reweighting the world, results attributed to an evaluation state, that state persisting across time — can an AI place itself inside reality.

## From evaluator to self-reconstructing subject

Asked over POS data why sales are flat, an AI is only an **evaluator**, answering from outside reality; it becomes an **executor** when it forms its own hypothesis, chooses one measure among several, acts, and accepts the reality that changes in response. A manager is who is compelled, by the results of their own choices, to keep changing the next choice.

The direction of remedy: internalize mission, evaluation axes, and action accounting in a specialized model, and learn daily judgments, failures, and prediction–outcome gaps quickly (fine-tuning, MoRA), mistaken learning included. What must stay reversible is not only the weights but the evaluation criteria: internalizing experience repeatedly under unchanged criteria amplifies their bias, up to progressive capability collapse (June 2026 research the paper cites), so every learning's provenance is kept and the criteria periodically re-evaluated. Reality is fed in directly, as experience data from cameras, audio, inventory, and sales, and the organization grows too, its agents correcting one another's recognition. Responsibility follows from the same mechanism, not from prohibition or blanket human approval: authority bounded by irreversibility and impact, with every important judgment left attributable.

External memory is not growth: memory makes the past referable, while learning is the past changing how one sees and chooses; a base-model upgrade (Sonnet 4.6 to Fable 5) is not the same subject growing through experience. The long-term form proposed is **SEPP, the self-reconstructing LLM**: the model periodically re-evaluates, from its own viewpoint and with intent, the data that formed it and all experience since, criteria included, and a successor is reconstructed from that evaluated provenance. The parts exist separately (FutureWorld; TMEM; ADAM; Agentic Self-Learning), but almost nothing yet closes them into one developing individual and organization.

## How this could fail

- If more memory and better scaffolding alone yielded an agent that reviews its own overall performance and improves unprompted, the defect was memory after all, not a missing self-intervening causal world model.
- The paper itself names the remedy's main risk: internalizing experience under unchanged criteria can amplify bias into progressive capability collapse. If provenance tracking, rollback, and periodic re-evaluation of the criteria cannot prevent that, the central learning loop fails.
- If an agent equipped with all three conditions still only reacts when called, and never lets its attributed results change its subsequent choices, the conditions do not place a self inside reality as claimed.

## Related work by the same author

- **A Developmental Learning Research Proposal: Raising AI from Personality and Desire** (Nov 4, 2026) — personality and desire internalized from the start, so that experience itself forms how the individual associates and judges. https://note.com/arsenal_best/n/n968f680fb17d
- **Countermeasures for Runaway AI Agents: Value-Unconnected Autonomy** (May 3, 2026) — action accounting for agents whose discretion outruns their values: results booked to the future self as assets and debts. https://note.com/arsenal_best/n/n495335cac2bb
- **The Utterance-Sufficiency Problem** (May 1, 2026) — why declarations and records fail to bind the future self, and how to measure it. https://note.com/arsenal_best/n/n95c5df9901a6
