# LDAME Architecture

## Core Principle

Separate LaserDisc preservation into three independent layers:

1. Archive
2. Experience
3. Presentation

The Archive and Experience layers remain stable over time while the Presentation layer may be replaced as improved video sources become available.

---

## Layer 1: Archive

The Archive layer preserves the original media and technical information.

Examples:

- RF captures
- Disc metadata
- Checksums
- Decoding parameters
- Preservation records

This layer should remain immutable whenever possible.

---

## Layer 2: Experience

The Experience layer preserves how the LaserDisc behaves.

Examples:

- Chapter navigation
- Frame numbering
- Side changes
- Audio track selection
- Commentary tracks
- Still frames
- Disc-specific interactive behavior

This layer defines what makes a title feel like a LaserDisc.

---

## Layer 3: Presentation

The Presentation layer provides one or more video sources.

Examples:

- Original ld-decode output
- MUSE-decoded video
- Blu-ray sources
- UHD sources
- Future restorations

Presentation sources may improve over time while Archive and Experience remain unchanged.

---

## Design Goal

Preserve the LaserDisc experience independently of any specific video source.

A user should be able to experience a title's original navigation, chapter structure, side changes, audio options, and behavior whether the presentation source is an RF decode, a Blu-ray transfer, or a future restoration.
