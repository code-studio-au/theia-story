# Migration from theia-mmo

27 November 2026 — repository separation requested by the creator.

Imported 201 Markdown documents and 5 supporting JSON files from
`theia-mmo/docs/story/` at source commit `464d29891f41fcc802dfd8df39e68c552880e890`. Their paths below that
directory are preserved at this repository's root. Zone/location briefs,
NPC/character cards, dialogue, campaign reviews, canon decisions and source
recovery records are included. The JSON files preserve editorial inventories,
dependencies, draft decisions and the original Engine import provenance.

The source is the [theia-mmo story tree at the migration revision](https://github.com/code-studio-au/theia-mmo/tree/464d29891f41fcc802dfd8df39e68c552880e890/docs/story).
[MIGRATION_MANIFEST.json](MIGRATION_MANIFEST.json) records every original path,
destination and source/destination SHA-256. Most files are byte-identical;
changes are limited to cross-repository link destinations, the README and the
new repository-location decision. No narrative or quest data was reconciled.
The original `IMPORT_MANIFEST.json` remains unchanged as historical evidence.

This repository starts with a snapshot import. Earlier commits and retired
documents remain in `theia-mmo` history, and their commit-pinned provenance
links remain intact. Historical references to the old `docs/story/` location
describe that history and are not the current checkout path.

Use sibling checkouts named `theia-story` and `theia-mmo`. Links from story
documents to implementation records point into `../theia-mmo/docs/` (with
appropriate traversal for nested documents). The game's runtime code, content
assets, zone/editor implementation notes and NPC/character system documentation
remain in the MMO repository.

Local Copilot caches, agent skill symlinks and ignored private conversations
were not imported or deleted; they remain in the original checkout. The initial
migration was local. On 27 November 2026, the creator subsequently authorized
committing and pushing both repositories. This repository will be published as
private at [code-studio-au/theia-story](https://github.com/code-studio-au/theia-story)
on `main`; the MMO migration uses its existing `feat/website-character-roster`
branch.
