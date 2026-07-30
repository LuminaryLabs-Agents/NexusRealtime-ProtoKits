# NexusEngine ProtoKits Visual Assets

A proving ground for reusable NexusEngine Domain Service Kits, where capabilities are composed, validated, and prepared for evidence-backed promotion.

## Files

- `logo-source.png`: retained chroma or alpha source.
- `logo-transparent.png`: full-resolution transparent mark.
- `logo-mask.png`: grayscale alpha mask.
- `logo-mask.svg`: editable single-color SVG wrapper; change the rectangle fill.
- `logo-1024.png`, `logo-512.png`, `logo-256.png`: padded transparent variants.
- `cover-1280x640.png`: normalized repository cover.
- `social-card.png`: cover composed with the repository mark.
- `manifest.json`: generation settings, hashes, dimensions, and validation.

`cover-source.png` preserves the selected generated cover.

## Usage

Use the transparent PNGs on arbitrary backgrounds. Use `logo-mask.svg` when the
mark color must remain editable. Do not stretch, crop, rotate, add effects, or
place the mark over low-contrast imagery.

## Regeneration

Regenerate through the Repo Image Studio plugin and review every replacement
before merging. Existing assets must not be overwritten without explicit
replacement approval.
