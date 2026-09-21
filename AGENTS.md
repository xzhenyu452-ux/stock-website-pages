# GitHub Pages artifact repository contract

## Repository ownership

- This repository contains generated GitHub Pages artifacts. It is not a business-source or feature-development repository.
- Do not hand-edit generated assets. Source changes belong in `../stock-website` and publication must use `../stock-website/tools/publish_github_pages.ps1`.
- `main` is the authoritative Pages branch. A published commit must be traceable to the tested website source commit.

## Mandatory task planning and closure

- The root `../tools/task_registry.ps1` and `../docs/ACTIVE_TASKS.md` govern every planned publication or maintenance change.
- Before changing this repository, register exact scope paths, source backlog/task ID, owner, branch/worktree, and deployment need; stop on uncoordinated conflicts.
- Routine publication is serialized by one release owner. Validate the website source first, build with the Pages base path, and inspect the generated diff before commit.
- Mark `ready_to_merge` only after artifacts are generated, checked, committed, and pushed without manual edits or unrelated files.
- Mark `deployed` only after GitHub Pages serves the expected commit/assets and HTTP verification passes. Record source and Pages commit SHAs in the owning source/deployment change log before completing the registry entry.
- If the user explicitly says `此会话任务完结`, `本会话任务完结`, or an unambiguous equivalent, synchronize the task table/registry and logs, validate the scoped change, commit and push the task branch, then merge and push authoritative `main` and update the root gitlink. This phrase does not authorize publishing Pages or hand-editing generated assets.

## Recovery

- If publication fails, do not patch assets manually. Fix the source or publication script and regenerate.
- To recover, republish a previously verified source/Pages revision through the documented script and verify the live site.

## Git usage rules

- `main` is the Pages authority; `master` is not an alias. Business development never occurs here.
- Maintenance uses a registered task branch/worktree. Routine generated publication is serialized by the release owner, who may update main only after source validation and generated-diff review.
- Stage only generated files owned by the publication. Record website source SHA and Pages SHA; never hand-edit, mix unrelated artifacts, rewrite main, force push, or move a published tag.
- Recover by regenerating or republishing a verified revision, not by patching live assets. Full rules: `E:/Codex/Instructions/Git多仓库与多会话开发规范.md`.
