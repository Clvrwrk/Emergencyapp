---
name: vibe-security
description: Audits codebases for common security vulnerabilities that AI coding assistants introduce in "vibe-coded" applications. Checks for exposed API keys, broken access control (Supabase RLS, Firebase rules), missing auth validation, client-side trust issues, insecure payment flows, and more. Use this skill whenever the user asks about security, wants a code review, mentions "vibe coding", or when you're writing or reviewing code that handles authentication, payments, database access, API keys, secrets, or user data — even if they don't explicitly mention security. Also trigger when the user says things like "is this safe?", "check my code", "audit this", "review for vulnerabilities", or "can someone hack this?".
license: MIT
metadata:
  author: Chris Raroque
  version: "1.0"
---

Audit code for security vulnerabilities commonly introduced by AI code generation. These issues are prevalent in "vibe-coded" apps — projects built rapidly with AI assistance where security fundamentals get skipped.

AI assistants consistently get these patterns wrong, leading to real breaches, stolen API keys, and drained billing accounts. This skill exists to catch those mistakes before they ship.

## The Core Principle

Never trust the client. Every price, user ID, role, subscription status, feature flag, and rate limit counter must be validated or enforced server-side.

## Audit Process

1. **Secrets & Environment Variables** — See `references/secrets-and-env.md`.
2. **Database Access Control** — See `references/database-security.md`.
3. **Authentication & Authorization** — See `references/authentication.md`.
4. **Rate Limiting & Abuse Prevention** — See `references/rate-limiting.md`.
5. **Payment Security** — See `references/payments.md`.
6. **Mobile Security** — See `references/mobile.md`.
7. **AI / LLM Integration** — See `references/ai-integration.md`.
8. **Deployment Configuration** — See `references/deployment.md`.
9. **Data Access & Input Validation** — See `references/data-access.md`.

## Output Format

Organize by severity: **Critical** → **High** → **Medium** → **Low**. For each: file/line, vulnerability name, concrete impact, before/after fix.
