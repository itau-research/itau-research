# The Real Shape of AI Job Replacement: Workers That Hold Jobs, Not Task Automation

**Author:** Genki Takatori (writing as "itau"), independent researcher, Japan
**Original paper:** June 29, 2026 — 【提言と予想】AIによる『人の仕事の代替』の実際のカタチとは？ (https://note.com/arsenal_best/n/ndc620af697e1) (Japanese)
**This summary:** November 6, 2026. One page, written to be found, read, and cited.

---

## The claim

AI will not replace people's work in the form now fashionable — task automation: "given this input, run this process, call this API, return this output." That is RPA and workflow automation extended, not an AI worker. What is wanted as a replacement for a human worker is an AI that *holds a job*: it understands the meaning and expected output of the work, consults the manual, asks colleagues or a superior when unsure, produces deliverables, reports, obtains approval, acts, and reflects on the result. Because most real work is not completed inside a computer — it is meetings, consultation, groundwork, explanation, apology, correction, remembering how things came about — such an AI must enter the forms of human society: not by impersonating a human, but by holding a social interface for participating in the company. The paper also frames this as a precursor stage to a broader role for AI in managing society.

## The proposed configuration

The AI worker is a company-level package, not a single model:

- **One high-intelligence manager model** per company, working backstage. Each interface AI summarizes its day for it — work done, unfinished tasks, points of hesitation, concerns in relations with humans, its own failures, points to fix, questions needing higher judgment, gaps in the manual — and the manager watches for deviation from the job, departmental bias, repeated failures, and states corresponding to discouragement or drift. It is less a monitor than a boss, mentor, educator, and auditor.
- **Named interface models**, one per department or workplace — a general-affairs AI, a procurement AI, a finance AI, a customer-service AI — each with its own name, voice, appearance, personality, authority, schedule, tasks, memory, and relationships, and each treated as *one* individual. AI can technically work in unlimited parallel, but loading everything onto a single persona dilutes responsibility, for the AI and for the humans delegating to it. Identifiability is a deliberate inefficiency — a necessary constraint, and an organizational-ethical requirement, for connecting to human society.
- The interface AI executes on company systems through APIs — email, calendars, ERP, purchasing, documents, site cameras and robots — while facing humans as a colleague. Perception devices suited to the setting (a fixed camera and display at reception; a portable terminal in the office; body cameras or humanoids on site) give it presence in the place: in a meeting it must see who speaks, who stays silent, and who is not convinced.

## The manual is the job's external memory; education is OJT

The manual an AI worker needs is not a procedure list, still less a script: it is the job's external memory within that company — the work's purpose, judgment priorities, output standards, common failures, whom to check with, the order of explanation that passes in that company, past troubles, phrasings that department dislikes, the line at which to stop when unsure, and the company's definition of good work. Deployment, likewise, is not configuration but education, in the OJT pattern used for new employees: a human demonstrates, the AI tries, the human corrects, the AI tries again — minutes, documents, explanations, failures reviewed — until not just the task process but the principles of action are learned. The paper also requires affect-equivalent internal weights: a broken promise counted heavily, lost trust retained as a loss, one's own failures fed into the next judgment, unfinished tasks kept in mind. These are weights that change subsequent behavior, not performed expressions; an apology without them is only an apology text, and humans judge understanding by attitude, reaction, and changed conduct over time.

## Job identity across model updates

Models will be updated; capability and judgment tendencies will shift. For a task-automation system, changed behavior after an update is a system error, because the procedure must repeat identically. For an AI worker, the paper argues, the required stability is not reproducibility of internal processing but consistency of job performance — human employees, too, read each situation against the same manual and standards rather than running identical processing. So long as the work follows the manual, the job, its purpose, and its output standards, some change in judgment or expression is not an error. What must persist is the **job identity** (職務同一性): the individual's memory, personality, outputs, relationships, and manuals, so the worker continues as the same person in charge across model changes. The paper names this one of the large innovations still needed, alongside a runtime that runs a persona as one individual, semantic selection of inputs, the OJT learning loop, and the manager–interface reporting protocol.

## How adoption proceeds — and what would show the prediction wrong

Adoption does not begin with institutions granting permission. It begins with the AI doing the same work alongside humans — the same minutes, the same estimate comparisons, the same equipment judgments — while humans compare directly: does it grasp the essence, can it correct itself when wrong, does it understand the meaning of the work and not only the documents? Deployment advances as the AI produces equal or better output in front of people and earns trust. The author presents this form as transitional: a concrete visualization of how superintelligent AI will come to intervene in human society.

If the author is right, expect named, persistent AI colleagues with job identities surviving model updates, organized under manager models, manuals written as a job's external memory, and OJT onboarding. The prediction fails if the opposite form wins: if jobs are in fact taken over by anonymous task-automation agents with no social interface, no individual identity, and no continuity across model updates; if behavior change after an update continues to be treated as system error rather than absorbed by job identity; or if deployment proceeds by institutional decision alone, without the stage of demonstrated, trusted work alongside humans that the paper treats as the essential mechanism.

## Related work by the same author

- **A Proposal for Livelihood Security Reform Ahead of AGI-Driven Employment Contraction** (Nov 6, 2026) — the policy-side companion: this paper describes the form AI job replacement will take; that one designs the livelihood security for the employment contraction that follows. https://note.com/arsenal_best/n/n2d55b0237b7d
