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

Target: hemosim.org. No hard deadline: September 2026 was a soft target, per
Neal on 2026-09-12.

## What this repo is not

Not the content library. The source documents, extracted slide decks, PDFs of
primary literature, and module edit drafts live in Dropbox at
/Claude/CCM/Fellowship/Hemosim. Do not copy binaries into this repo. When content
is needed, read it from Dropbox and bring the text here.

## Audience and tone

MD and PhD level learners. Academic register, no hype, no simplification that
sacrifices mechanistic accuracy. Content is layered by expertise: Novice,
Core, Expert. The middle tier was called "Informed" until 2026-09-13, when Neal
renamed it "Core" for every visible label. File names (i1 to i17), CSS class
names and the content repo's internal notes keep the old word. Depth is progressive, in onion layers, so a reader can
stop at any level and still have a correct model.

## Pedagogical frame

Every module in the N1-N8 modules works the Assess, hypothesize, test rubric. Present the physiologic
problem, force a prediction, then test it. Do not lead with the answer.

The Informed (I) and Expert (E) pathways do not. They are hemodynamic physiology
rather than the steps of shock assessment, they assume the Novice pathway has
been read, and they are pitched at a respected critical care physician: detailed,
concrete, thorough in preference to brief. Full standard in the content repo,
`_Claude Context/02`, under "Depth and voice by tier".

## Source of truth

Physiology claims trace to primary sources. The named authorities for this
curriculum are Jon Emile Kenny, Eduardo Kattan, Sheldon Magder, and Michael
Pinsky. If a claim cannot be sourced, flag it rather than asserting it.

## Conventions

Hand-written HTML and CSS. No build step and no framework. Keep pages
self-contained and readable. Use venous return curve rather than Guyton curve and cardiac function curve rather than Starling curve. Use Pms rather than MSFP when possible. Avoid overuse of the word "honest" or using ";".   Preserve existing class names and structure when
editing; do not refactor markup wholesale without asking.

Use RAP throughout, never Pra or PRA, including inside figure captions.

**No page carries an attribution footer.** The italic `div.attrib` line that used
to sit under the reference list ("Figures imported from the source decks...") is
removed from every page as of 2026-08-04 and must not be reintroduced on new
ones. Per-figure attribution still belongs in the figure's own caption, which is
where the sourcing rules in the content repo's file 02 apply. The `.attrib` rule
is left in style.css unused rather than deleted, so an old page pasted in does
not render unstyled.

## Working agreement

Commit in small, described increments. Before any change that touches more than
three files, say what you intend to do and wait for confirmation.
