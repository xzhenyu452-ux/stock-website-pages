# Stock Website Pages

Last updated: 2026-07-31 16:07

## Purpose

This repository contains generated GitHub Pages artifacts. Business source belongs to `stock-website`; publication must use `stock-website/tools/publish_github_pages.ps1` rather than hand edits here.

## Start Here

- Read `docs/START_HERE.md` for the first-pass workflow.
- Read `docs/PROJECT_INDEX.md` for the file and folder map.

## Key Areas

- `assets/` generated frontend assets
- `data/` generated published snapshots
- `docs/` repository governance records

## Change Management

Every substantive change should also update:

- `docs/change_log.md`
- one graded log under `docs/logs/`

## Notes

用户明确声明“此会话任务完结”时，按 `AGENTS.md` 同步任务记录、验证、提交并推送任务分支，再串行合并 `main` 和更新根仓库指针；该表达不自动触发 Pages 发布。
