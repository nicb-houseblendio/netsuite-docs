# netsuite-docs — Houseblend's local NetSuite documentation corpus

The complete public NetSuite Help Center (docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/) plus
tier-2 reference datasets, stored as one markdown file per topic so AI agents and people can search and
cite it offline. Generated and maintained by the engine in
`houseblend-clients/Templates/netsuite-docs/` — see its `spec.md`, `DESIGN.md` and `README.md`.

- **Never edit corpus files by hand.** A wrong page is re-fetched (`fetch-docs.js --ids <id>`), never patched.
- `index/` and `state/` are generated and git-ignored; `build-index.js` rebuilds the index in minutes.
- Oracle content is Oracle's. This corpus is **internal reference material only**: never redistributed,
  never pasted into client deliverables as-is; every answer cites the public docs.oracle.com URL.
- Layout: `census.json` · `manifest.json` + `manifest/<branch>.json` · `corpus/<branch-slug>/<pageId>.md`
  · `corpus/<branch-slug>/{INDEX.md,llms.txt}` · `dangling.json` · `runs.log` · `tier2/` · `corpus/suiteanswers/`.
- Clone beside houseblend-clients: `C:\Users\beann\github\netsuite-docs` (engine `config.json` → `../../../netsuite-docs`).
