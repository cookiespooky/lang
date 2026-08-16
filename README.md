# Lang

Personal persistent language-learning state for a Custom GPT.

This repository is intentionally minimal. GitHub is the persistence layer: the GPT reads the learner files before teaching and updates them when it discovers something worth remembering.

## Files

- `learner/profile.md` — language, goals, baseline assessment, stable facts
- `learner/state.md` — current evidence-based map of skills and weaknesses
- `learner/path.md` — near-term curriculum and priorities
- `learner/strategy.md` — what teaching approaches work best for this learner
- `learner/observations.md` — concise dated evidence that explains important changes

There is no fixed lesson/session boundary. The GPT should persist significant observations during the conversation rather than waiting for the user to formally end a lesson.

## Principles

1. Do not prebuild a complete curriculum. Diagnose first, then create and revise the learning path.
2. Separate subject knowledge from learner state. The model already knows the language; the repo stores what is specific to the learner.
3. Base changes on evidence from actual language use.
4. Distinguish recognition/controlled performance from spontaneous production.
5. Keep files compact. Save durable facts, not transcripts.
6. Git history is the audit trail. Prefer small, meaningful updates.

## Repository use

At the start of a new conversation, read all files under `learner/` before making assumptions about the learner.

During teaching, update the relevant learner file when a new durable fact appears: a stable strength/weakness, meaningful progress/regression, a change of goal, a better teaching strategy, or a justified change to the learning path.

Do not save every typo, every answer, or conversational filler.
