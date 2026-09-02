# PIXEL RAMP SNES REMASTER TOOL KIT 

A realtime remaster look for Super Nintendo games, running inside a patched [Snes9x](https://github.com/snes9xgit/snes9x) rather than as a screenshot filter.

The look is **Pixelramp**: palette-aware upscale (2× or 8×), bloom, distance light-cast, optional layer-Z, and per-object sprite rules (lamps, muzzle flashes, and similar authored highlights). It started as an offline Python prototype and now runs as an in-emulator GPU path on Windows (D3D11).

This GitHub copy is a placeholder for now. The working tree on disk is larger than what is published here.

[![Watch the video](https://img.youtube.com/vi/f5eBDgdht-A/maxresdefault.jpg)](https://www.youtube.com/watch?v=f5eBDgdht-A)

<img width="1434" height="807" alt="Thumbnail Pixel 169" src="https://github.com/user-attachments/assets/9d149fb3-978f-4ae7-a0a6-6dab2e54c34c" />


## What lives in the local project

| Piece | Role |
|---|---|
| `snes9x-1.63/` | Forked Snes9x with Pixelramp in the video-filter dropdown |
| `native/pixelramp_gpu/` | Shared analyze + D3D11 compute core (also a standalone viewer) |
| `csharp/` | Remaster Studio — one Avalonia executable for painting sprite rules |

Snes9x is the host. Remaster Studio is the authoring tool a player would actually run. Python stays for goldens and experiments, not for shipping.

## Status

Active research / prototype. Not a public release. Game ROMs are not part of this repo.

Source for the emulator, filter, and studio will land here when the tree is cleaned up enough to share.
