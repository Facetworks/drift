# Changelog

All notable changes to this project are documented here, following
[Keep a Changelog](https://keepachangelog.com/) and semantic versioning.

## [0.2.0] - 2026-09-06

### Fixed
- No longer hard-requires float blending: 8-bit accumulation trails with matched tone mapping on phones that lack EXT_float_blend.
- Mobile scaling: 16k particles (was 65k), smaller trail buffer, shorter warmup, DPR capped at 1, live count in the header.
- Time-based fade and deposit gain, so 90/120Hz phones match 60Hz; bounded hash time input for weak mobile sin().
- Balanced deposit gain for dark backgrounds with bright cores.
- Toolbar scrolls on narrow screens; viewport-fit cover; safe pointer capture; context-loss fallback.

## [0.1.0] - 2026-09-05

### Added
- Initial release: curl-noise flow-field particles in one HTML file.
