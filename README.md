# AI News by Carni — Reviewer frontend

Этот репозиторий содержит публичную frontend-оболочку Reviewer.

Production UI:
`https://review.carni.ltd/`

## Роль репозитория

Здесь живут:
- browser-facing frontend;
- GitHub Pages assets;
- код оболочки Review control center.

## Граница ответственности

Этот репозиторий **не ведёт отдельную глобальную базу знаний**.

Здесь не должны дублироваться:
- production approval contracts;
- Shorts Factory architecture;
- глобальный current state;
- publisher state;
- Supabase state;
- стратегическая память проекта.

Каноническая база знаний:
`DmitryCarni/ai-news-by-carni-private/docs/knowledge/`.

Стартовый порядок:
1. `PROJECT.md`;
2. `CURRENT_STATE.md`;
3. `SHORTS_PRODUCTION.md` для Reviewer/Storyboard/thumbnail/video задач.

## Источник истины

Если frontend README или comment расходится с production:
`проверенное живое состояние > private knowledge base > локальный comment`.

Production approval/state logic хранится в private repo и Supabase.
