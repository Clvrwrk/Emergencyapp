# AI / LLM Integration Security

AI API keys must never appear in client-side code. All AI calls go through your backend.

Set hard spending caps. Implement per-user limits.

Separate user input from system prompts. Sanitize LLM output before rendering as HTML.
