# AI News by Carni — Reviewer frontend

Этот репозиторий содержит публичную frontend-оболочку Reviewer.

URL:

`https://review.carni.ltd/`

## Роль репозитория

Здесь живут:
- browser-facing UI;
- frontend assets;
- routing к production Edge Functions.

Здесь **не хранится глобальная база знаний проекта** и не определяется production approval contract.

Канонический источник:

`DmitryCarni/ai-news-by-carni-private`

База знаний:

`DmitryCarni/ai-news-by-carni-private/docs/`

Для Reviewer/Storyboard/thumbnail/video flow использовать:

`docs/knowledge/04_SHORTS_И_REVIEWER.md`

Для current state:

`docs/knowledge/02_ТЕКУЩЕЕ_СОСТОЯНИЕ.md`

## Граница ответственности

Frontend отображает и отправляет действия пользователя.

Production state, immutable approvals, Storyboard revisions, thumbnail state и publisher state находятся в Supabase/private control plane.

Если local UI assumption расходится с live backend contract — приоритет у проверенного live state и private repo.

## Язык документации

README и техническая документация ведутся на русском.

Technical identifiers, API names, paths, enum, variable names и строки, которые должны совпадать с кодом, не переводятся.
