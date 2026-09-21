# HemoSim

Practical hemodynamics for clinicians who care for patients in shock.

HemoSim is a modular, case-based curriculum in bedside hemodynamics. This
repository holds the web pilot. It is a work in progress, shared so that 
colleagues can read it, test it against their own understanding, and tell 
us where it falls short.

> **Status: prototype.** The content is under active physician review and has
> not been finalized. It is an educational resource, not medical advice, and it
> should not be used to direct the care of any patient.

## Who it is for

HemoSim is written for healthcare providers and is pitched at the level of a
physician: a resident, fellow, or attending who manages shock and wants a firmer
physiologic footing. Medical students, physician assistants, and nurse
practitioners should find it usable, although it is not written specifically for
those groups. 

## How the curriculum is organized

Content is layered by expertise, so that a reader can stop at any level and
still hold a correct model of the circulation.

| Tier | Pages | Purpose |
| --- | --- | --- |
| **Novice** | `n1.html` to `n8.html`, plus `n7-t1.html` to `n7-t4.html` | A systematic bedside approach to the patient in shock. |
| **Core** | `i1.html` to `i17.html` | The physiology behind the bedside approach, in depth. |
| **Expert** | not yet built | Edge cases, controversies, and the primary literature. |

A note on file names: the Core tier was originally called "Informed," which is
why its pages are numbered `i1` to `i17`. The visible label changed and the file
names did not.

### Novice pathway

The Novice modules follow a fixed teaching pattern: assess, hypothesize, test.
Each page presents a physiologic problem, asks the reader to commit to a
prediction, and only then works through the answer.

| Page | Topic |
| --- | --- |
| N1 | What shock is, and why hemodynamics matters |
| N2 | Oxygen delivery as the organizing principle |
| N3 | Recognizing shock at the bedside |
| N4 | The big-picture circulatory map |
| N5 | The curves, the equation, and the shock-type grid |
| N6 | The ACT method |
| N7 | The pulmonary artery catheter, which opens into four topic pages: indications and setup, insertion and troubleshooting, waveforms and wedging, cardiac output measurement |
| N8 | Put it together |

### Core pathway

The Core modules assume the Novice pathway has been read. They are organized
around the circulation itself rather than around the steps of shock assessment,
and they favor thoroughness over brevity.

| Pages | Topic |
| --- | --- |
| I1 to I3 | Physiologic foundations, bedside phenotypes of shock, pressure measurement and waveform fundamentals |
| I4 to I10 | A circuit of the circulation, interface by interface: left ventricle to arterial system, arterioles to capillaries, the microcirculation and the vascular waterfall, capillaries to the right atrium, venous return, the right ventricle to the left atrium, and the closed loop |
| I11 to I16 | Monitoring: tools, heart-lung interactions, pulse pressure variation, right atrial and CVP waveforms, advanced PA catheter interpretation, cardiac output measurement |
| I17 | Applied cases |

## Evidence standard

Physiology claims are traced to primary literature rather than to secondary
summaries. Every page ends with a numbered reference list, and each reference
has been checked against PubMed. Figures taken or adapted from published work
are credited in their own captions. Where a claim could not be sourced, the
intent is to flag it as such instead of asserting it. If you find a statement
that is wrong, unsupported, or out of date, that is exactly the feedback this
pilot exists to collect.


## Viewing the site

**Read it here: https://nchaisso.github.io/hemosim-web/**

Choose a level on the landing page and read the modules in order.

There is no build step and no framework. The pages are hand-written HTML with
one shared stylesheet, so the site also runs offline: download or clone the
repository and open `index.html` in any browser.

## Repository layout

| Path | Contents |
| --- | --- |
| `index.html` | Landing page and level selector |
| `n*.html`, `i*.html` | The module pages |
| `style.css` | The single shared stylesheet |
| `bannerA.svg`, `bannerB.svg`, `banner-preview.html` | Banner artwork and a page for comparing the two |
| `img/` | Figures used by the pages |
| `CLAUDE.md` | Working instructions for the AI assistant used during the build (see below) |

The drafts, review documents, and tooling behind these pages live in a companion
repository, [hemosim-content](https://github.com/nchaisso/hemosim-content). The
source decks and journal PDFs that originally guided the build are not part of
either repository.

## How it was built

The pages were drafted and assembled from human written content with the help of Claude, an AI assistant
from Anthropic.  The work was done under physician direction. Once drafted, every module goes
through line-by-line review by the authors, and their edits are
applied to the page. `CLAUDE.md` is the standing instruction file for that
assistant. It is left in the repository for transparency about the process.

## Feedback

Corrections and criticism are welcome. Please open an issue on this repository
and name the page and the passage in question.

## Copyright

Copyright 2026, the HemoSim authors. All rights reserved. Figures reproduced or
adapted from published work remain the property of their original publishers and
are credited in their captions.
