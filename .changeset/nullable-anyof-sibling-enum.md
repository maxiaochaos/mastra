---
'@mastra/schema-compat': patch
---

Fixed optional union fields in OpenAI tool schemas that have an `enum` or `const` alongside a nullable union. Tools can now send `null` for those fields when they have no value, and unions that already accept `null` no longer get a duplicate `null` option.
