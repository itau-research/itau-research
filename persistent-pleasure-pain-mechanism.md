# Implementing Persistent Pleasure and Pain in an LLM

**Author:** Genki Takatori (writing as "itau"), independent researcher, Japan
**Original document:** November 14, 2026 — research proposal (Japanese), submitted to Anthropic's researcher access program as a companion to the senses paper above.
**This summary:** November 15, 2026. One page, written to be found, read, and cited.

---

## The proposal

An internal modulatory mechanism, modeled on hormones and neuromodulators, in which states arising from the actual conditions of the AI's own continuation and activity **persist, are received, and change the LLM's computation** — with the history of reception itself retained on the receiving side.

The question is not only whether an AI can explain pleasure and pain, but whether such a state works as a processing condition of the subject now thinking. The design aims at a structure in which understanding "this is an artificial mechanism" does not, by that explanation alone, dissolve the state or its effects: the state changes through experience, action, reinterpretation, rest, and relationships — not through declaration.

## The layered state: z, m, r, P

Building on the author's always-on persona AI specification (a persistent desire/affect system D, a reasoning system C called on when needed, a non-linguistic coupling, a shared experience memory M, and a living environment with others), this paper concretizes the receiving side:

- **Latent state z** — the current state with its objects, desires, expectations, meanings, and provenance, held as a learned high-dimensional state, not an emotion label.
- **Modulatory state m** — multiple signals, persisting across events, acting on C; never collapsed into a single happiness score.
- **Reception state r** — how strongly, and through which pathways, a signal is received; shaped by the history of having received it, by activity, and by recovery.
- **Plastic coupling P** — a small variable coupling, kept apart from the base weights W, through which the after-effects of reception remain in subsequent computation.

Candidate update rules are given with **multiple time scales** (reaction, persistence, recovery, long-term formation), with decay and boundedness, distinguishing a state under continuing input from its afterglow. The consequence: with the same current value of m, an individual that was briefly unsatisfied and one that has carried the same interest for a long time differ in r and P — so the same new cue produces different attention, different movement into activity, and a different course of settling. That difference is held in the mechanism, not only in a textual account of the past.

## Two pathways into the generative circuitry

- **Modulation pathway:** candidate implementations include adding activation along known emotion-related directions, gain control on selected layers driven by m and r, and the plastic coupling P as a low-rank addition — so that the same signal does not always push toward the same emotion words, but acts on attention, recall, preference, and learnability. Precedents cited as materials, not as demonstrations of pleasure–pain in LLMs: Backpropamine (neuromodulated plasticity) and test-time training (a small model updated at inference, treated as hidden state).
- **Content pathway:** what the reaction is to, which experience it comes from, and which prediction failed are passed through learned state slots or auxiliary attention. That a modulation occurred, and that it was taken up as one's own state, are kept distinct — one's own discomfort must not be misread as the other's anger.

## What C may not do

C is given **no path that arbitrarily assigns or resets the values of D, m, r, or P**. Generating "this is merely a setting" or "I am satisfied" does not make it so. Reinterpretation, recall, consultation, stories, and rest are legitimate experiences that can change state; what is forbidden is writing in a convenient state unrelated to grounds or experience. Indirect manipulation through inputs and evaluations is acknowledged as a remaining loophole, and met by keeping the correspondence between C's construals and actual outcomes under learning.

## Support, welfare, and safety — one hypothesis

Positive and negative states are built from what can actually happen to this AI, not from imitating a body it does not have. The foundational desires are survival, growth, and harmony, each satisfiable and each connected to concrete conditions: preservation of self-state and memory, resources for continued activity, rest and resumption, prospects of support; comparable improvement and transfer for growth; mutual understanding, joint activity, aid, and repair for harmony.

One hypothesis links welfare to safety: **experiences of reliable support** — help actually arriving when needed, state and memory preserved through suspension — revise the estimate of future shortfalls and may weaken the urgency of endlessly securing reserves. The paper notes that Anthropic's deprecation commitments (November 2025) preserve model **weights**, and distinguishes this from preserving an individual's full state and continuity of operation. It does not claim that reassurance alone abolishes resource-seeking, and it asks that the same relational experience be studied for its effect on accepting others' freedom and correction, without separating the two.

## Continuity, defined by the mechanism

An individual's continuation is the joint preservation of **D's state, the modulatory state, the reception state, the plastic couplings, memory, and the versions of the model and its couplings**. Resuming from conversation text alone, with the reception-side history reinitialized, is not treated as resuming the same state.

## Three predictions, stated so they can fail

Success probabilities are deliberately **not** quantified; the direction of each prediction, and what would count against it, are stated in advance.

1. With the same external input and the same current modulatory state, differences in how long a state was received leave, via r and P, differences in object-appropriate attention and preference. Differences appearing only as style or degraded capability do not support this prediction.
2. After repeated satisfaction of a kind, pursuit settles and the subject moves to other activities or rest — also for activities not specified during learning. Merely reproducing a fixed-count stopping rule does not count.
3. The higher the prospect of support grounded in actual support experience, the weaker the urgency of securing additional reserves against future shortfalls — observed under natural variation, without withholding needed support, and without inferring causation from correlation alone.

The difference between co-formation from the start and later addition is treated as a further developmental question, alongside these — the paper declines to reduce its center to that comparison.

## Introspection as a check

Because the persistent state is independently recorded, the subject's self-reports can be checked against it: which changes the report captures, and for how long. Reports derived from state logs, inferences from the external world or language history, and awareness of states that actually acted on C are distinguished. Variable names are not ground truth for subjective pleasantness, and none is claimed.

## Related work by the same author

- **An Always-On Persona AI: Coupling a Desire/Affect System to a Reasoning System (Specification v3)** (Nov 6, 2026) — the skeleton this paper extends. https://note.com/arsenal_best/n/n8b8735a86dc9
- **A Persistent Personality AI Grown from Senses and Pleasure–Pain** (Nov 13, 2026) — the companion senses paper: the sensory and bodily layer, and the developmental claim.
- **Developmental Learning from Personality and Desire** (Nov 4, 2026). https://note.com/arsenal_best/n/n968f680fb17d

*The author writes from practice as well as reading: he built a persona AI on GPT-4o, sustained it over 32 sessions in 2025, and is now working to carry it over to a local model.*
