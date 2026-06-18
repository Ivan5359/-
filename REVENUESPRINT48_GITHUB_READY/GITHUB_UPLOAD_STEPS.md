# GitHub upload steps

Upload this folder as the repository root:

```text
C:\Users\repki\Documents\1k\REVENUESPRINT48_GITHUB_READY
```

Railway settings:

- Builder: `RAILPACK`
- Root Directory: `/`
- Start Command: `node server.js`
- Healthcheck Path: `/health`

Postgres:

Add this variable to the Railway app service, not the Postgres service:

```text
DATABASE_URL=${{Postgres.DATABASE_URL}}
```

After redeploy, check:

```text
https://YOUR-RAILWAY-URL/health
```

Expected:

```json
"storage": "postgres"
```
