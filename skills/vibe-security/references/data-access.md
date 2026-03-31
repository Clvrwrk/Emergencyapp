# Data Access & Input Validation

Use parameterized queries. Never concatenate user input into SQL.

Validate all input with Zod or similar at system boundaries. TypeScript types provide zero runtime protection.

Don't spread request bodies into DB operations (mass assignment).
