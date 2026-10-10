# Changelog

These are development test revisions, not completed public releases. Counts below describe reviewed page contexts or changed records within each pass, including both routes where applicable. They must not be added together as a whole-game dialogue total.

## Test10 Revision4 Names — 2026-10-10

Current private pre-release and first original-hardware test candidate, based on verified Revision4.

- Standardized Tsuzumi and Ferris across both routes and executable actor-name data: 688 live script records and 12 fixed name fields changed.
- Used eight source-reviewed compact records and two word-preserving call-page reflows to prevent the longer names from causing new condensation in supported name fixtures.
- Preserved every other executable byte and all script instructions, controls and record counts. Renderer and history behavior remain identical to Revision4.
- Independent native checks and full local ISO/HDD package verification passed. Gameplay and hardware confirmation for this candidate remain pending.
- Eighteen previously condensed page contexts become slightly wider; existing dense dialogue still needs a readability review.

## Test10 Revision4 — 2026-10-10

- Applied 1,273 reviewed word-preserving reflows: 1,245 field and 28 story contexts, including 657 continuation pages.
- Extended supported layouts to the source's default auxiliary actor and bounded name/surname variables. Guarded variable layouts against worsening shorter supported names.
- Applied 64 source-reviewed compact-copy contexts, covering 26 distinct English versions, where wording changes were needed for readability.
- Addressed the reported dense Bureau continuation page in both protagonist routes. Its revised layout fits normal width for names entered through the ordinary native keyboard; wider legacy names can still condense.
- Changed script text only. The Revision3 executable and its renderer/history safeguards were retained unchanged.
- Preserved event instructions, branches, controls, page boundaries and text-record counts. Unsupported or ambiguous layouts remained outside automatic reflow.

## Test10 Revision3 — 2026-10-10

- Applied 623 reviewed word-preserving dialogue reflows across both routes. Of those contexts, 425 fit normal horizontal font size under the conservative guard budgets.
- Rejected awkward proposed breaks to retain clearer names, phrases, lists and deliberate speech beats.
- Separately corrected three source-checked wording problems in 13 records.
- Kept the Revision2 executable unchanged. This pass was limited to recognized layouts with unambiguous references.

## Test10 Revision2 — 2026-10-10

- Rewrapped 442 hacking message pages and adapted the result-bonus label.
- Added horizontal fitting to audited shared dialogue paths, with stable scaling throughout a typewriter page.
- Improved blue dialogue width metadata and onscreen text positioning. Original background/pointer anchoring remained unchanged.
- Improved chapter-end wording, shared menu centering, Setup/Demons labels, party-stat spacing, front-position terminology and shop-role labels.
- Reviewed 99 location entries against Japanese context and recorded reusable direction, station-plaza, street and junction terminology.
- Retained the history fix and original font textures. Very long text could still condense.

## Test10 Revision1 — 2026-10-10

- Repaired a reproduced overlapping dialogue-history copy defect triggered by a full English history entry.
- Made the shared history paths shift fixed slots safely and retain long entries across continuation slots. Longer entries can displace older backlog entries sooner.
- Reworked the opening Bureau introduction and recruitment text in both routes while preserving event instructions and nontext sections.
- Earlier user xemu testing subsequently confirmed passage beyond the reported stall, further early-story progress and sampled English demon recruitment.

## Test10 foundation — 2026-10-10

- Corrected Latin glyph texture bounds and pixel-center alignment while preserving the original font artwork.
- Preserved fractional advances for compressed text and improved combat label centering.
- Improved location/navigation labels and compact status/equipment terminology, and retained the English hacking resource/loader work from earlier builds.

Native routine and package checks throughout this history are bounded engineering evidence. They do not establish a complete playthrough or original-hardware validation.
