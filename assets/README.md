# Image assets

The Korean and English participant notebooks load these original image files using HTTPS URLs pinned to a Git commit.

- `common/`: images shared by both languages.
- `ko/`: Korean illustrations.
- `en/`: English illustrations.
- `readme/`: the event banner used by the README guides.
- `manifest.json`: image hashes, dimensions, and notebook or document references.

All 23 notebook illustrations were extracted byte-for-byte from the approved notebooks. The provided event banner in `readme/` is also preserved byte-for-byte. No resizing, recompression, or visual edits were applied.

Participants do not need to clone this folder, upload image files, or connect a runtime to view the illustrations. An internet connection and access to `raw.githubusercontent.com` are required.

When revising an illustration, commit its replacement first, then update the corresponding notebook URL to that commit. Existing distributed notebooks keep their pinned image versions.
