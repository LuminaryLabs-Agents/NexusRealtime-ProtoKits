# Visual Identity

## Concept

NexusEngine ProtoKits is represented as a modular foundry. Small reusable
capability blocks enter a shared composition and validation path, then resolve
into larger connected domain clusters. The imagery reflects the repository's
documented role as a proving ground; it does not imply that every ProtoKit is
stable or promoted.

The compact mark combines one central kit socket with three connected modules.
Its open connection points represent composition, while the branching layout
represents a kit growing into a broader domain.

## Palette

| Role | Color |
|---|---|
| Deep technical background | `#071B33` |
| Warm module accent | `#F28C28` |
| Connection and validation accent | Electric cyan |
| Neutral structure | Off-white |

The orange and cyan contrast separates authored modules from their connections
without assigning maturity or promotion status by color.

## Asset Set

Assets are indexed in [`docs/assets/brand/README.md`](assets/brand/README.md):

- transparent logo source and 256, 512, and 1024 pixel variants;
- grayscale alpha mask and editable single-color SVG mask;
- normalized 1280 by 640 cover and social card; and
- a versioned manifest containing generation settings, dimensions, alpha
  evidence, and SHA-256 hashes.

## Usage

- Use `logo-transparent.png` on arbitrary backgrounds.
- Use `logo-mask.svg` when a single-color treatment is required.
- Use `social-card.png` for repository previews and public project links.
- Preserve the mark's clear space, orientation, and three-branch silhouette.
- Do not stretch, crop, rotate, add text, or add effects to the mark.
- Provide meaningful alternative text whenever an asset is embedded.

## Regeneration

Regenerate the complete set through Repo Image Studio and review replacements
before merging:

```bash
export REPO_IMAGE_STUDIO="/path/to/repo-image-studio"

python3 "$REPO_IMAGE_STUDIO/scripts/build_image_pack.py" build \
  --logo-source <logo-source.png> \
  --cover-source <cover-source.png> \
  --out-dir docs/assets/brand \
  --project-name "NexusEngine ProtoKits" \
  --summary "A proving ground for reusable NexusEngine Domain Service Kits, where capabilities are composed, validated, and prepared for evidence-backed promotion." \
  --primary-color F28C28 \
  --background-color 071B33 \
  --logo-position top-center \
  --logo-size 320

python3 "$REPO_IMAGE_STUDIO/scripts/build_image_pack.py" validate \
  --pack-dir docs/assets/brand
```

Repo Image Studio is a maintainer tool, not a package or runtime dependency.
