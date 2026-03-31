# Database Access Control

Supabase: Enable RLS on every table. Never use `USING (true)`. Scope policies to row owner. Include `WITH CHECK` on INSERT/UPDATE. Storage buckets need their own policies.

Firebase: Never ship `allow read, write: if true`. Validate ownership. Subcollections are NOT secured by parent rules.
