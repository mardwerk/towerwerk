# Profile ownership and BTD6 attribution

[td-profile](https://github.com/mardwerk/td-profile) owns the generic Profile Validator, reusable schemas and copyable Profile Template.
[btd6-atlas](https://github.com/KyleDerZweite/btd6-atlas) owns BTD6 captures, source cleanup and its BTD6 Profile.
Tower Generator owns its product rules and any future generation integration.
[Manga Mayhem](https://github.com/mardwerk/manga-mayhem/issues/92) owns its game Profile, Tower files, gameplay and acceptance decisions.

A Profile is a directory selected by its local path.
Keep its dependencies inside that directory and its governed Tower records separate.
Follow the [research boundary](RESEARCH.md#storage-and-update-boundaries) when reusing character evidence.
A new Tower Generator Profile is deferred until generation work resumes.
The [selected authoring editor](PRODUCT.md#selected-authoring-editor-boundary) lives here and uses the external MangaMayhem Profile and game-data.
Its development follows the game-owned playable example and data contract under the [delivery order](PRODUCT.md#established-direction).

The [realignment record](REALIGNMENT.md) documents retirement of the Default Profile/Usopp experiment and its setup.
There is no current validator installation, editor or authoring command in this checkout.
Do not treat its removed schemas, CLI or setup workflow as the future backend contract.
Propose generic checker or reusable schema changes upstream in td-profile; game-specific rules belong to the owning Profile.
Follow the [review instructions](../AGENTS.md) for Kyle's review of future generation mappings and product rules.

## Historical Default Profile

The [complete Default Profile](https://github.com/mardwerk/tower-generator/tree/c7a71f25147ee871bf48790e6e5b0cd6515d8cfa/default/profile) preserves its manifest, local dependencies, schemas and imported notices.
The [historical integration guide](https://github.com/mardwerk/tower-generator/blob/c7a71f25147ee871bf48790e6e5b0cd6515d8cfa/docs/PROFILE.md) records its setup and checks.
The experiment used identity `tower-generator-default`, revision `0.1.0` and checker interface 5.
Its recorded Linux amd64 verification used td-profile v1.0.2, checker 5.0.1, source commit `48fc5daa723d13d89d33bce4a863ba5bf38a1b39`.
This evidence does not establish execution on other platforms or acceptance of gameplay balance.

The experiment copied the Atlas BTD6 Profile at commit [`de82968`](https://github.com/KyleDerZweite/btd6-atlas/tree/de829684232157967fd66f0e999a45df3a669c63/profile), with its own identity and revision.
Its model contracts retain the capture and build provenance below and [imported notices](https://github.com/mardwerk/tower-generator/tree/c7a71f25147ee871bf48790e6e5b0cd6515d8cfa/default/profile/licenses).
Retain source notices when reusing historical material.
Historical records remain evidence, not a selected schema for the new backend or future generation.

## BTD6 source attribution

The historical data reference is capture 56.3, Steam build 24829026, at revision [`a380413`](https://github.com/KyleDerZweite/btd6-atlas/tree/a380413ed809c98654acec7aa37cba40f80bf5c5/data/56.3-build-24829026).
Atlas game data and derived tables are licensed CC BY-NC 4.0.
Cite capture, build, actual source commit and source files when importing or using values.
Keep generated records local and ignored by Git; do not publish the BTD6 corpus in this repository.

Atlas's BTD6 Profile describes BTD6 data and is separate from td-profile's generic Profile Template.
Dart Monkey's Atlas verification remains accepted reference evidence.
The [older generator attribution](https://github.com/mardwerk/tower-generator/blob/generator-before-validator-reset-2026-09-29/docs/BTD6-REFERENCE.md) preserves its source mappings and deliberate departures.

### Retained historical catalogue

The [cold-store upgrade catalogue](research/materials/99-cold-store/upgrade_catalog.csv) is preserved source evidence, not a current Atlas capture or a supported game-data import.
Its SHA-256 is `0d9505b191318cc14abf16504778f085dbce146afd1cc617e56770815486cec0`, matching the [snapshot provenance record](research/materials/20_knowledge/btd6-snapshot.md#raw-evidence).
Its 390 rows cite [Cyber Quincy costs](https://github.com/hemisemidemipresent/cyberquincy/blob/master/jsons/costs.json) in `cost_source` and [Btd6ModHelper game-data](https://github.com/Btd6ModHelper/btd6-game-data) tower exports in `mechanic_source`.
Those CSV URLs name moving branches and do not establish the original source revisions.

On 2026-10-28, GitHub identified Cyber Quincy's repository licence as AGPL-3.0 in [LICENSE.md](https://github.com/hemisemidemipresent/cyberquincy/blob/master/LICENSE.md); the Btd6ModHelper game-data licence endpoint returned HTTP 404.
Neither result establishes permission to redistribute this derived table or a licence for its game content.
The Atlas CC BY-NC 4.0 statement above does not establish a licence for this independently sourced catalogue.
[Issue #132](https://github.com/mardwerk/towerwerk/issues/132) owns the unresolved source-permission and retention decision.
This clarification preserves the existing evidence without selecting a publication exception or authorizing new generated data in Git.
