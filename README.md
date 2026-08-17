<h1 align="center">Mohaned Mohamed Fozy</h1>

<p align="center">
  <b>Python Automation Developer · AI Integration</b><br>
  Cairo, Egypt · Open to remote roles and freelance projects
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9%2B-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python 3.9+">
  <img src="https://img.shields.io/badge/Focus-Workflow%20Automation-0A7E8C?style=flat-square" alt="Workflow Automation">
  <img src="https://img.shields.io/badge/Focus-AI%20Integration-6E4AFF?style=flat-square" alt="AI Integration">
  <img src="https://img.shields.io/badge/Tests-393%20passing-3FB950?style=flat-square" alt="393 tests passing">
</p>

---

I build the boring half of a business into software: the report someone assembles by
hand every month, the inbox someone sorts every morning, the stock sheet nobody
checks until a customer complains. I write it in Python, put it on a real trigger so
it runs without anyone remembering to run it, and add an AI step only where a rule
cannot make the judgement.

Everything below runs on a laptop with no GPU and no paid API key by default. Each
repository ships sample data and a one-command demo, so you can see it work before
reading a line of code.

---

## Selected work

| Project | What it removes | Built with |
|---|---|---|
| **[order-ops-pipeline](https://github.com/Mohaned-Fozy-Ai/order-ops-pipeline)** — *capstone* | A store owner's whole morning: checking new orders, spotting the bad ones, updating the sheet, messaging customers | Ingest → validate → AI enrich → persist → notify → report, on a schedule. SQLite system of record, webhook receiver with HMAC verification, circuit breaker, resumable runs |
| **[ai-inbox-triage](https://github.com/Mohaned-Fozy-Ai/ai-inbox-triage)** | Reading an unsorted support inbox to find out which message matters | Classifies, scores urgency, extracts order numbers, drafts replies — Arabic and English. Deterministic backend by default, LLM optional, with an accuracy harness |
| **[stock-watch-automation](https://github.com/Mohaned-Fozy-Ai/stock-watch-automation)** | Nobody noticing a product went out of stock until sales stop | Unattended monitor with state in SQLite, change detection between runs, alert cooldown, Slack/email channels, GitHub Actions cron |
| **[sales-report-automator](https://github.com/Mohaned-Fozy-Ai/sales-report-automator)** | The monthly spreadsheet ritual | Tolerant CSV ingest, a quality gate that quarantines bad rows instead of crashing, and a report in CSV, Markdown and HTML |
| **[smart-file-organizer](https://github.com/Mohaned-Fozy-Ai/smart-file-organizer)** | Filing a folder of hundreds of attachments by hand | Rule-based sorting, SHA-256 duplicate detection, dry-run by default, and an undo journal for every applied run |

---

## How I work

- **Dry-run first.** Anything that moves, deletes or sends starts in preview mode. Destructive actions are opt-in.
- **A system, not a script.** State between runs, de-duplicated alerts, retries with backoff, a non-zero exit code when something is actually wrong.
- **AI where it earns its place.** A deterministic fallback is always the default path, so the system still works when a model is down, slow or wrong. Low-confidence output is routed to a human instead of guessed.
- **Tested and measured.** 393 tests across these five repositories. Every number in a README comes from a real run, and any business estimate names the assumption behind it.

---

## Stack

**Language** Python (standard library first: `sqlite3`, `csv`, `urllib`, `hmac`, `email`, `decimal`, `logging`, `argparse`, `dataclasses`)
**Automation** GitHub Actions cron · systemd timers · cron · webhook receivers with signature verification
**Integrations** REST APIs · Google Sheets API · Slack webhooks · SMTP · OpenAI-compatible chat endpoints
**AI** Prompt-to-strict-JSON with schema validation and repair retry · confidence gating · human-in-the-loop routing · Arabic text normalisation
**Reliability** Retries with exponential backoff and jitter · circuit breakers · idempotency keys · structured JSON logging · resumable runs
**Data** SQLite (WAL, migrations) · `Decimal` money handling · tolerant CSV parsing · data quality gates

---

## Certifications

<!-- FILL: add each certificate as you earn it, with its public verification link.
     Planned, in order: HackerRank Python (Basic) · Kaggle Python · Kaggle Pandas ·
     Cisco NetAcad Python Essentials 1 · Cisco Introduction to Modern AI ·
     Hugging Face AI Agents · IBM SkillsBuild Python. -->

---

## Contact

Cairo, Egypt (UTC+3) · Arabic (native) · English (conversational)

<!-- FILL: LinkedIn URL -->
<!-- FILL: email address -->

<p align="center"><sub>Available for remote and freelance work in Python automation and AI integration.</sub></p>

<!-- Profile README for github.com/Mohaned-Fozy-Ai -->
