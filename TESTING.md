# Testing

**Test10 Revision4 Names is awaiting its first original-Xbox hardware test.** Native text/history checks and local package verification passed. These checks use bounded test scenes and modeled graphics interfaces, so they cannot establish how the text looks on a real display or whether every scene progresses.

Earlier user xemu testing passed the reported Bureau stall, continued into the early story and exercised English recruitment. The final candidate needs its own gameplay check.

## Before testing

Follow [PATCHING.md](PATCHING.md) and verify the original input and patched output hashes first. Keep a spare copy of your normal save and use one complete build at a time. Restart the emulator with the new image and load an in-game save; an older emulator snapshot retains old code in memory. For Xbox HDD testing, extract the verified patched image into a separate, complete game folder.

## What to check

- Dense dialogue at 480p with your intended CRT or mask settings: squeezed letters, missing words, uneven line breaks and text near screen edges.
- Bureau conversations, speaker names and continuation pages. Longer legacy player names can still cause extra squeezing; 18 already-condensed contexts become slightly wider after the spelling fixes.
- Progression across chapters and both protagonist routes as testing continues, including dialogue history and the earlier stall location.
- Menus, party statistics, map directions, battle labels, hacking tutorials/results and recruitment branches encountered naturally.
- Normal saving, a full restart and loading the save again.

Some layouts remain outside automatic reflow, and some optional negotiation responses remain Japanese. A successful short run does not establish complete coverage.

## About xemu reports

User testing has shown **many visual errors, slowdowns and animation problems in xemu**. Compare reproducible issues with the Japanese game using the same settings before deciding whether the emulator or patch is responsible.

Reports should include the candidate/output hash, route, name length, emulator version or Xbox setup, video/display settings and steps to reproduce. Describe the location without quoting story dialogue. Keep saves, ISOs and extracted game files out of the repository.
