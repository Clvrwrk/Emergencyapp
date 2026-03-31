# Deployment Security

Disable debug mode and source maps in production. Verify `.git` is not publicly accessible.

Never use production keys in preview deployments. Set security headers (CSP, HSTS, X-Frame-Options).

Never use `Access-Control-Allow-Origin: *` on authenticated endpoints.
