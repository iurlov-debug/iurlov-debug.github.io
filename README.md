# Earth Memory Archive v1.0

Статический сайт на Jekyll для GitHub Pages. Архив знаний исследовательской команды.

## Быстрый старт (5 минут)

### 1. Создайте репозиторий
- Название: `yourusername.github.io` (или любое другое)
- Публичный (Public)

### 2. Загрузите файлы
- Откройте репозиторий → **Add file** → **Upload files**
- Перетащите ВСЕ файлы и папки из этого архива
- **Commit changes**

### 3. Включите GitHub Pages
- Settings → Pages (боковое меню)
- Source: **Deploy from a branch**
- Branch: **main** / **root**
- **Save**
- Через 2–3 минуты: `https://yourusername.github.io`

### 4. Настройте (опционально)
Откройте `_config.yml` и измените:
```yaml
url: "https://yourusername.github.io"
```

## Структура

```
├── _characters/          # Горн, Архивариус, Биолог
├── _episodes/            # Выпуски с источниками
├── _layouts/             # Шаблоны страниц
├── assets/css/           # Стили (полевой дневник)
├── index.md              # Главная — команда
└── _config.yml           # Настройки + коллекции
```

## Важно: коллекции включены

В `_config.yml` прописано:
```yaml
collections:
  characters:
    output: true
    permalink: /characters/:path/
  episodes:
    output: true
    permalink: /episodes/:path/
```

Без этого GitHub Pages НЕ создаст страницы для персонажей и выпусков.

## Добавление нового выпуска

1. Создайте файл `_episodes/YYYY-MM-DD-title.md`
2. Скопируйте front matter из `_episodes/2026-07-26-amethyst.md`
3. Заполните `sources:` и `fact_check:`
4. Загрузите через GitHub web UI → Commit
5. Сайт обновится автоматически через 1–2 минуты

## Работа с AI (как я буду помогать)

Я генерирую готовые Markdown-файлы. Вы загружаете их через веб-интерфейс GitHub.

**Пример:**
- Вы: «Новый выпуск про вулканы»
- Я: создаю `_episodes/2026-08-01-volcanoes.md` + обновлённые sources
- Вы: drag-and-drop на github.com → Commit
- GitHub Pages: автосборка
