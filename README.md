# Планировщик — Telegram Mini App

Личный планировщик: календарь, трекер привычек и идеи. Одна страница `index.html`, открывается кнопкой меню в Telegram-боте.

Данные хранятся в облаке Telegram (у каждого пользователя своё) и копией на устройстве. Токен бота здесь не нужен и не хранится.

## Как выложить на GitHub Pages (один раз)

1. **GitHub Desktop → войти в нужный аккаунт.** Меню GitHub Desktop → Settings → Accounts. Если там старый аккаунт — Sign out, потом Sign in to GitHub.com новым. Во вкладке Git там же выбрать почту нового аккаунта.
2. **Добавить папку.** File → Add Local Repository → Choose… → папка `Documents/GitHub/planner` → появится надпись, что это ещё не репозиторий, — нажать **create a repository** → Create Repository.
3. **Первый коммит.** Внизу слева в поле Summary написать «Этап 1: каркас» → Commit to main.
4. **Опубликовать.** Кнопка **Publish repository** сверху. Снять галочку **Keep this code private** (бесплатный GitHub Pages работает только с открытыми репозиториями) → Publish.
5. **Включить сайт.** Repository → View on GitHub → вкладка **Settings** → слева **Pages** → Source: *Deploy from a branch*, Branch: **main**, папка **/(root)** → Save.
6. Через 1–2 минуты там же появится адрес вида `https://ЛОГИН.github.io/planner/`. Открыть его в браузере — должна показаться страница с вкладками.

## Как подключить к боту

1. В Telegram открыть **@BotFather**. Если бота ещё нет — `/newbot` и следовать подсказкам.
2. `/mybots` → выбрать бота → **Bot Settings** → **Menu Button** → **Configure menu button**.
3. Отправить адрес страницы (`https://ЛОГИН.github.io/planner/`), потом название кнопки, например «Планировщик».
4. Открыть чат с ботом — слева от поля ввода появится кнопка «Планировщик».

Токен, который выдаёт BotFather, никуда не вставляем и никому не показываем.

## Как обновлять

Изменили файл → GitHub Desktop → Commit to main → **Push origin**. Сайт обновится через 1–2 минуты. Если в Telegram видна старая версия — закрыть мини-приложение и открыть снова.
