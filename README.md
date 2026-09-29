# Darkly

Web security project from the 42 cursus. Darkly is a deliberately vulnerable web
application; the goal is to find, exploit, and — most importantly — explain and
remediate a set of common web vulnerabilities, capturing a flag for each one.

This repository documents **14 vulnerabilities**, each in its own folder with a
short write-up (the flaw, how it was exploited, its impact, and how to prevent it)
plus the captured flag and any tooling used.

## Vulnerabilities covered

| # | Category |
|---|----------|
| 1 | Stored XSS (comment form) |
| 2 | Weak authentication |
| 3 | SQL injection (member search) |
| 4 | Hidden form fields |
| 5 | Cookie manipulation |
| 6 | SQL injection (image search) |
| 7 | Directory enumeration |
| 8 | Brute-force login |
| 9 | Open redirect |
| 10 | Form value manipulation |
| 11 | File upload / MIME bypass |
| 12 | Path traversal |
| 13 | XSS via `data:` URI |
| 14 | HTTP header spoofing |

Each folder's `Resources/README.md` explains the vulnerability and, where relevant,
includes the scripts used (e.g. a directory-enumeration helper, a brute-force
script). Every write-up ends with concrete **prevention** guidance — the point of
the project is defensive understanding, not just capturing flags.

## Note

Group project, done together with a teammate (**mikferna**).

## Topics

`web-security` · `owasp` · `xss` · `sql-injection` · `path-traversal` · `42`
