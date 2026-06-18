# RevenueSprint 48: запуск и Railway

Эта папка `leadrescue-48` самостоятельная, но в корне проекта также есть wrapper-конфиг для Railway.

## Локальный запуск

```bash
npm install
npm start
```

Открой:

```text
http://localhost:3000
```

Если `DATABASE_URL` не задан, данные будут храниться локально в `data/revenuesprint.json`.

Опциональные лимиты для безопасного сканера:

```text
MAX_SCAN_LIMIT=25
MIN_SCAN_GAP_MS=45000
```

`MAX_SCAN_LIMIT` ограничивает размер одного серверного скана, `MIN_SCAN_GAP_MS` задает минимальную паузу между сканами.

## Railway

Вариант A — деплой из корня репозитория:

1. Загрузи весь корень проекта в GitHub.
2. В Railway оставь Root Directory `/`.
3. Builder: `RAILPACK`.
4. Start command: `node leadrescue-48/server.js`.
5. Health check path: `/health`.

Вариант B — деплой только папки приложения:

1. В Railway выставь Root Directory `/leadrescue-48`.
2. Builder: `RAILPACK`.
3. Start command: `node server.js`.
4. Health check path: `/health`.

После этого:

1. Добавь Railway PostgreSQL.
2. Убедись, что у web-сервиса есть переменная `DATABASE_URL`.
3. При желании добавь `MAX_SCAN_LIMIT=25` и `MIN_SCAN_GAP_MS=45000`.
4. Railway запустит:

```bash
node server.js
```

Проверка:

```text
/health
```

## iPhone / PWA

Сайт можно добавить на главный экран iPhone. Но iPhone не даёт сайту стабильно работать в фоне как нативному приложению. Поэтому сканер и автопилот работают на сервере Railway, а телефон только показывает готовый статус и CRM.

## Важное правило

Сайт может искать бизнесы, проверять сайты, готовить сообщения, вести CRM, напоминать и экспортировать данные. Массовую отправку сообщений без человека не делаем: финальную отправку всегда подтверждает человек.
