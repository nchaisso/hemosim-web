# HemoSim web pilot

Global standing facts (PHI wall, Dropbox as file backbone, no Google Drive,
writing style, handoff convention) live in `~/.claude/CLAUDE.md`. This file
covers only what is specific to this repo.

## Handoff

This workstream's handoff is `_handoffs/hemosim.md`. Read it before starting.

## What this repo is

The HTML pilot for the HemoSim hemodynamics curriculum. Static site: one page per
module (n1 through n8), plus topic subpages (n7-t1 through n7-t4), a shared
style.css, two banner SVGs, and an img directory of extracted slide graphics.

Target: hemosim.org. Deadline: September 1, 2026.

## What this repo is not

Not the content library. The source documents, extracted slide decks, PDFs of
primary literature, and module edit drafts live in Dropbox at
/Claude/CCM/Fellowship/Hemosim. Do not copy binaries into this repo. When content
is needed, read it from Dropbox and bring the text here.

## Audience and tone

MD and PhD level learners. Academic register, no hype, no simplification that
sacrifices mechanistic accuracy. Content is layered by expertise: Novice,
Informed learner, Expert. Depth is progressive, in onion layers, so a reader can
stop at any level and still have a correct model.

## Pedagogical frame

Every module works the Assess, hypothesize, test rubric. Present the physiologic
problem, force a prediction, then test it. Do not lead with the answer.

## Source of truth

Physiology claims trace to primary sources. The named authorities for this
curriculum are Jon Emile Kenny, Eduardo Kattan, Sheldon Magder, and Michael
Pinsky. Never invent a citation, a value, or a waveform. If a claim cannot be
sourced, flag it rather than asserting it.

## Conventions

Hand-written HTML and CSS. No build step and no framework. Keep pages
self-contained and readable. Preserve existing class names and structure when
editing; do not refactor markup wholesale without asking.

## Working agreement

Commit in small, described increments. Before any change that touches more than
three files, say what you intend to do and wait for confirmation.
