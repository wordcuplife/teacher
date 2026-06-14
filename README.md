# Teacher

Teacher is an exam-focused agent skill for explaining cluster and cloud computing course material. It turns lecture PDFs, workshop notes, slides, and mock-exam questions into concise teaching or memorisable revision notes.

The skill keeps the user's language as the main explanation language, preserves source terminology for exam recognition, and prioritises concepts that are supported by the supplied course evidence.

## Installation

### Codex

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/wordcuplife/teacher.git ~/.agents/skills/teacher
```

Restart Codex after installation. You can invoke the skill explicitly with `$teacher`, or ask for exam-focused teaching while providing lecture or workshop files.

### Manual installation

Place this repository in the skills directory used by your agent, keeping `SKILL.md` at the repository root.

## Usage

Example requests:

```text
$teacher Explain pages 19–38 of this lecture for my final exam.
```

```text
$teacher Use these lecture and workshop PDFs plus the mock-exam images to create a bilingual Markdown cheatsheet.
```

The skill first proposes a short plan and waits for execution approval unless the request already includes it.

## What It Does

- Inspects supplied PDFs and mock-exam images, including visual page content.
- Ranks topics by exam evidence instead of summarising every slide.
- Translates the source content language into the user's question language.
- Introduces technical terms as `source term (translated term)`.
- Explains what each major concept is and what it is used for.
- Adds simple everyday examples for difficult mechanisms.
- Ends each concept or teaching block with a one- or two-sentence plain-language recap.
- Separates lecture-supported facts, mock-exam evidence, and predictions.
- Produces page explanations, exam answers, or Markdown cheatsheets.

## Scope

The current skill is designed for cluster and cloud computing revision. Its workflow can be adapted to other technical subjects, but course-specific claims must still come from the material supplied by the user.

It does not guarantee an exam result. It is designed to maximise useful coverage while keeping uncertainty and inference visible.

## Repository Contents

- `SKILL.md`: the agent's complete teaching workflow and quality rules.
- `AGENTS.md`: maintenance guidance for contributors and coding agents.
- `LICENSE`: MIT licence.

No lecture files, screenshots, student data, or private course material are included in this repository.

## License

MIT
