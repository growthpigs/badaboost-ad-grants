# Badaboost Ad Grants

**Repo:** `growthpigs/badaboost-ad-grants`
**Created:** 2026-04-03

## What This Is

AI-powered Google Ad Grant management service for nonprofits. We obtain and manage $10K/month Google Ad Grant accounts using programmatic AI, Google Ads API, and automated content marketing — achieving what previously required a full team.

**The business:** Badaboost Ad Grants (BNAG) has 5+ years of history (2020-2025) with proven methodology, existing NPO registrations in France, and a working engine (Google Ads Funnelizer). We're relaunching with modern AI tooling to scale.

**The model:** Help nonprofits advance their mission via the Google Ad Grant. For-profits create "Parallel-Hybrid" nonprofit arms in France to access $10K/month in free Google search ads.

## Related Repos

| Repo | Purpose | Relationship |
|------|---------|-------------|
| `growthpigs/google-ads-funnelizer` | The engine — code, APIs, scripts, content pipeline | Tools that execute the work |
| `growthpigs/ad-grant-clients` | Client work — per-client campaigns, content, analytics | Where client deliverables live |
| This repo | The service — methodology, SOPs, templates, knowledge | How we do things |

**Local paths:**
- Engine: `badaboost/internal-projects/google-ads-funnelizer/`
- Clients: `badaboost/internal-projects/ad-grant-clients/`
- This: `badaboost/internal-projects/badaboost-ad-grants/`
- Business: `badaboost/internal-projects/badaboost-llc/`

## The Service

### Google Ad Grant Basics

| Fact | Value |
|------|-------|
| Monthly grant | $10,000 USD in Google Search Ads credits |
| Annual value | $120,000 USD |
| Daily budget | $329 USD |
| CTR requirement | >5% account-wide |
| Max CPC (manual) | $2.00 (bypassed with maximize conversions bid) |
| Quality Score | 3+ on all keywords |
| Content freshness | Update every 90 days |
| Conversions | 1+ meaningful per month |

### The 11-Step Grant Pipeline

```
1. Onboarding → 2. Name & Domain → 3. NPO Registration (France)
→ 4. Asset Creation (brand, site, content) → 5. Nonprofit Approval
→ 6. Techsoup Token → 7. G4NP Approval → 8. Workspace Setup
→ 9. Ad Grant Submission → 10. Ad Grant Account → 11. Client Handover
```

Timeline: 4-6 weeks from onboarding to live grant.

### Pricing (2026 — Updated for AI-First Model)

**New client pricing (ISKCON pilot onwards):**
- $500/month management fee (target nonprofit budget)
- Focus on getting results first, then referrals
- Referral discount structure TBD

**Historical pricing (full-service, 2022-2023):**
- $16K total ($6K deposit + $10K on delivery)
- Or $4K/month × 5 months
- 15% of ad spend monthly retainer (~$1,500/month)
- $34,050 total value in deliverables

### The Parallel-Hybrid Structure

For-profit businesses create a nonprofit arm registered in France:
- France registration = fast (~10 days), minimal admin
- No EIN/501c needed — French NPOs are "social/cultural" organizations
- No accounting required if non-earning
- Can advertise globally from France
- Client owns the NPO and all assets

### Three Pillars (Project Waterfall)

| Pillar | Purpose | Tools |
|--------|---------|-------|
| **SEO** | Long-term authority (5yr view) | DataForSEO, Google Trends |
| **Google Ads** | Short-term traffic ($10K/mo) | Google Ads API |
| **Content Marketing** | Blog via CIA → Waterfall → BuildFast | Notion, BuildFast |

### Key Capability: 85-95% Spend Rate

Most self-managed grants spend $500-$1,000 of $10K. We consistently achieve 85-95% spend with targeted conversions within 10 days of receiving the grant.

## Existing Grant Accounts (from Notion)

| Account | Domain | Status | Notes |
|---------|--------|--------|-------|
| **Retirementality** | retirementality.net | Active — $8K spend | Personal grant, needs funnel completion |
| **Badaboost Ad Grants** | badaboostadgrants.org | BASF Ads Running | Igor managing |
| **Grounding Hope** | groundinghope.org | Waiting | Full client knowledge base exists |
| **Break Patterns** | breakpatterns.org | BASF Ads Running | Straight Forward ads mgmt |
| **Wishborn** | wishborn.org | No ads running | V2 conversion testing done |
| **Social Media Thrive** | — | No ads running | Waiting |
| **Find Krishna** | findkrishna.org | Waiting | IONOS registered, G4NP OK — ISKCON related |
| **World Master Class** | — | Ready | Intake form done |
| **Ultimate Closer** | — | Waiting | Strategy call material |
| **Kulturbackstube** | — | Requires Domain | Needs everything |

**Revival priority:** Grounding Hope, Break Patterns, Wishborn (already have assets). Find Krishna connects to ISKCON pilot.

## Notion Knowledge Base

The BNAG Notion Team-space contains extensive documentation from 2022-2023:

| Resource | Notion ID | Content |
|----------|-----------|---------|
| BNAG Team-space | `8d08bd0d` | Main hub — pipeline, SOPs, databases |
| HOME BASE | `a58cdc9d` | Operations — process DBs, campaign DBs, client SOPs |
| The Offer | `79b3286b` | Full $34K offer stack with deliverables |
| Deliverables | `fbfd283c` | Detailed deliverable descriptions |
| Grant Process | `c7d65832` | 11-step pipeline with full descriptions |
| Onboarding Emails | `2ac1500c` | Client email sequence |
| FAQ | `02cc6074` | 14+ compliance and sales Q&A |
| Sales Campaigns | `db63b84a` | Outbound sales SOPs |
| Find Krishna | `13a5e860` | ISKCON-related account (findkrishna.org) |
| Ad Grants Accounts DB | `collection://5caff6d1` | All grant accounts |
| Ad Campaigns DB | `collection://6b911a96` | Per-client campaigns |
| NPO-AG DB | `collection://86cb85b3` | NPO registration tracking |

## Team

| Person | Role |
|--------|------|
| **Roderic Andrews** | Strategy, systems, AI tooling, client relations |
| **Jonathan (Jono) Andrews** | Account management, client operations, content |

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Ads Engine | Google Ads API (OAuth2) via google-ads-funnelizer |
| Content Pipeline | `content-pipeline.py` → Notion → BuildFast |
| Blog | BuildFast (syncs from Notion) |
| Lead Capture | Quiz app (Vercel) → GHL (GoHighLevel) |
| Analytics | GA4 + GTM + Microsoft Clarity |
| SEO | DataForSEO + Google Trends |
| CRM | GoHighLevel (Harvest Demand) |
| NPO Registration | Simplitoo (French admin partner) |
| Hosting | Webflow (client sites), Siteground (domains) |
| MCC | Badaboost Ad Grants (924-843-0199) |

## Project Structure

```
badaboost-ad-grants/
├── CLAUDE.md              ← This file (project identity for AI)
├── HANDOVER.md            ← Live working context (updated during work)
├── features/              ← Living component docs
│   ├── GRANT-PIPELINE.md  ← The 11-step process
│   ├── PRICING.md         ← Current pricing models
│   └── COMPLIANCE.md      ← Ad Grant rules and policies
├── docs/05-planning/      ← Plans (Claude Code reads this)
├── knowledge/             ← Extracted Notion knowledge
│   └── notion-archive/    ← Exported Notion content
└── .foundry/              ← Pipeline runtime artifacts
```

## Conventions

- **Naming:** kebab-case files, UPPERCASE.md for feature docs
- **Git:** Conventional commits. Branch naming: feature/X, fix/X
- **Notion IDs:** Always store as 8-char shorthand (first 8 of UUID) in references
- **Client work:** Goes in `growthpigs/ad-grant-clients`, NOT here

## Key Decisions

| Decision | Why | Date |
|----------|-----|------|
| NPOs registered in France | Fastest registration (~10 days), minimal admin, no EIN needed | 2022 |
| Separate client repo | Client data grows fast, keeps methodology repo clean | 2026-04-03 |
| GAF as shared engine | Reusable across all accounts, not per-client | 2024 |
| $500/mo pilot pricing | Matches nonprofit budgets, prove value then grow via referrals | 2026-04-03 |
| AI-first relaunch | Programmatic AI + APIs replace team of people | 2026-04-03 |

## GitHub Is the Source of Truth

All project management lives in GitHub:

| What | Where |
|------|-------|
| Admin Documents (18) | GitHub issues in `Admin Documents` milestone |
| Activity Log | Pinned issue — updated every session |
| Work Ledger | Pinned issue — DU tracking |
| Phase Master Index | Pinned issue — roadmap and priorities |
| Feature specs | GitHub issues with `spec` label |
| Bug reports | GitHub issues with `bug` label |

**Quick access:**
```bash
gh issue list --repo growthpigs/badaboost-ad-grants
gh issue list --repo growthpigs/badaboost-ad-grants --milestone "Admin Documents"
gh issue list --repo growthpigs/badaboost-ad-grants --label "epic"
```

## Working with This Project

### Starting a Session
1. Read this file (you're doing it now)
2. Read `HANDOVER.md` for current context
3. Check `gh issue list` for active work
4. Check `features/` for component knowledge

### During Work
- **HANDOVER.md** — update continuously (not at session end)
- **features/*.md** — update when a component changes
- **GitHub issues** — comment with progress, close when done

### Features Documentation

`features/` contains living docs — one file per component/domain:

```
features/
├── GRANT-PIPELINE.md    ← The 11-step acquisition process
├── PRICING.md           ← Pricing models and tiers
├── COMPLIANCE.md        ← Google Ad Grant rules
├── CONTENT-STRATEGY.md  ← Waterfall, clusters, SEO
└── ONBOARDING.md        ← Client onboarding flow
```

## Methodology

This project follows **The Software Foundry** — a spec-first pipeline:

```
MINE → SCOUT → ASSAY → CRUCIBLE → PLAN → HAMMER → TEMPER → AUTORESEARCH → RALPH LOOP
```

- Methodology docs: `growthpigs/the-foundry`
- Current phase: MINE — gathering knowledge, establishing structure
- Pipeline runner: `~/_PAI/operations/the-foundry/bin/foundry.sh`

## What NOT to Do

- **Don't create random .md files.** Use `features/` for component docs.
- **Don't duplicate GitHub issues locally.** GitHub is the source of truth.
- **Don't skip Ratify gates.** Every phase transition gets reviewed.
- **Don't merge without runtime testing.** Tests pass ≠ feature works.
- **Don't commit secrets.** No `.env`, no API keys, no credentials in git.
- **Don't put client work here.** Client deliverables go in `growthpigs/ad-grant-clients`.

## Reply Footer (MANDATORY — Every Task Completion)

Every reply at task completion MUST end with a `---` separator followed by this 7-line status footer:

```
---
🔧 CC Engaged: https://github.com/growthpigs/badaboost-ad-grants/issues/NNN | Status: XX% complete
📋 CC Queue: [queued items waiting their turn]
💭 Open Loops: [firehose ideas not yet queued as tasks]
📅 Coming: [planned items, upcoming sprints]
🔌 MCPs: Chi-GW [✅/❌] | Chrome [✅/❌] | Agent Browser [✅/❌]
✅ X/Y complete | XX% confident ([context note])
📊 DD.MM HH:MM | ~Xk tokens | ~$X.XX
```

**Rules:**
- `---` separator ALWAYS precedes the footer
- CC Engaged MUST have a full clickable GitHub issue URL — never bare `#123`
- Get time with: `date "+%d.%m %H:%M"`
- Pricing: opus=$15/1M, sonnet=$3/1M, flash=$0.60/1M

*Last Updated: 2026-04-03*
