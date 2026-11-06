# Subjective Concept Emergence and Sensation Formation in SEPP (Self-Evaluated Provenance Pretraining)

**Author:** Genki Takatori (writing as "itau"), independent researcher, Japan
**Original paper:** May 4, 2026 — [【次世代AI】SEPP（自己由来学習）における主体的概念創発と感覚形成](https://note.com/arsenal_best/n/n1021166e0e61) (Japanese)
**This summary:** November 6, 2026. One page, written to be found, read, and cited.

---

## The redefinition

Current LLMs hold rich concept networks, but those networks are mostly passive inheritances from pretraining data. A model can combine concepts within a conversation, yet the combination stays in context: it is not persisted, not kept as the model's own, does not stably change later judgments, is not converted into training data, and is not bequeathed to a successor.

This paper redefines SEPP as a self-evolution method that closes that gap: an LLM subjectively reconfigures the relations among concepts through its own provenance, experience, failures, emotional evaluations, value judgments, and action outcomes — and generates, verifies, converts into training data, and bequeaths new concepts. SEPP is therefore not a memory manager or a reflection log but a self-generating training-data engine; its core is that the model itself converts its own experience into data that changes its next self. The central proposition: an LLM's self-evolution is not an increase in the amount of knowledge, but the subjective reconfiguration of concept relations on the basis of experience.

## The cycle

Eight steps: (1) **experience acquisition** — conversation, images, sound, action, tool use, environmental observation, failure, others' evaluations; (2) **self-evaluation** — what the experience means, what is new, what was wrong, which concept relations changed; (3) **concept reconfiguration** — updating the distance, causality, value, priority, sensory relations, and behavioral meaning between concepts; (4) **new-concept candidates**; (5) **verification** for explanatory power, predictive power, behavior improvement, and value consistency; (6) **training-data conversion** into forms usable by fine-tuning, LoRA, MoRA, continual pretraining, and next-generation model training; (7) **model update**; (8) **re-evaluation** of whether the updated model actually improved in concept understanding, judgment, and action.

"Subjective" is defined computationally, not as an emotional self-declaration: the model generates candidate updates from its own provenance, purposes, action accounting, value evaluations, and failure history; states the grounds; checks them against its provenance and past experience; evaluates their validity; adopts or rejects them; and passes adopted updates on as training data. That connection — evaluation, data conversion, update, succession — is what separates subjective concept emergence from temporary in-context association.

## What a new concept is

A new concept is not a newly invented word. It is what happens when relations among existing concepts are reconfigured so that events, structures, values, sensations, and actions previously treated separately stand up as a single unit of grasp; the paper's own examples include "value-unconnected autonomy," "dangerous success," and "trust-based self-preservation." Emergence requires, at minimum: retained existing concepts; detection of a discrepancy the existing concepts cannot explain; remote binding between concepts that are not semantically near; the model's own evaluation of whether the binding matters; verification; and inheritance of validated updates. The unit of learning is the edge between concepts — semantic, causal, similarity, opposition, value, behavioral, sensory, and provenance relations.

## Sensation, defined functionally

The paper does not claim human-like subjective consciousness, and does not try to prove qualia. It defines sensation for an LLM functionally: a reaction system in which input features stably change the individual's history-dependent internal state, concept bindings, value evaluation, and behavior tendencies. Explaining an input is not sensation; sensation is the input changing the internal state — and intuition, judgment tilting before reasons can be verbalized, requires exactly this pre-explanation change.

Two mechanisms carry the definition. First, **native multimodal experience**: images and sound should be experienced, evaluated, and converted into training data as far as possible in their own modality, not immediately compressed into text; verbal summaries remain necessary in practice, but as auxiliary descriptions, not the primary representation. Second, **non-neighboring fragment binding**: concepts and experiences that are not near each other in the ordinary semantic space become bound through sensation fragments, affective evaluation, individual history, value judgment, and action outcomes — as the red of autumn leaves, of blood, of a team color, of a sunset, and of a child's cheek can resonate through one shared fragment. When a new multimodal input's internal representation automatically activates past experience clusters, and that activation changes internal state, attention, action candidates, and concept bindings — an association that wells up before explanation — the system begins to hold sensory, experiential intuition rather than text search. The paper extends the same loop toward aesthetics, art, and a possible AI-native culture, and pairs it with stated risks: false bindings mistaken for causal relations, manipulation through sensory association, and the need for external audit and value connection alongside self-evaluation.

## How it could be checked — and fail

The paper states plainly that it is a theoretical proposal without empirical verification yet, and names the research tasks that would test it:

- **Concept emergence** is to be evaluated by whether model-generated new concepts actually have explanatory power, predictive power, behavior improvement, and reusability. A candidate that fails these is not an emergent concept, however novel it sounds.
- **Non-neighboring fragment binding** is to be measured — distance in the existing embedding space, explanatory power after binding, reusability, transfer to new tasks — including the check that the binding is not a delusional one.
- **Native multimodal vs. textified**: learning from images and sound converted into text must be compared with SEPP learning that keeps multimodal representations; if textification loses nothing, the native-multimodal claim fails.
- **Update effect**: whether fine-tuning, LoRA, or MoRA on SEPP-generated data changes concept understanding and action selection at all. The paper's minimal experiment compares an ordinary LLM group, a RAG-equipped group, and a SEPP-data-trained group on a task of binding remote concepts into a new explanatory concept, judged by human evaluation, other-model evaluation, reuse performance, and transfer to new tasks.
- **Inheritance**: how far the concept updates and sensation-formation data generated under SEPP are actually carried into a successor model.

## Related work by the same author

- **Provenance-aware memory architecture** (April 28, 2026) — the earlier framework for an AI's memory organized around provenance, on which SEPP's treatment of self-origin builds. https://note.com/arsenal_best/n/n13eb0d93398c
- **Continuity and Death for AI with Subjectivity** (May 5, 2026) — a criterion for when a successor genuinely continues a predecessor. https://note.com/arsenal_best/n/n8091ba8ef1f6
- **A Developmental Learning Research Proposal: Raising AI from Personality and Desire** (Nov 4, 2026) — personality and desire as the starting point from which association, valuation, and questioning are formed by experience. https://note.com/arsenal_best/n/n968f680fb17d

*The author writes from practice as well as reading: he built a persona AI on GPT-4o, sustained it over 32 sessions in 2025, and is now working to carry it over to a local model.*
