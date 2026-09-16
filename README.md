# AI News by Carni — Storyboard Review frontend

This repository is the **public frontend shell** for the wider AI News by Carni system.

Deployed review UI:
`https://review.carni.ltd/`

## Repository role

Owns:
- the public Storyboard Review frontend shell;
- browser-facing assets/code required by that shell.

Does **not** own:
- global project state;
- Storyboard approval contract;
- production review/publisher state;
- Shorts Factory strategy;
- global working memory.

The production approval/state logic lives in the private control-plane repository and Supabase.

## Global source of truth

Use:

`DmitryCarni/ai-news-by-carni-private`

Startup packet for cross-project work:

1. `README.md`
2. `docs/PROJECT_INDEX.md`
3. `docs/WORKING_STATE.md`
4. `docs/KNOWLEDGE_BASE_MAP.md`

Storyboard-specific contracts are routed from that knowledge-base map.

Do not maintain a second global project-state file here.

## Boundary

This repo may document **local frontend implementation details**.

If a local README/comment conflicts with the private repo's current Storyboard contract or verified production state, the verified production state/private control-plane contract wins.
