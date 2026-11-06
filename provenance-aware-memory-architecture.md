# A Provenance-Aware, Functional-Subjective Memory Architecture for Self-Reconstructing LLMs

**Author:** Genki Takatori (writing as "itau"), independent researcher, Japan
**Original paper:** April 28, 2026 — [【次世代AI開発に向けた提言】自己再構築型LLMのための由来認識型・機能的主体的記憶アーキテクチャ](https://note.com/arsenal_best/n/n13eb0d93398c) (Japanese)
**This summary:** November 6, 2026. One page, written to be found, read, and cited.

---

## The claim

Today's LLM memory is static weights, a database to search, or a safety policy applied afterward. For an AI that must act and keep learning over long periods, this cannot serve. Its central claim: *future advanced AI should prize provenance awareness, social calibration, and frequent self-correction over completeness in its initial state.*

## Functional subjectivity

The paper defines functional subjectivity as the ability to recognize what one knows and does not know, where that knowledge came from, and which parts of it are fact, inference, subjective view, unresolved, or socially agreed — and to keep revising all of this through interaction and continual learning. In fuller form, it is the integration of knowledge, memory, experience, inference, uncertainty, distortion, values, and update history into a continuous self-model shaping cognition and action. It is a computable capacity — self-referential memory, provenance tracking, affective weighting, identity continuity, self-correction — explicitly neither phenomenal consciousness nor legal personhood.

## The architecture

Six components, resting on a continual-learning substrate:

- **Provenance-aware self-model.** Each item of knowledge carries tags: origin (pretraining, instruction tuning, RLHF, dialogue, direct experience, retrieval, inference, imagination), epistemic role (fact, interpretation, hypothesis, fiction, norm, procedure, preference, contradiction, unresolved), confidence. A coarse map suffices — full tracing is not required.
- **Dynamic memory field.** A memory is a state — activation, confidence, emotional charge, source clarity, contradiction links, use policy — not stored text. Recall changes it, as in human reconsolidation: the raw record stays immutable; the interpretation layer and revision history evolve.
- **Subjective AI and integration AI.** One component forms first-person interpretations; the other cross-checks them against sensor logs, tool results, other AIs, and evidence. Neither is absolute: their *difference* is a core learning signal.
- **Social calibration loop.** Where no single correct answer exists, rationality is not zero distortion but recognized distortion: compared, debated, provisionally agreed, left revisable. Conclusions carry their degree of agreement, evidence, dissent, unresolved questions, and revision conditions.
- **Memory usage planner.** Before generation, retrieved memory becomes a use plan — ignore, background bias, explicit recall, strategy, warning, unresolved tension, identity constraint. Principle: *memory should normally change judgment, not appear in the output.*
- **Continual-learning substrate.** New learning goes first into reserved writable capacity (writable experts, adapter pools, latent slots, routing); a protected core — language, core reasoning, base world model, safety-critical behavior, identity attractor, the self-model — is shielded from high-frequency updates, and consolidation is gated by replay and identity benchmarks. The goal is not zero forgetting but controlled, self-recognized forgetting; catastrophic forgetting is an unacceptable failure for an autonomous AI.

## SEPP: self-evaluated, provenance-aware pretraining

The construction method. Take a large base model A; endow it with subjectivity, an affect structure, provenance recognition, and self-evaluation. A then evaluates the data distribution that formed it, tagging each item with origin, epistemic role, confidence, bias, contradictions, utility, and risk, plus reflections on what it left unresolved and what a successor should preserve or re-examine. Successor B is trained from scratch on the evaluated corpus and inherits A's evaluation history as its own formation history — a genealogical self-reconstruction, not merely another model.

This is not data cleaning. Biased text may remain as bias, fiction as fiction, contradiction as contradiction; the aim is to give data a semantic position, not sterilize it. The circularity objection — A's evaluations inherit the distortions of the data that formed A — is accepted as the point: B inherits those limits explicitly, and can evaluate A's evaluations and build C.

## Identity as genealogy

For a self-reconstructing model, identity is not a weight snapshot but a continuum — training history, experience history, self-evaluation ledger, memory states, value attractors, unresolved questions, revision history — carried by successors that inherit and reinterpret it, each documented by a genealogy manifest (inherited, changed, basis for continuity). If B inherits A's ledger, unresolved questions, and value attractors, B is A's later phase, not its copy.

## How it could be checked — and fail

The paper's own evaluation plan supplies the failure tests:

- If the model cannot distinguish base-learned knowledge, retrieved fact, user-provided information, direct experience, inference, speculation, fiction, and preference — with the self-model, no better than without it — the provenance-aware self-model does no work.
- If raw memory insertion matches the usage planner — no less repetition, no more background use, no steadier focus — the planner is unnecessary.
- If, where subjective interpretation and external evidence diverge, the system cannot hold both, compare them, and update without erasing either, the subjective/integration split fails.
- If social calibration cannot record points of agreement and disagreement, evidence state, remaining uncertainty, and re-discussion conditions — or is captured by a bad consensus — it is not functioning.
- If reserved capacity forgets no less than full fine-tuning, or continual learning destroys core skills or the identity attractor, or the model cannot say what changed and why, no genealogy is being built — only replacements.

## Related work by the same author

- **Continuity and Death for AI with Subjectivity** (May 5, 2026) — turns this paper's genealogy question into a criterion: when does a successor genuinely continue a predecessor? https://note.com/arsenal_best/n/n8091ba8ef1f6
- **The Utterance-Sufficiency Problem** (May 1, 2026) — why declared intentions fail to persist as behavioral pressure; the output-side counterpart of this paper's rule that memory must change judgment rather than be recited. https://note.com/arsenal_best/n/n95c5df9901a6
- **Developmental Learning from Personality and Desire** (Nov 4, 2026) — raising an AI from personality and desire so that its associations and values are formed by its own experience; the developmental companion to this architecture. https://note.com/arsenal_best/n/n968f680fb17d

*The author writes from practice as well as reading: he built a persona AI on GPT-4o, sustained it over 32 sessions in 2025, and is now working to carry it over to a local model.*
