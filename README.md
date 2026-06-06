# LDAME
The MAME of LaserDisc: preserving disc behavior, navigation, audio, and experience beyond the original hardware.
LDAME
LaserDisc Archive & Media Emulator

LDAME is an open preservation and playback framework designed to preserve the experience of LaserDisc, not just its video signal.

Inspired by the role that MAME plays in arcade preservation, LDAME seeks to provide a portable, future-proof representation of LaserDisc titles that preserves their structure, navigation, audio options, and unique behaviors while allowing multiple video sources to be used.

Vision

Traditional LaserDisc preservation focuses on preserving the original signal:

RF captures (Domesday Duplicator)
ld-decode outputs
Video transfers
Audio extraction

LDAME focuses on preserving the disc experience:

Chapter structure
Side changes
Frame numbering
Audio track selection
Commentary tracks
Still frames
CAV-specific functionality
Disc metadata
Player navigation behavior

while optionally allowing replacement or enhancement of the underlying video source.

Design Philosophy

LaserDisc titles contain much more than a movie.

Many releases include:

Alternate audio tracks
Commentary tracks
Unique chapter layouts
Frame-accurate navigation
Side break placement
Interactive content
Supplementary galleries
Special authoring choices

These elements are often lost when content is converted to modern containers such as MKV.

LDAME aims to preserve those elements as first-class features.

Goals
Preserve
Original RF captures
ld-decode metadata
Frame numbering
Disc TOC information
Chapter maps
Side structure
Audio track definitions
Commentary metadata
Still-frame locations
Interactive disc behavior
Support Multiple Video Sources

An LDAME title may reference:

Original ld-decode video
MUSE-decoded video
Blu-ray sources
UHD sources
Fan restorations
Future remasters

The playback engine maps those sources onto the original LaserDisc timing and navigation model.

Frame-Based Architecture

LaserDisc is fundamentally frame-addressable.

LDAME uses frame numbers as its primary timeline rather than timestamps whenever possible.

Example:

Frame 000000  Start of disc
Frame 051234  Chapter 18
Frame 054000  Side A ends
Frame 054001  Side B begins

This enables accurate emulation of:

CAV frame stepping
Chapter search
Side transitions
Audio synchronization
Layered Preservation Model
Layer 1 — Archive

Preserves original media:

RF captures
Disc metadata
Checksums
Decoding parameters

This layer remains immutable.

Layer 2 — Experience

Preserves user-visible behavior:

Chapters
Navigation
Side changes
Audio routing
Commentary selection
Galleries
Layer 3 — Presentation

Provides one or more video sources:

Original decoded video
Enhanced video
Blu-ray replacement
UHD replacement
Future restorations

The presentation layer may evolve while archive and experience layers remain intact.

Example Use Case

A collector owns a DTS LaserDisc release.

LDAME could preserve:

Original DTS audio
Original PCM audio
Original chapter structure
Original side breaks
Original frame numbering

while displaying:

A modern Blu-ray transfer
A UHD remaster
A future restoration

The title still behaves like the original LaserDisc.

Long-Term Goal

Create a platform-independent "virtual LaserDisc" format that preserves:

The disc
The authoring
The navigation
The audio
The collector experience

without requiring future users to possess original LaserDisc hardware.

Relationship to Existing Projects

LDAME is intended to complement, not replace:

Domesday86 Project
ld-decode
VHS-Decode
Existing archival efforts

Those projects preserve the original signal.

LDAME aims to preserve and emulate the complete LaserDisc experience built on top of that signal.

Why the Name?

LDAME is inspired by MAME (Multiple Arcade Machine Emulator).

Where MAME preserves arcade machines and their behavior, LDAME seeks to preserve LaserDisc titles and their behavior.

The goal is not merely to play video files, but to preserve the experience of interacting with a LaserDisc title for future generations.
