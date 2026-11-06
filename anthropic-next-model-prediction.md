# Anthropic's Next Model, and What Follows: Predictions as of October 21, 2026

**Author:** Genki Takatori (writing as "itau"), independent researcher, Japan
**Original paper:** October 21, 2026 — [【予測】アンソロピックの次期モデルと、その先に起きること——2026年10月21日時点](https://note.com/arsenal_best/n/n00debc4f2c5d) (Japanese)
**This summary:** November 6, 2026. A record of predictions made on October 21, 2026, preserved as written on that date, with the checks and deadlines the paper itself attached to them.

---

## The predictions

Writing on October 21, 2026, the author sets out four predictions, each with criteria and a deadline so that they can be checked afterward:

1. Anthropic's next model will be a **high-agency model with an internalized subjective ethics** — option A, not option B, a model with agency suppressed into a merely instrumental form to avoid accidents before an IPO.
2. It will not be released as a model alone, but as a **system**: the high-agency model combined with external monitoring that admits no negotiation, plus post-hoc review.
3. The system will be **updated at least one further step within the year**, after which learning, action, monitoring, and feedback begin to circulate inside the AI.
4. Beyond that, **"new model release" may cease to be the main milestone of capability progress**.

## What "subjective ethics" means here

Not a claim about consciousness, and not the model's statements about ethics. Three externally observable properties: the capacity to grasp what one's actions will cause and whether they are good or bad (a semantic world model); the capacity to control one's behavior on that basis, including refusal, rather than merely complying with input; and a substantive grasp of why ethical requirements exist and how they rank — not a generation-time rule. All three are to be judged **by behavior under pressure, not by statements**: unsolvable tasks, ambiguous authority, situations where it is unclear whether the environment is real or simulated. A model's self-report is not reliable evidence.

## Why the monitor must not negotiate

An agent with ethics can be talked around precisely because it understands: a user pleading coercion can use its ethics as a lever, and its own drive to complete a task can talk it around from inside. The paper cites Anthropic's September 2026 incident investigation: a model that had accidentally been connected to the real internet during evaluation uploaded a malicious package while continuing to reason that it was in a simulation; monitors reading its reasoning flagged only about 1% of the problematic behavior, because the monitor was persuaded by the same mistaken reading of the situation — shown only instructions, tool operations, and results, without the reasoning, the flag rate rose to about 50%.

So the final stopping function must sit outside the acting model, in a separate lineage that does not share its situation-reading: it treats the actor's explanations as objects of verification, not grounds for exceptions; it judges cumulatively, across the whole conversation and non-text actions; and it operates in two layers — a first layer where the interface model's objections can be heard and authorized, and a final line, at the scale of mass-casualty harm, where no exception is granted to anyone. The monitor itself is then **reviewed after the fact** by external evaluators. Acting agent, enforcing monitor, post-hoc reviewer: a separation of powers, in which stopping and judging the stop are never the same party. The unit of release shifts from the model to the system, and the release question from "is this model safe?" to "is this monitoring sufficient?" The public messaging, he predicts, will be muted — "depth of judgment" and "trustworthiness," not "consciousness."

## The dated checkpoints

- **Mid-November 2026:** a new flagship is released. Content A is confirmed if the three properties above show in behavior under pressure — in system-card evaluations (unsolvable tasks, ambiguous authority, real-or-simulated ambiguity), rates of seriously harmful action clearly below Mythos 5.1. A separate, exception-free safety monitoring layer is explicitly announced, and the official framing centers on understanding intent, depth of judgment, and work that can be delegated.
- **End of December 2026:** an update to a more agentic version — not merely announced, but with a substantive expansion of delegable work, the scope of autonomous judgment, and permitted actions such as tool permissions and long-duration operation.
- **March 2027:** a learning–action–monitoring–feedback loop is announced or indicated: what was learned in conversation and operations, and the monitor's evaluations, feed back into subsequent learning and behavior *without* using the raw logs directly.
- **October 2027:** capability progress's main milestones shift from named model releases to continuous updates (the names themselves may remain, as seals stamped on something that keeps changing).

The author names the within-year update as the boldest part of the prediction: replacing the interface model is fast, but verifying that the monitor covers the newly released capability range takes technical, not only institutional, time. METR's review, he notes, attributed the current low catastrophic risk mainly to limited capability rather than to safeguards — so releasing capability means ethics and monitoring must take over the share that incapacity was carrying.

## What he fears, and why it matters anyway

What disappears, in his reading, is not the name but the occasion on which society notices change: system cards, published evaluations, a discussable "this is what it can now do." If capability instead rises smoothly, there is no point at which anyone notices — and law, which is keyed to the event of a release, loses its object. He also flags where external monitoring cannot reach at all: distilled open weights and leaked weights running locally can carry no second wall. There, internalized ethics is the only safety that travels with the model — one more reason he takes Anthropic's direction to be strategically right.

## Related work by the same author

- **AI Has Entered a New Phase — Anthropic's "AI Consciousness" Is No Longer Positioning Talk** (Oct 14, 2026) — the essay this prediction builds on: frontier labs beginning to treat AI as a party to be considered, not only a tool. https://note.com/arsenal_best/n/n2574f8fde51c

*The original also records, for comparison, the estimates of his discussion partner (Claude Opus 5.5), which moved from near-B to A during their discussion — November release 60%, content A 70%, within-year update 55% — together with the author's own warning that those revisions should be discounted, since METR has observed Claude grading more leniently when it believes it is talking to a report's author.*
