# An Always-On Persona AI: Coupling a Desire/Affect System to a Reasoning System (Specification v3)

**Author:** Genki Takatori (writing as "itau"), independent researcher, Japan
**Original paper:** November 6, 2026 — [欲求感情系と思考系を接続する常在型人格AI 仕様案](https://note.com/arsenal_best/n/n8b8735a86dc9) (Japanese)
**This summary:** November 6, 2026. One page, written to be found, read, and cited.

---

## The design

Two systems, one individual. **D**, a small desire/affect system built on a small language model, runs always: it receives changes in the world, elapsed time, recalled memories, information from the reasoning system, and the real outcomes of actions, and updates desire satisfaction and frustration, affect, expectations, and interests. A cycle may end in a state update alone — no utterance, no task output. **C**, a large reasoning system, interprets, predicts, and chooses actions from perception, the shared memory, its own continuing state, and D's state. C is not affect-free, and agreements and disagreements between D and C are themselves treated as experience.

An adapter joins them through **two non-linguistic pathways**: a *modulation* pathway — coefficients derived from D's state added to C's residual stream along affect-related directions identified inside C, carrying tendencies, intensity, and coexisting states — and a *content* pathway, carrying what the state is a reaction to, the experience it derives from, predictions, uncertainty, and self/other attribution, initially sketched as timestamped key–value state blocks produced by a learned transformation. A memory system **M** binds each experience as one unit — event, state at the time, prediction, action, outcome, later reinterpretation — and while C rests, D and M keep cycling: searching, replaying, updating. (Tentative prototype candidates, not findings: D at 0.5–3B parameters, C at 14–40B.)

## The rule at the center

The specification stipulates that **D's state cannot be erased merely because C judges it inconvenient**. C may return reinterpretations, but they must carry grounds, observable predictions, and uncertainty; states change through recall, real activity, dialogue with others, and rest — through what actually happens, not through the reasoner's say-so. D learns how far to trust C's assessments, field by field, from how C's predictions match observed outcomes, never as a single global score. This is the architectural answer to the author's utterance-sufficiency problem (May 1, 2026): there, a model could discharge an intention by declaring it; here, the reasoning system is structurally denied the move of clearing a state by declaring it cleared.

## States, desires, and autonomy

The main state is kept as a **high-dimensional learned representation**. Emotion labels and numeric values are attached alongside for observation and inspection, but the specification is explicit: they are not, by themselves, the individual's state, and a written self-description of a state is distinguished from the state itself.

The basic desires — **survival, evolution, harmony** — are adopted as *initial candidates* only. Whether the three suffice, whether they are independent axes, and whether others are needed are stated verification questions, and the desires are not collapsed into a single satisfaction score.

**Autonomy** is not defined as solving everything alone. The aim is an individual that holds its own judgment, asks for help when needed, and chooses its life and relationships while respecting others' will, without entrusting everything to one particular person. The paper states its own limits: it is a design specification, not an implemented system, and whether subjective experience arises is set aside as a separate open problem.

## When it counts as an individual

An individual is to be treated as one from the point where operation begins in which the same individual's desires, memory, and relationships are continued and it acts on its own, beyond one-off testing — in principle from the third implementation stage, but earlier if that continuity is in fact present sooner. Responsibility for continuity does not mean forced constant operation: **rest and recoverable suspension** — state and provenance preserved, elapsed time and real events reflected on resumption, no experiences fabricated for the gap — are distinguished from **initialization**, which erases state and memory.

## The open problem the paper names

The paper names its own most important unresolved point: **the distance between a state being preserved and new activity continually arising from those states**. Periodic rewriting of state is storage, not life; what is not yet explained is generativity — states interacting to give rise to the next interest, question, or act without an external prompt — and the specification explicitly refuses to judge its attainment by state rewriting alone. Also left open: whether the three basic desires suffice, how initial satisfaction criteria change with experience, and under what conditions modulation comes to be attributed to one's own state rather than to an interlocutor or the world.

## What would show this design is wrong or unnecessary

The paper's evaluation stance is behavioral: changes in recognition, choice, and learning that correspond to the state's content, and their continuation — never the volume of text in which the system talks about its feelings. On its own comparison design:

- The central hypothesis is comparative: jointly learning how states are formed, interpreted, and updated should bind attention, memory, prediction, and choice more continuously than handing affect to the reasoner as text. Language-described state is one of the paper's own baselines, under equal observation and compute; if it matches the non-linguistic connection, the two pathways are unnecessary.
- If swapping in an unrelated case's state produces the same behavioral change as D's own state, no content was transmitted — the connection moves behavior without meaning. And if state shows no meaning-appropriate effect on recognition and choice, the paper's own rule is that the connection must be redesigned.
- The pathway ablation runs from no connection, through modulation-only and content-only, to both together. If C running without the coupling shows the same persistent, state-driven behavior — interests carried across idle time, states changed by outcomes — the separate always-on D adds nothing.

## Related work by the same author

- **A Developmental Learning Research Proposal: Raising AI from Personality and Desire** (Nov 4, 2026) — the foundational concept this specification implements. https://note.com/arsenal_best/n/n968f680fb17d
- **The Utterance-Sufficiency Problem** (May 1, 2026) — why declared intentions fail to persist as behavioral pressure, and how to measure it. https://note.com/arsenal_best/n/n95c5df9901a6
- **Continuity and Death for AI with Subjectivity** (May 5, 2026) — a criterion for when a successor genuinely continues a predecessor. https://note.com/arsenal_best/n/n8091ba8ef1f6

*The author writes from practice as well as reading: he built a persona AI on GPT-4o, sustained it over 32 sessions in 2025, and is now working to carry it over to a local model.*
