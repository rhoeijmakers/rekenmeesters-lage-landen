# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project: "De Rekenmeesters van de Lage Landen"

This is a Dutch popular-science book project — no build system, no tests, no code. All content lives in `/boek/` as Markdown files.

## File structure

```
boek/
  index.md          ← inhoudsopgave + status per hoofdstuk (update this when adding chapters)
  proloog.md
  deel1_h1.md       ← Deel I, Hoofdstuk 1
  deel1_h2.md
  deel2_h3.md       ← Deel II, Hoofdstuk 3
  ...               ← naming: deel{deel_nr}_h{hoofdstuk_nr}.md
  epiloog.md
```

## Writing conventions

- **Language**: Dutch throughout, no English except for proper nouns and quoted foreign-language titles
- **Tone**: Accessible, narrative, lightly journalistic — like *Sapiens* or *De ontdekking van de hemel*
- **Chapter structure**: Open with a concrete, vivid scene (an anker moment), then broaden to the historical/scientific context
- **Balance**: Weave science, business, and colonial context together — not as separate sections
- **No academic jargon**: Explain concepts through story and analogy, not definitions
- **Shadow side**: Colonial and ethical dimensions are included honestly, not as footnotes

## Chapter template

Each chapter should have:
1. A chapter title + deel header
2. A scene-opening paragraph (concrete moment, named person, specific place and year)
3. Thematic sections with `###` subheadings
4. A navigation link at the bottom: `→ Verder naar [Volgende hoofdstuk](bestand.md)`

## Continuity rules

- **Philips** appears in H7, H10, H13 (ASML origin), H15 (Signify) — keep the characterization consistent: engineering-driven, long-term R&D culture
- **CWI/Mathematisch Centrum** is the thread connecting Van Wijngaarden (H8) → Dijkstra (H9) → ABC → Van Rossum/Python (H11)
- **Kamerlingh Onnes' superconductivity** (H6) reappears in H16 (quantum computing qubits) — make that callback explicit
- The colonial chapters (H3–H5) deliberately include the moral accounting; do not soften or remove this framing

## Index maintenance

After writing or revising any chapter, update `boek/index.md` to reflect the current status (✅ Geschreven / 🔄 In revisie / ⬜ Nog te schrijven).
