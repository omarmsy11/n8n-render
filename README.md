# n8n-render

Successfull installation of n8n on Render using Docker.

To make it run just open Render Dashboard and use this git as Blueprint.

Important note if using disk on Render: Keep the mountPath as is, otherwise n8n won't change the data.

The .env.example file contains examples of lines that can be added manually on Environment Variables on Render after install. Never commit real values: secrets (N8N_ENCRYPTION_KEY, DB_POSTGRESDB_PASSWORD) go only in the Render Dashboard (service > Environment). For local use, copy .env.example to .env (ignored by git) and fill it in.

N8N_ENCRYPTION_KEY is asked for when the Blueprint is created. Keep a copy of it: changing it later makes the credentials already stored in n8n unreadable.

To change the webhook URL from localhost to your domain, for example, just add the var WEBHOOK_URL followed by the full URL.

Version 0.224.1
