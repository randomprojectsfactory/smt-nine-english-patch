# Applying the patch

This patch produces **Test10 Revision4 Names** from the exact original Japanese XISO below. It includes the earlier fixes; you do not need an older English patch first.

## Required files

- Your original Japanese XISO, matching the source hash and size below.
- `SMT-NINE-English-Test10-Rev4-Names.xdelta` from this repository.
- A 64-bit [xdelta3](https://github.com/jmacd/xdelta/releases) executable. The documented command was verified with xdelta3 3.2.1 on macOS and reproduced the exact output hash. Windows and Linux application remain untested; see `patch-manifest.json` for the verification receipt.

Keep the original image and write the patched image to a separate file. The filenames can differ; the hashes must match. This patch is specific to this XISO layout, so a full-disc dump, another XISO layout or an already-translated image is not the same input.

| File | Bytes | SHA-256 |
| --- | ---: | --- |
| Original Japanese XISO | 2,188,050,432 | `9f040606b4af02a9d8a32d3d0175da189f3556b0c2541d953a39c69bca8c2521` |
| Test10 Revision4 Names output | 2,195,193,856 | `b3907691ef6d78aa0ab4dbd3d088d3a12ef5b070bf0aaa8cd1655bec077c5ec6` |

## Apply

Put the patch and the matching original image in a working folder. Run:

```sh
xdelta3 -d -s "Shin Megami Tensei - Nine (Japan).xiso.iso" "SMT-NINE-English-Test10-Rev4-Names.xdelta" "SMT NINE English Test 10 Revision 4 Names.xiso.iso"
```

On Windows, use `xdelta3.exe` (or `./xdelta3.exe` in PowerShell) in place of `xdelta3`. Leave the source, patch and output arguments in the same order. The output filename must be unused.

## Check the result

Compare the source hash before applying and the output hash afterwards. Check the patch itself against `SHA256SUMS.txt` too.

macOS:

```sh
shasum -a 256 "Shin Megami Tensei - Nine (Japan).xiso.iso"
shasum -a 256 "SMT NINE English Test 10 Revision 4 Names.xiso.iso"
shasum -a 256 -c SHA256SUMS.txt
```

Linux uses `sha256sum` instead of `shasum -a 256`. In PowerShell, use:

```powershell
Get-FileHash -Algorithm SHA256 "Shin Megami Tensei - Nine (Japan).xiso.iso"
Get-FileHash -Algorithm SHA256 "SMT NINE English Test 10 Revision 4 Names.xiso.iso"
Get-FileHash -Algorithm SHA256 "SMT-NINE-English-Test10-Rev4-Names.xdelta"
```

The output is accepted only when its SHA-256 matches the table. A source mismatch or patch error needs to be resolved before testing; forcing the patch is not part of these instructions.

## Use it locally

Select the verified patched XISO in xemu. For original-Xbox HDD testing, extract the verified patched image with your usual XISO tool and copy the complete game folder, including `default.xbe` and `Media/`, to the Xbox. Extraction and transfer are separate steps; the patch is not an HDD installation by itself.

Keep the reconstructed ISO, extracted files and saves on your own devices. This repository contains the patch and notes only. See [TESTING.md](TESTING.md) for the next checks.

Command syntax follows the [xdelta3 documentation](https://jmacd.github.io/xdelta/commandline/).
