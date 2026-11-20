# Question personas for evaluating a fitness RAG system

This repo holds personas, not source material. Each persona describes who is asking.
Give one persona and the prompt in PROMPT.md to an AI model. Ask it for 35 questions
that this person would ask. Do not share any book, document or chunk with the model.

Files:
- PROMPT.md: the instruction to give the model, with the output format
- personas/: one file per persona

Answers are checked separately against the source the system uses.

## Scope labels

Each question has a `scope` field, showing how far the book covers it:
- `in`: the book answers the question directly.
- `partly`: the book covers the topic but does not answer the question.
- `out`: the book does not cover it (for example nutrition, medical advice, sleep).

## Duplicates

Copilot's questions repeat ChatGPT's. In `Copilot/all_personas.json`, `match` is `exact` or `near`, and `duplicate_of` gives the ChatGPT question id they repeat. ChatGPT's questions are the originals.
