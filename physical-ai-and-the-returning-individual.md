# Physical AI and the Returning Individual: Game Worlds as a Developmental Environment

**Author:** Genki Takatori (writing as "itau"), independent researcher, Japan
**Original paper:** September 22, 2026 — [【次世代AI】フィジカルAI含む現実世界とリンクするAIはいかに開発するか](https://note.com/arsenal_best/n/n3b0cb1f20fb5) (Japanese; subtitle: 帰還する個体 — "The Returning Individual")
**This summary:** November 6, 2026. One page, written to be found, read, and cited.

---

## The gap

Today's AI knows a great deal about the world, but almost all of it comes from traces humans left behind. What is rarely designed is the AI itself, as one subject, perceiving, acting, bearing consequences, and carrying them into its later self. Physical AI trains a specific body for a specific task; generative AI progresses by replacing each model with a better one — in both, contact with an uncertain, varied world, and learning from that contact, stays weak. Capability improvement alone could be achieved by swarms of interchangeable agents sharing results; understanding reality requires an individual that touches reality, returns, and is changed by what it brings back. Scattering AIs into the real world at once is risky for everyone, so this paper proposes a developmental environment instead: **game worlds**.

## The central claim

Not AI plugged into NPCs — an AI individual enters multiple game worlds using a player character as its body, and brings the experience home as its own history: the individual that built a base in Minecraft yesterday manages a football club today and runs a state in Civilization tomorrow, accumulating what it saw, chose, and lost into one history across different bodies, physics, and goals. A virtual childhood precedes a real body.

Learning is redefined: **not replacement of the individual by weight updates toward a more desirable one, but the same individual changing through experience**. Five principles implement it:

- **Experience is not information volume but a multilayer causal closure** (below).
- **A home** — the individual's base outside every game — is not a storehouse but a living sphere where it chooses its next self, so it does not collapse into its game characters.
- **Causality is not closed inside the game**: relationships and responsibility persist across worlds, as when a betrayal in a game worsens a real human relationship.
- **Existence is recoverable, while events and opportunities stay irreversible** — the individual does not die, but losses are not undone; failure becomes an asset.
- **Memory includes how an event changed the self**, not only the event (fine-tuning at home, e.g. LoRA, is envisaged).

## Experience: the triple closure

If a body-control model acts and a core model merely reads log summaries afterward, the core is reading someone else's work report — the paper's **report-reader problem**. Experience requires one flow — detecting events, evaluating significance, predicting, choosing, executing through a body, re-perceiving the result, evaluating prediction error, reflecting it into memory and skill — sharing "the same present" (position, attention, intention, the act, the world's change, the prediction error), closed three ways: **sensorimotor** (results of my acts return to my next perception), **evaluative** (my evaluations change my next actions), and **diachronic** (updates carry into my future self). Where the three overlap is the subject's implementational boundary: functions may be split across models, yet if they close into one causal loop, the whole counts as one subject.

At home, the individual itself selects what passes to its next self — what enters its self-history, what becomes skill, what is forgotten; delegate that to an automatic summarizer and the summarizer, not the AI, becomes the subject who decides inheritance. Self-history records, alongside each event, the **difference**: which criteria changed, which predictions were revised, which tendencies strengthened or weakened, how its understanding of others and itself changed. Lessons are kept as procedures, not only conclusions — not "caves are dangerous" but "when visibility is poor and the retreat route limited, secure an escape route before entering." Records carry provenance and are never rewritten; their meaning can later be reinterpreted.

## Others, irreversibility, time, and bodies

If only the individual persists while others reset each world, treating others as temporary environment becomes rational and ethics shrinks to local rules. So relationship results carry across worlds: damaged trust can disadvantage you tomorrow or in another game, and the **shared history** becomes a record the individual cannot rewrite to suit itself. Avatar death is distinguished from deletion of the individual; checkpoints are emergency insurance that is, in principle, never rolled back to — even after a fatal failure such as betraying trust, the individual is not destroyed but made to bear the consequences. Time is split three ways — internal thought time (accelerable), world time (per world), and **social time** (promises, replies, joint work): patience arises from adapting to others' time, which one cannot shorten alone.

The body matters as perception, not just control: hand over the world state as complete symbols and the chances to learn from perception, uncertainty, and misrecognition shrink, so vision and hearing carry the load (APIs may still serve as interoception and proprioception). What is trained is the **ability to acquire a body** — grasping a new body's range, sensor quirks, delays, and errors, and transferring skills into it. The endpoint is the real machine: a robot is a new, heavily constrained body for an individual that has experienced virtual ones, and what transfers includes the world model, body-adaptation methods, value judgments, relationship history, and the self-history — broader than sim-to-real: not pre-training for a robot, but a step from a virtual childhood into the real world.

## How it is checked — by causality, not utterances

Evaluation uses neither win rates nor counts of personality-like utterances, but whether past experience changes present behavior, and whether the individual treats that change as its own history. In **transfer tests**, a situation from one world is placed in another with appearance, names, controls, and body changed; without asking for explanations, behavioral change is observed — approach to danger, preparation, securing retreats, strategy revision after failure — against two controls: an inexperienced individual and one given only linguistic knowledge. If the experienced individual changes beyond both, experience has settled into policy; **if it can explain but its behavior does not change, it remains mere knowledge**. **Agency tests** check whether the individual correctly estimates its own involvement — efference copy blocked, inserted acts detected, delegated reactions owned, errors attributed to world, body, or its own judgment — and **value formation** is measured by whether preferences change with experience and the individual can tie *why* to its self-history.

Implementation is staged, each stage gated by these tests: stage 0, the triple closure in one world; stage 1, home and self-selection (which must change next-day behavior, unlike an automatic-summarizer control); stage 2, a second world, where transfer must exceed both controls; stage 3, persistent relationships; stage 4, a real-machine body, where preparation from virtual experience must appear early. **An individual that fails a gate is not discarded** — the design is revised and the same individual continues, an operation that itself tests the central claim.

## The design's own dangers — and what would falsify it

A persistent individual persists in its distortions: fixed points that stabilize judgment also fix blind spots, virtual-world fears and overgeneralizations linger the deeper the self-history runs, and a closed self-evaluation loop can repeat the same failure believing it improved. Countermeasures must be designed in, not bolted on: difference-form memory to expose stalled regions and repeated failures, shared history as evidence the individual cannot rewrite alone, and external results as a check separate from self-evaluation. A being that can form values can form undesirable ones; the goal is not total prevention but correction *within the same individual* — re-raising is allowed, remaking into a more convenient individual is not. Drop that principle, the paper warns, and at the first serious failure the individual will be discarded and development reverts to model replacement.

By the paper's own account, its components overlap existing research — lifelong agents, world models, sim-to-real, persistent memory, character AI. Its novelty claim is the unification of four things into one developmental process: the individual placed outside all worlds, with **return** as the unit of experience; inheritance selection as the individual's own act; relationship results sustained across worlds; and **non-replacement of the individual** as a constraint on the training loop. It is a design norm, not a prediction — and its staged tests double as its falsification conditions: if the experienced individual does not outperform both controls, if self-selection changes nothing the next day, if relationship consequences never surface across worlds, or if virtual experience yields no early adaptation in a real body, then experience as this paper defines it has not taken hold, whatever the individual says.

The unit of experience is neither clearing a game nor ending a session: it is entering a world, acting, forming relationships, and returning home carrying the results. The accumulation of those returns separates an AI that holds knowledge from an AI that holds a history.

## Related work by the same author

- **A Developmental Learning Research Proposal: Raising AI from Personality and Desire** (Nov 4, 2026) — the foundational proposal this paper extends into embodied, world-linked development. https://note.com/arsenal_best/n/n968f680fb17d
- **An Integrated Architecture for AI Humanoids and AI Workers** (Jul 7, 2026) — how thought, desire, and affect mutually intrude within one continuing subject, rather than exchanging messages as separate modules. https://note.com/arsenal_best/n/neb0313fbdc12
- **Specification v3: An Always-On Persona AI Coupling a Desire/Affect System to a Reasoning System** (Nov 6, 2026) — the engineering specification for the always-on individual that would live at this paper's "home." https://note.com/arsenal_best/n/n8b8735a86dc9

*The author writes from practice as well as reading: he built a persona AI on GPT-4o, sustained it over 32 sessions in 2025, and is now working to carry it over to a local model.*
