# PROJECT_INDEX

Last updated: 2026-07-31 16:07

## Quick Links

- `README.md`
- `docs/START_HERE.md`
- `docs/change_log.md`
- `docs/logs/`

## Managed Tree

<!-- project-tree:start -->
```text
stock-website-pages/
|- assets/
|- data/
|- docs/
|  |- logs/
|  |- START_HERE.md
|- .nojekyll
|- AGENTS.md
|- index.html
|- README.md
```
<!-- project-tree:end -->

## Key Entrypoints

- `index.html`: generated Pages entrypoint
- `assets/`: generated frontend bundle
- `data/`: generated published data
- `../stock-website/tools/publish_github_pages.ps1`: authoritative publication entrypoint

## Ownership Notes

- `assets/`, `data/`, and `index.html` are generated artifacts and are not edited manually.
- `AGENTS.md`, `README.md`, and `docs/` own repository governance.
