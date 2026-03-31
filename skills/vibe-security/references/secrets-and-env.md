# Secrets & Environment Variables

Never hardcode API keys, tokens, passwords, or credentials in source code. If a secret was ever committed to Git history, consider it compromised — rotate it immediately.

Client-side prefixes (bundle = public): `NEXT_PUBLIC_`, `VITE_`, `EXPO_PUBLIC_`, `REACT_APP_`.

Never client-side: `service_role` key, Stripe secret key, DB connection strings, JWT secrets.

Ensure `.env` files are in `.gitignore`.
