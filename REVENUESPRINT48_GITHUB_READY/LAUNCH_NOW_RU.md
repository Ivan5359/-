# RevenueSprint 48: запуск сегодня

## Что продаем

`$500 Quote Recovery Sprint` для локальных подрядчиков в США.

Клиент присылает 20-50 старых смет, no-response лидов или заявок. За 48 часов ты отдаешь:

- Recovery Board: Hot / Warm / Cold.
- Follow-up тексты для каждого сегмента.
- Today action list.
- 3-day и 7-day follow-up план.
- Simple tracking sheet.

Главное обещание: не гарантированный доход, а быстрый порядок в уже оплаченных/полученных лидах клиента.

## Кому писать

Лучшие первые ниши:

- roofing contractor;
- HVAC repair;
- painting contractor;
- flooring contractor;
- fencing contractor;
- remodeling contractor;
- plumbing contractor.

Лучшие города для старта: Austin, Dallas, Phoenix, Tampa, Charlotte, Nashville, Denver, Atlanta.

## Дневной план

1. Открой `index.html`.
2. Выбери город и 3-4 ниши.
3. Нажми `Full Auto`.
4. Проверь верхние лиды в `Lead Queue`.
5. Нажми `Build Today Pack`.
6. Отправь 20-40 ручных сообщений через email/contact form.
7. Все отправленные отмечай `Sent`.
8. Все ответы отмечай `Reply`.
9. Для ответов используй `Copy Close Kit`.
10. После оплаты попроси CSV по шаблону intake.

## Что нельзя автоматизировать

Не добавляй массовую автоотправку сообщений. Это риск банов, жалоб и юридических проблем.

Автоматизируем:

- поиск кандидатов;
- проверку сайтов;
- поиск контактов;
- scoring;
- сортировку очереди;
- тексты;
- follow-up due dates;
- export/backup;
- delivery pack.

Человек подтверждает:

- что бизнес релевантный;
- что контакт найден корректно;
- что сообщение не вводит в заблуждение;
- что opt-out соблюден.

## Первый close script

Great. The sprint is simple: you send 20-50 older estimates or no-response leads, I segment them into Hot/Warm/Cold, write the follow-up messages, and give you a callback board your team can use immediately.

The fixed sprint is $500. No long contract and no guarantee claim. The value is that we clean up revenue already sitting in your pipeline and give your team a clear action list in 48 hours.

If that works, I can start after payment and the CSV.

## После первого клиента

Предложи monthly upsell:

`Recovery Autopilot` за `$299-$799/month`: weekly old-lead cleanup, follow-up queue, reply tracking, and a short report.

## Локально и deploy

Статический режим:

- открой `index.html`;
- данные хранятся в браузере;
- делай `Backup JSON`.

Серверный режим:

```bash
npm install
npm start
```

Railway:

- подключи GitHub repo;
- добавь PostgreSQL;
- проверь `DATABASE_URL`;
- опционально задай `MAX_SCAN_LIMIT=25` и `MIN_SCAN_GAP_MS=45000`.
