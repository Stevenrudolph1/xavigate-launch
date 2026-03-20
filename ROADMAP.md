# Xavigate Launch Roadmap

Last updated: 2026-03-03
Location: `~/Projects/planning/xavigate-launch/ROADMAP.md`
Say: **"open the launch roadmap"** or **"xavigate roadmap"**

---

## List 1.0 — Launch Readiness ✅
Complete. All 10 items done (commit 6cf1bc0, 2026-03-03).
Board: M1 `~/.openclaw/workspace/docs/audits/LIST-1.0-EXECUTION-BOARD.md`

## List 2.0 — Checkout + Analytics ✅
Complete. All 5 items done (2026-03-03).

| ID | Task | Status |
|----|------|--------|
| L2-01 | Stripe products for 4 map tiers | ✅ Done — 4 products + prices in Stripe + D1 |
| L2-02 | End-to-end checkout test | ✅ Done — all tiers work (test + live) |
| L2-03 | Analytics (pageviews, CTA clicks, checkout) | ✅ Done — cookie-free, `analytics_events` in D1 |
| L2-04 | Mobile QA | ✅ Done — responsive CSS verified |
| L2-05 | CORS fix | ✅ Done — already correct (5 origins) |

**Commits:** `xavigate-site` @ 846d817, `renergence-shop-worker` @ 09c81e0

---

## List 3.0 — Trust + Conversion (Post-Launch Optimization)

| ID | Task | Priority | Status |
|----|------|----------|--------|
| L3-01 | First real Map case study (anonymized, with permission) | P1 | Blocked — needs real client |
| L3-02 | Testimonial collection system (post-delivery email) | P1 | Not started |
| L3-03 | Email capture for non-buyers (sample map gate or newsletter) | P1 | Not started |
| L3-04 | Behavioral triggers (reading 2+ books → Map CTA) | P2 | Not started |
| L3-05 | Individual research reference pages (31 entries) | P2 | Not started |

## List 4.0 — Scale Infrastructure

| ID | Task | Priority | Status |
|----|------|----------|--------|
| L4-01 | Automated intake → map generation pipeline | P1 | Not started |
| L4-02 | Client portal (map delivery, follow-up ordering) | P2 | Not started |
| L4-03 | Practitioner dashboard (for guided intake tier) | P2 | Not started |

## Beyond Lists — Growth

- Marketing launch (Substack, email list, soft announce)
- Practitioner pipeline (first certified practitioners)
- Pricing validation (conversion data → tier adjustments)
- Content engine (Substack → site articles → SEO flywheel)
- Second product surface (training via OpenClaw/Beacon)

---

## Status Rhythm

| Cadence | Check |
|---------|-------|
| Weekly (Monday) | Conversion data, support emails, update board |
| Biweekly (1st/15th) | Review analytics, identify top friction, ship 1 fix |
| Monthly | Full site QA, add 2-3 research entries, request testimonials |
| Per-Sale | Shriya sends MNTEST+intake within 24hrs, post-delivery testimonial request |

---

## Key Files

| What | Where |
|------|-------|
| Site repo | `~/Projects/xavigate-site/` (push main = deploy) |
| Shop worker | `~/Projects/renergence-shop-worker/` |
| Stripe keys | `~/Projects/archive/xavilms/xavi-lms/.env` |
| Analytics data | D1 `analytics_events` table |
| Execution board (L1) | M1 `~/.openclaw/workspace/docs/audits/LIST-1.0-EXECUTION-BOARD.md` |
| This roadmap | `~/Projects/planning/xavigate-launch/ROADMAP.md` |

---

## Handoff Prompt

Paste into a new Claude Code session to resume:

> **Context:** Xavigate.com is at soft launch readiness. Lists 1.0 (site build) and 2.0 (checkout + analytics) are complete. 4 map tiers ($397/$697/$1,097/$197) have live Stripe checkout. Cookie-free analytics tracking pageviews and CTA clicks. All core pages cross-linked.
>
> **Roadmap:** `~/Projects/planning/xavigate-launch/ROADMAP.md`
>
> **Next:** List 3.0 — Trust + Conversion. Start with L3-02 (testimonial collection) or L3-03 (email capture), whichever Steven prioritizes.
>
> **Key files:** Site: `~/Projects/xavigate-site/`, Shop worker: `~/Projects/renergence-shop-worker/`, Stripe keys: `~/Projects/archive/xavilms/xavi-lms/.env`
