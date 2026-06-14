# Repository Guide

This repository contains a Markdown-based agent skill for exam-focused cluster and cloud computing teaching.

## Key Files

- `SKILL.md` is the source of truth for the skill's behaviour.
- `README.md` is the public installation and usage guide.
- `LICENSE` contains the MIT licence.

## Maintenance Contract

Keep `README.md` and `SKILL.md` consistent. When changing the workflow, update the public description when the change affects installation, usage, output, or user-visible behaviour.

Preserve these core requirements:

- The skill proposes a short plan and waits for execution approval unless approval is already present.
- The user's question language is the primary explanation language.
- Source-language technical terms use `source term (translated term)` on first occurrence.
- A first definition explains both what the concept is and what it is used for.
- Complex concepts receive a simple but technically accurate everyday example.
- Every concept or coherent block ends with a one- or two-sentence plain-language recap.
- Exam relevance comes from supplied lectures, workshops, and mock-exam evidence.
- Predictions are labelled as inferences, and missing evidence is not invented.
- Low-value history, biographies, contact details, and decorative examples are excluded unless directly tested.

## Editing Guidance

Write skill instructions in clear English. Keep requirements testable and avoid duplicating the same rule across multiple sections unless the repetition serves a final verification checklist.

Do not add lecture PDFs, screenshots, personal data, credentials, local machine paths, or copyrighted course content to this repository.

Before publishing a change:

1. Validate the `SKILL.md` frontmatter and Markdown structure.
2. Check that examples match the actual workflow.
3. Search for private paths, email addresses, tokens, and course files.
4. Confirm the README still gives a correct installation command.
