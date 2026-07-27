# Earth Memory Studio — GitHub Pages

Полевой дневник исследовательской команды Earth Memory Studio.

## Структура

```
.
├── _config.yml              # Конфигурация Jekyll + коллекции
├── _data/
│   └── sources.json         # Проверенные источники по выпускам
├── _characters/
│   ├── gorn.md              # Горн — геолог
│   ├── archivist.md         # Архивариус — кот
│   └── biologist.md         # Биолог
├── _episodes/
│   └── 2026-07-27-amethyst.md   # Выпуск 01: Аметист
├── _layouts/
│   ├── default.html         # Базовый шаблон
│   ├── episode.html         # Шаблон страницы выпуска
│   └── character.html     # Шаблон страницы персонажа
├── assets/css/
│   └── style.css            # Стили «полевой дневник»
└── index.md                 # Главная страница
```

## Как обновить сайт

1. Отредактируйте файлы Markdown в `_episodes/` или `_characters/`
2. Обновите `_data/sources.json` при добавлении новых источников
3. Загрузите изменения в репозиторий GitHub
4. GitHub Pages автоматически пересоберёт сайт (1–2 минуты)

## Правила верификации

- Все факты должны иметь источник с `authority: peer_reviewed` или `primary_historical`
- Легенды и мифы обязательно помечаются `[ЛЕГЕНДА/ДЕБАНК]`
- Температурные/числовые данные — только из peer-reviewed источников
- Все URL проверены на доступность
- Ошибки исправляются с указанием даты коррекции

## Деплой

Сайт живёт на: https://iurlov-debug.github.io
