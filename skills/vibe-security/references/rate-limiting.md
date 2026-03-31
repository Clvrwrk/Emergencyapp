# Rate Limiting

Required on: auth endpoints, AI API calls, email/SMS, file processing.

Do not store counters in public Supabase tables. Use Upstash Redis or private schema.

Set hard spending caps on AI API providers.
