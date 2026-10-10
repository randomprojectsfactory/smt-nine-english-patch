# SMT NINE English Patch

This is a work-in-progress English patch for the Japanese Xbox release. **Test10 Revision4 Names** is the current candidate; its first original-Xbox hardware test is still pending.

The current work covers story dialogue, menus, battle text, hacking tutorials and location/navigation names. Tested recruitment conversations work in English, but some optional negotiation responses remain Japanese. Text baked into scenery and the original name-entry keyboard are outside this pass. English drafts and technical work were assisted by Codex.

## Making the text work

English needed more than replacing Japanese strings. Font-cell bounds, spacing and centering were corrected; menu wording was shortened and dialogue lines redistributed to fit their boxes. A dialogue-history buffer fix resolved a reproduced stall caused by longer English entries. Tsuzumi and Ferris now use consistent spellings across both routes.

Native text checks and local package verification passed. Earlier user emulator testing confirmed progress beyond the reported stall and sampled recruitment. The final candidate still needs gameplay testing. Dense dialogue can remain squeezed, some line breaks need polish, and blue backgrounds/pointers can misalign near screen edges. Later chapters and both routes still need playing through.

In user testing, **xemu has shown many visual errors, slowdowns and animation problems**. Compare an issue with the Japanese game before attributing it to the translation. Original hardware will be especially useful for judging 480p/CRT readability.

## Patch files only

**No ISO or extracted game files belong in this repository.** Use your own exact matching original Japanese XISO. [PATCHING.md](PATCHING.md) contains the source/output hashes and `xdelta3` instructions. See [TESTING.md](TESTING.md) for checks and [CHANGELOG.md](CHANGELOG.md) for revision details.
