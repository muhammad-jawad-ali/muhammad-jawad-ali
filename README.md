# Muhammad Jawad Ali

Full-stack and applied AI engineer. I ship product features end to end: React and Next.js on the front, FastAPI and Postgres on the back, Docker and CI in between, and LLMs where they actually help.

- **Now:** Junior Full-Stack Developer at Zigron, building **Heliorix**, a GIS SaaS platform (part-time).
- **Also:** Final-year BS Computer Science at FAST-NUCES Islamabad.
- **Looking for:** remote Junior Full-Stack or Applied AI Engineering roles with US/EU teams. I work your hours, with at least 4 hours of overlap with US Eastern.

**Portfolio:** [mjawadali.com](https://mjawadali.com) · **LinkedIn:** [in/muhammad-jawad-ali](https://www.linkedin.com/in/muhammad-jawad-ali/) <!-- · **Email:** add a professional address here -->

---

## Selected work

### [Scaffold](https://github.com/muhammad-jawad-ali/Scaffold): an adaptive AI tutor that does not hand out answers
A tutor for C++ programming labs. A policy decides how much help a student gets, and a guardrail keeps the reference solution from leaking through the model.
- Bayesian Knowledge Tracing that discounts passes that look pasted or hint-driven. Benchmarked against an LSTM (DKT) on 4,000 held-out students.
- Locally hosted `qwen2.5-coder:7b` through Ollama. No student code leaves the machine.
- Prompt-injection screening, plus a leakage guardrail that compares token overlap and the C++ syntax tree against the reference.
- Student code runs in locked-down Docker containers: no network, read-only filesystem, all capabilities dropped, memory and PID limits.
- CI runs about 950 Python tests, the web tests, the sandbox tests and a Docker smoke test on every PR. Tagged releases publish images to GHCR.

`React` `TypeScript` `FastAPI` `PostgreSQL` `Docker` `GitHub Actions` `Ollama`

### [NayaGhar](https://github.com/muhammad-jawad-ali/NayaGhar): a demand-first real estate marketplace · [live](https://naya-ghar-delta.vercel.app)
Buyers post what they want, and verified agents compete to pitch matching properties. Three roles (buyer, agent and admin) with route-level access control, a negotiation room, notifications and an admin console.

`Next.js 16` `React 19` `MongoDB` `NextAuth` `Zod` `Vercel`

### Systems and performance
- **[KLT Feature Tracker on GPUs](https://github.com/muhammad-jawad-ali/KLT-Feature-Tracker-Acceleration-on-GPUs):** ported the KLT feature tracker to CUDA and profiled the speedup.
- **N-body simulation:** parallelised with MPI and OpenMP. <!-- TODO: link the repo once it is public -->
- **JSON to XML translator:** a compiler front end in C++ with Flex and Bison. <!-- TODO: link the repo once it is public -->

---

## Stack

| Area | Tools |
|---|---|
| Frontend | React, Next.js (App Router), TypeScript, Tailwind CSS |
| Backend | FastAPI, Python, Node.js, REST |
| Data | PostgreSQL, MongoDB, SQLAlchemy, Alembic |
| Infra | Docker, Docker Compose, GitHub Actions, Vercel, GHCR |
| AI | Local LLMs (Ollama, Qwen), prompt-injection defence, n8n agent workflows, PyTorch |
| Systems | C++, CUDA, MPI, OpenMP |

## How I work

- **Readable over clever.** Plain names, explicit control flow, code a new teammate can follow on day one.
- **Small changes, merged often.** Trunk-based development, short-lived branches, squash or rebase before merge.
- **Tests and CI first.** If CI doesn't check it, I don't assume it works.
- **Product first.** I start from the user problem, then pick the stack.
