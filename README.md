# GlancEhr — Releases

The automated club player of the Glance family: drop a folder, it plays.

This repository hosts signed, notarized DMG releases of GlancEhr for macOS.
The source code is private. Bug reports and feature requests are welcome via the [Issues tab](../../issues).

## Download

Current version: **GlancEhr 1.0.0** — [GlancEhr-v1.0.0.dmg](https://github.com/AmritusG/glancehr-releases/releases/download/v1.0.0/GlancEhr-v1.0.0.dmg) ([SHA-256](https://github.com/AmritusG/glancehr-releases/releases/download/v1.0.0/GlancEhr-v1.0.0.dmg.sha256), [release notes](https://github.com/AmritusG/glancehr-releases/releases/tag/v1.0.0))

All versions are on the [Releases tab](../../releases).

## What it is

Drop a folder of clips on GlancEhr. Every file is checked first; the ones that can play are played in random order,
joined by automatic transitions (356 of them, picked so the same one never comes twice in a row), with a dark clip never
cut straight into a bright one. Send To puts the show full screen on a second screen and keeps it there: unplug the
screen and plug it back, and the show returns to it. It keeps the Mac awake while it plays, can start at login, and a
watchdog restarts it if it ever crashes or hangs, back on the same clip.

It plays DXV1 / DXV3 and HAP (Hap1, Hap5, HapY, HapM) natively, alongside what macOS plays itself (H.264, HEVC,
ProRes), plus still pictures.

**Windows and iPhone / iPad are coming.**

## Installing

1. Download the `.dmg`
2. Double-click to mount
3. Drag `GlancEhr.app` into your Applications folder
4. First launch: macOS verifies the signature and notarization, then opens

## Requirements

- macOS 14 (Sonoma) or later
- Apple Silicon or Intel Mac

## Reporting issues

Please open an [Issue](../../issues) with your macOS version (`sw_vers`), the GlancEhr version (About menu), the steps
to reproduce, and a screenshot or recording if it is visual.

## License

GlancEhr binaries are distributed for personal and commercial use. The open-source notices (the transitions' sources
and the Rust crates) are inside the app, in `GlancEhr.app/Contents/Resources`, and in this repository
(`ATTRIBUTION.md`, `THIRD-PARTY-CRATES.md`).
