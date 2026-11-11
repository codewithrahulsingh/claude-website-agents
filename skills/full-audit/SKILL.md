---
name: full-audit
description: Audits an existing website for QA, accessibility, performance, security and technical SEO. Use when the user says "audit this site", "site check karo", "full audit" or runs /full-audit.
argument-hint: <site url>
---

Run an audit on the existing site: $ARGUMENTS
Audit only sites the user owns or is authorized to work on. Do not change the live site.

Run in parallel: qa-tester, accessibility-checker, performance-optimizer, security-auditor, technical-seo.
Then combine into `docs/audit-summary.md`: top 10 issues by severity with fix and owner agent.
Show only the progress bar + issue counts in chat.
