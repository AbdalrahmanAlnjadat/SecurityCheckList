# 🔐 Web Security Checklist — Pre-Deployment Audit Tool

A free, interactive security checklist for web developers. **210+ checks across 21 categories** — covering everything from SQL injection to hardcoded secrets to session cookie flags. Built as a single HTML file; no install required.

> **Bonus:** Includes a built-in AI prompt you can copy and paste into Claude, ChatGPT, or Gemini to have it audit your entire codebase automatically before you ship.

---

## 🚀 How to Use

1. Download `security-checklist.html`
2. Double-click it — it opens in your browser
3. Go through each category and check off items as you verify them
4. When you're ready for a deeper audit, click **"Copy AI Prompt"** and paste it into any AI model along with your code

That's it. No npm, no setup, no account needed.

---

## 🤖 The AI Audit Feature

The built-in prompt turns any AI into a security auditor for your project. Here's how:

1. Click the **"⎘ Copy AI Prompt"** button in the tool
2. Open Claude / ChatGPT / Gemini
3. Paste the prompt, then paste your code (or describe your stack)
4. The AI will go through every single check and return:
   - ✅ **PASS** — verified safe
   - ❌ **FAIL** — with the vulnerable code, the attack scenario, and exact fix
   - ➖ **N/A** — not applicable to your stack
5. At the end it gives a **READY / NOT READY** deployment verdict

This works best when you paste actual code files alongside the prompt so the AI can check them directly.

---

## ✅ What's Covered (21 Categories)

| # | Category | Checks |
|---|----------|--------|
| 1 | 💉 Injection Attacks | SQL, NoSQL, LDAP, Command, XPath, SSTI |
| 2 | 🕷️ Cross-Site Scripting (XSS) | Reflected, Stored, DOM, CSP |
| 3 | 🔐 Authentication | Password hashing, brute-force, MFA, JWT |
| 4 | 🍪 Sessions & Cookies | HttpOnly, Secure, SameSite, timeout, regeneration |
| 5 | 🛡️ Authorization & Access Control | Role enforcement, privilege escalation |
| 6 | 🔁 CSRF | Token validation, SameSite, Origin checks |
| 7 | 🔓 IDOR & Broken Object Level Auth | Object ownership, UUID vs sequential IDs |
| 8 | 📋 HTTP Security Headers | HSTS, CSP, X-Frame-Options, nosniff |
| 9 | 📥 Input Validation & File Uploads | MIME types, magic bytes, path traversal in filenames |
| 10 | 🕵️ Information Disclosure | Stack traces, .env exposure, debug mode, source maps |
| 11 | 🔑 Hardcoded Secrets & Config | API keys in code, .env in git, secrets in bundles |
| 12 | 🔒 TLS / HTTPS | Certificate validity, TLS version, cipher suites |
| 13 | ⏱️ Rate Limiting & DoS | Login, registration, file upload, ReDoS |
| 14 | 📦 Third-Party & Dependencies | CVE audit, SRI hashes, pinned versions |
| 15 | 📊 Logging & Monitoring | Auth events, 403s, admin actions, alerting |
| 16 | 🌐 CORS & API Security | Origin allowlist, credentials header, GraphQL limits |
| 17 | ↩️ SSRF & Redirects | Webhook validation, open redirects, internal IP blocking |
| 18 | 📁 Path Traversal & File Access | Directory escape, realpath validation |
| 19 | 👑 Admin Role Hardening | MFA, IP restriction, re-auth on destructive actions |
| 20 | ⚡ Performance & Availability | Indexes, N+1 queries, pagination, caching |
| 21 | 🚀 Environment & Deployment | Dev vs prod config, open ports, backup testing |

---

## 📸 Screenshots

> Open `security-checklist.html` in your browser — dark terminal-style UI, progress tracking per category, and a one-click AI prompt copy button.

---

## 🗂️ Files

```
/
├── security-checklist.html   ← The entire tool, single file
└── README.md
```

---

## 💡 Who This Is For

- Developers about to deploy a web app for the first time
- Freelancers doing a final check before handing off a project
- Teams that want a repeatable pre-launch security process
- Anyone building a site with user accounts, roles, sessions, or file uploads

---

## 🤝 Contributing

Found a check that's missing? Open an issue or pull request. Security is a moving target and the list should grow.

---

## 📄 License

MIT — free to use, share, and modify.
