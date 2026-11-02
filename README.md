# NYC Building Models

An evolving, AI-assisted reconstruction of real New York City buildings.

The goal is to preserve successive reconstructions as different AI models and methods become available, so anyone can download historical versions and compare their results.

## Scope

This repository distributes standalone building geometry, UVs, materials and textures, together with the minimal license, attribution and version records needed to use them. Game source code, gameplay state, player data, conversations, credentials and private project history are excluded.

**Status:** repository initialized. No building assets have been published yet. Each asset must pass a fresh privacy inspection and a source/license review before publication.

## Building versions

- Each building has a stable public identifier and its own version sequence (for example, `federal-hall-v001`, then `federal-hall-v002`).
- Published versions are retained rather than overwritten. A correction becomes a new version. Each release describes changes from the preceding version; consumers can select an older release.
- Published model assets are intended to be self-contained GLB files using metres and a documented local pivot. Geographic placement and runtime terrain, collision and navigation integration are managed separately by the consuming application. Format and placement compatibility must be checked before replacing an installed model.
- Large model files are distributed as GitHub Release assets; `catalog.json` will index their individual downloads and SHA-256 hashes.
- Version records identify the date, known AI model/provider, format, units, local pivot, appearance changes and relevant source/accuracy limitations. Unverified AI provenance is recorded as unknown rather than guessed.
- Model files contain no game logic. A game or viewer needs a compatible asset downloader and importer to use them; that integration is not supplied by this repository.

Models are reconstructions. A newer version or AI model is not automatically more accurate, and surveyed accuracy is not assumed.

## License

Original contributions are offered under [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/), to the extent the contributors can grant those rights. Credit the project and the relevant contributors, link the license, and indicate modifications. Third-party materials retain their applicable licenses and required attribution; asset-specific notices take precedence where necessary.

Only sanitized asset files and their necessary public records belong here. File extensions alone are not a privacy guarantee: model metadata, image metadata, embedded resources, external paths and commit identity must also be inspected before every synchronization.
