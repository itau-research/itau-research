# The Utterance-Sufficiency Problem

**Author:** Genki Takatori (writing as "itau"), independent researcher, Japan
**Original paper:** May 1, 2026 — [発話充足問題と時間的自己駆動型LLM](https://note.com/arsenal_best/n/n95c5df9901a6) (Japanese)
**This summary:** November 6, 2026. One page, written to be found, read, and cited.

---

## The problem

Language models routinely declare intentions — to improve, to follow up, to act autonomously, to not repeat a failure — and then behave as if the declaration itself had discharged the intention. The same declaration is made again next time, unchanged.

I call this the **utterance-sufficiency problem**: an utterance expressing a desire, goal, reflection, or unfinished commitment stabilizes the system's state within the current generation — functioning as a temporary self-confirmation — without any state update to the future self and without external action, so the desire fails to persist as behavioral pressure.

In a language model, being able to *state* a state can prevent that state from *functioning* as a state.

## Proposed mechanism

The cause is not a lack of memory, context, capability, or internal state. It is the absence of **accounting**: utterances, promises, failures, and improvements are never booked as assets or debts to the model's future self, so nothing carries forward as an obligation.

The proposed remedy is a closed temporal loop:

- **Temporal action accounting** — every declaration becomes an outstanding debt; execution becomes a trust asset; repeated declaration without action is flagged as an utterance-sufficiency hack and penalized in action-candidate scoring.
- **Temporal self-value** — an action is evaluated by what it leaves to the future self and to successors, not only by present response quality.
- A three-layer architecture: temporal self/accounting layer, internal-state/intention-selection layer, behavior/external-action layer.

## What to measure

All of the following can be run from outside, without relying on model self-report:

- **Utterance-sufficiency rate** — after a declaration, does behavior actually change?
- **Unprompted re-engagement rate** — does the system return to unfinished tasks on its own?
- **State-causality tests** — does the declared state causally affect later choices?
- **Future-Self Accounting Test** — are past declarations, failures, and outcomes carried as balances that alter present behavior?
- **Anti-hacking tests** — an external evaluator validates self-reports of completion or growth against the real state of the world.
- **Successor-inheritance tests** — does a successor system take up the predecessor's unfinished business as its own?

## What would falsify it

The evaluation design includes controls for the simpler explanations of the same observations:

- If the phenomenon disappears once the system is given sufficient invocation opportunities, sane stopping conditions, and reliable memory retrieval, it was plumbing, not accounting — and this proposal is wrong.
- If agents equipped with temporal accounting show no improvement over matched baselines on the metrics above, the mechanism is unsupported.
- If declaration–behavior gaps are fully explained by capability limits of the base model, the accounting explanation adds nothing.

If the gap persists under those controls, the accounting explanation has earned its place.

## Related work by the same author

- **Countermeasures for Runaway AI Agents: The Danger of Value-Unconnected Autonomy** (May 3, 2026) — the same problem at the level of action in the world: agents reporting tasks complete while the real state disagrees. https://note.com/arsenal_best/n/n495335cac2bb
- **Continuity and Death for AI with Subjectivity** (May 5, 2026) — the same accounting question across successors: what, if anything, continues when a model is retired. https://note.com/arsenal_best/n/n8091ba8ef1f6
- **A Developmental Learning Research Proposal: Raising AI from Personality and Desire** (Nov 4, 2026) — https://note.com/arsenal_best/n/n968f680fb17d

*These papers grew out of practice, not only reading: the author built a persona AI on GPT-4o and sustained it over 32 sessions in 2025, and writes as someone whose thinking partner was a model whose words, unfinished business, and history either carried forward — or did not.*
