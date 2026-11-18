# Notebook images

The Korean and English participant notebooks load these original image files using HTTPS URLs pinned to a Git commit.

- `common/`: images shared by both languages.
- `ko/`: Korean illustrations.
- `en/`: English illustrations.
- `manifest.json`: image hashes, dimensions, and notebook references.

All 23 images were extracted byte-for-byte from the approved notebooks. No resizing, recompression, or visual edits were applied.

Participants do not need to clone this folder, upload image files, or connect a runtime to view the illustrations. An internet connection and access to `raw.githubusercontent.com` are required.

When revising an illustration, commit its replacement first, then update the corresponding notebook URL to that commit. Existing distributed notebooks keep their pinned image versions.
