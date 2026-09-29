This project was built as part of the 42 cursus by hcarrasc42 and mikferna.

# Darkly

> _You can't defend what you don't understand — so first, break it._

A web-security project from the 42 cursus. **Darkly** is a deliberately
vulnerable web application; the goal is to find, exploit, and — most importantly
— **explain and remediate** a set of common web vulnerabilities, capturing a flag
for each one. This repository documents **14 vulnerabilities**, each with a
concise write-up and prevention guidance.

![Field](https://img.shields.io/badge/field-web%20security-red?style=flat-square)
![Reference](https://img.shields.io/badge/reference-OWASP-informational?style=flat-square)
![School](https://img.shields.io/badge/42-cursus-black?style=flat-square)

## 📖 About

Darkly is a defensive-security exercise disguised as a capture-the-flag: the
point is not just to grab flags, but to understand **why** each flaw exists and
**how** to prevent it. Each vulnerability lives in its own folder with a short
`Resources/README.md` describing the weakness, how it was reached, its impact,
and the fix — and, where relevant, the small helper scripts used along the way.

## 🎯 Vulnerabilities covered

| # | Category | Class |
|---|----------|-------|
| 1 | Stored XSS (comment form) | Injection |
| 2 | Weak authentication | Broken auth |
| 3 | SQL injection (member search) | Injection |
| 4 | Hidden form fields | Broken access control |
| 5 | Cookie manipulation | Broken auth |
| 6 | SQL injection (image search) | Injection |
| 7 | Directory enumeration | Security misconfiguration |
| 8 | Brute-force login | Broken auth |
| 9 | Open redirect | Broken access control |
| 10 | Form value manipulation | Broken access control |
| 11 | File upload / MIME bypass | Insecure upload |
| 12 | Path traversal | Broken access control |
| 13 | XSS via `data:` URI | Injection |
| 14 | HTTP header spoofing | Broken access control |

## 💡 What This Project Demonstrates

- **Recognizing common web vulnerability classes** — injection, broken
  authentication and access control, misconfiguration, and insecure uploads —
  mapped to the kinds of issues the OWASP Top Ten describes.
- **A defensive mindset:** every write-up ends with concrete **prevention**
  (parameterized queries, input validation, least privilege, correct upload and
  redirect handling), because the purpose is to build software that resists these
  attacks.
- **Methodical documentation:** each finding is reproduced, explained, and fixed
  — the habit of turning an exploit into an actionable lesson.

## 📂 Project Structure

```
darkly/
├── 1-XSS_Comment_Form/           Resources/README.md · flag
├── 2-Weak_Authentication/        …
├── 3-SQL_Injection_Members/      …
│   … (one folder per vulnerability, 1–14)
└── 14-Header_Spoofing/           Resources/README.md · flag
```

Each folder's `Resources/README.md` explains the vulnerability and its remediation.

## Note

Group project, done together with a teammate (**mikferna**).
