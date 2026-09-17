# Inkraft

AI-assisted writing support for Chinese academic writing workflows.

[Live demo](https://cyrilla-mist.github.io/inkraft/) · [Portfolio](https://cyrilla-mist.github.io/portfolio/)

> **Status:** Earlier experiment. Public and usable, but maintained minimally rather than developed as a current flagship product.

## Overview

Inkraft was built to explore a more careful AI writing workflow for university students. Instead of only generating or rewriting text, it also tries to explain what changed, flag possible meaning drift, and remind the user when a result still needs manual verification.

The interface is primarily designed for Chinese academic-writing tasks.

## Features

- **Writing review** — checks academic expression, logical flow, revision priorities, and possible writing risks.
- **Paraphrasing** — restructures wording while attempting to preserve the original meaning.
- **Academic polishing** — improves clarity and formality at different editing strengths.
- **Abstract generation** — creates a requested-length abstract and extracts keywords.
- **Translation polishing** — adapts wording across languages with context-aware notes.
- **Reference formatting** — restructures citation information into requested formats and flags missing fields.
- **Combined workflow** — produces paraphrasing, polishing, and abstract outputs from one input.
- **Responsive UI** — supports desktop and mobile layouts with light and dark themes.

## Design Principles

Inkraft follows a few simple constraints:

- preserving meaning is more important than changing sentence structure;
- readability should not be sacrificed only to reduce textual similarity;
- the model should not invent unsupported data, cases, citations, or conclusions;
- risky changes should be surfaced instead of silently treated as correct;
- AI output remains a draft that requires human review.

## Technology

- HTML
- CSS
- JavaScript
- DeepSeek API
- Cloudflare Worker
- GitHub Pages

The frontend uses native HTML, CSS, and JavaScript. Model requests are routed through a Cloudflare Worker so API credentials are not stored in the public frontend.

## Usage

1. Open the live demo.
2. Choose a writing workflow.
3. Paste the text to review or revise.
4. Adjust available parameters when needed.
5. Review the result, change notes, and risk reminders before using the output.

## Limitations

Inkraft does not replace an instructor, academic-integrity review, plagiarism-detection service, or professional copy editor. It does not guarantee plagiarism scores, AI-detection outcomes, factual correctness, or citation validity.

Do not submit personal identifiers, confidential research data, or other sensitive material.

## Version

Current public version: **v1.2**

## Author

Cyrilla

© 2026 Cyrilla
