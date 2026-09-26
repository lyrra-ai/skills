# 🧰 Asyniq Skills — Which one, when

32 skills total: the original 25 curated from the claude-skills repo, plus 7 added
2026-09-14 (see "Added later" below) for a solo AI-integration freelancer.
Ignore everything else in that repo — this is your whole toolkit.

**Where they live:** `~/.claude/skills/` (personal scope) — installed and confirmed on
this machine 2026-09-14 — so they load in EVERY Claude session, in any folder you open
(Asyniq subfolders AND external client repos alike). This file is just the reference
map; the skills themselves are global. (`/c/PrjMil/skills/` and `/c/PrjMil/claude-skills/`
are just the source copies used to install from — the actual live copy Claude reads is
under your home directory, `~/.claude/skills/`.)

**Companion agents + commands also installed** (`~/.claude/agents/`, `~/.claude/commands/cs/`):
`cs-backend-engineer` / `cs-fullstack-engineer` agents, and the `/cs:backend-review` /
`/cs:fullstack-review` slash commands that invoke them — these back the senior-backend
and senior-fullstack skills' deeper workflow. Their internal file paths were rewritten
from the original repo's `engineering-team/skills/...` layout to the actual installed
location (`~/.claude/skills/senior-backend/...`) so they resolve correctly.

**Known limitation:** `/cs:backend-review` and `/cs:fullstack-review`'s "fork into
specialists" step references a few skills not installed here (`observability-designer`,
`ci-cd-pipeline-builder`, `senior-security`, `adversarial-reviewer`, `performance-profiler`,
`ra-qm-team/*`) — the forcing-questions + decision-engine + profiles parts of those
commands work fully; that one step will just no-op for those specific specialists. Their
"Related commands" footer also mentions `/cs:frontend-review`, `/cs:engineer-grill`,
`/slo-design`, `/karpathy-check` — none of those are installed either. Not blocking, just
don't expect those specific cross-links to work.

In a session, just describe the task in plain English. Claude auto-picks the skill.
To force one, say e.g. *"Use the contract-and-proposal-writer skill to draft this Upwork proposal."*

---

## 🟢 WIN CLIENTS (business side)

| Skill | Use it when | Roadmap tie-in |
|-------|-------------|----------------|
| **contract-and-proposal-writer** | Every Upwork/direct proposal + before signing ANY client | Proposal System · Rule #3 |
| **cold-email** | Epic 2 M4+ cold outreach (550-emails/mo funnel) | Cold Outreach Tracker |
| **copywriting** | Upwork profile, LinkedIn headline, asyniq.com copy | Sprint 2 profile tasks |
| **landing** | Portfolio/services page on asyniq.com | Brand asset |
| **pricing-strategist** | Epic 3 — moving to value-based/fixed pricing | "First $2k+ fixed project" |
| **rfp-responder** | Direct clients that send a formal RFP | Epic 3 direct clients |
| **social-content** / **x-twitter-growth** | Epic 2 "1 post/week" content cadence | LinkedIn/X growth |

**Weekly from day one:** contract-and-proposal-writer + copywriting.

---

## 🔵 DELIVER THE WORK (your craft — AI integration)

| Skill | Use it when |
|-------|-------------|
| **saas-scaffolder** / **spec-to-repo** | Spin up the 3 portfolio projects (and client MVPs) fast |
| **zero-hallucination-coder** | Build RAG / LLM features (Portfolio Project 1) |
| **stripe-integration-expert** | Portfolio Project 3 + any billing/payments work |
| **llm-cost-optimizer** | On EVERY AI project — quote the $ savings to the client (a selling point) |
| **prompt-governance** | Before shipping prompts into a client's production app |
| **senior-fullstack** / **senior-backend** / **senior-prompt-engineer** | Architecture + code review on client builds |
| **slo-architect** / **feature-flags-architect** | Client wants reliability / safe rollout of AI features (premium work) |
| **demo-video** | After each portfolio project + each client handoff — scripts your Loom demos |
| **llm-wiki** | Build a personal KB of AI-integration patterns you reuse across clients |

---

## ⚪ WORKFLOW HELPERS (across everything)

| Skill | Use it when |
|-------|-------------|
| **grill-me** | Before locking a client scope or sprint plan — stops you under-scoping fixed-price jobs (Rule #2) |
| **handoff** | End of a work session — generates a continuity note for your next session |
| **caveman** | Long sessions — token compression, cuts your Claude/API cost 20–50% |
| **roast** | Monthly retrospective — blunt, anti-sycophancy critique of your decisions |

---

## 🆕 Added later (2026-09-14, from the wider claude-skills repo)

| Skill | Use it when |
|-------|-------------|
| **rag-architect** | Designing/reviewing RAG pipelines for client AI features — complements zero-hallucination-coder |
| **mcp-server-builder** | Building an MCP server for a client — very on-brand for an AI-integration freelancer specifically |
| **codebase-onboarding** | Inheriting a client's existing codebase — the single most common freelance-start scenario |
| **ship-gate** | Pre-launch / pre-handoff checklist before delivering any client project |
| **api-design-reviewer** | Reviewing/designing a REST API contract before building it — also backs `/cs:backend-review`'s API step |
| **database-designer** | Schema design, index strategy, normalization calls — also backs both `/cs:` review commands' schema step |
| **migration-architect** | Planning a zero-downtime data/schema/service migration for a client — also backs `/cs:backend-review`'s migration step |

---

## 📌 The typical flows

**Every proposal:** grill-me (scope) → contract-and-proposal-writer (proposal + signed agreement).

**Every client project:** grill-me (lock scope) → build with zero-hallucination-coder / senior-* → llm-cost-optimizer (quote savings) → prompt-governance (before ship) → demo-video (handoff).

**Sprint 2 right now:** saas-scaffolder → build 3 projects → demo-video for each Loom → copywriting for Upwork + LinkedIn.

**Every session:** handoff at the end · caveman when it runs long.

---

*To add a skill later: copy its folder into `~/.claude/skills/`. If the repo folder only
has a README + a `skills/` subfolder, grab the inner `skills/<name>/` (that's where SKILL.md is).*
