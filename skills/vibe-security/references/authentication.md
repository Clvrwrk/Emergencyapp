# Authentication & Authorization

Use `jwt.verify()`, never `jwt.decode()` alone. Reject `"alg": "none"`.

Next.js middleware is NOT a reliable sole auth layer. Always verify auth in Server Actions, Route Handlers, and data access functions.

Store tokens in `HttpOnly` cookies, not localStorage.
