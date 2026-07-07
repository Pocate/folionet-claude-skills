# folionet-data
**Version:** v0 — skeleton built from 06-kpis-measurement. Not yet fed real numbers — needs Metricool connected + the platform CSV before it can do more than tell you what to look for. Update the moment either lands.

## What this skill does
Load this every Monday before the content research session. Paste the week's Metricool export (or the 5-number weekly dashboard, manually tracked) and it tells you what worked, what didn't, and what to prioritize next week — using the benchmarks already defined in the KPI framework, not guesswork.

**Input:** Metricool weekly export, or the 5 manually-tracked numbers below if Metricool isn't connected yet.
**Output:** A short read — 3 things, max — on what moved, what to double down on, what to fix.

---

## THE NORTH STAR
**First operations per month** — activated clients who complete their first investment. Everything else is a leading indicator toward this one number. If a channel or post drives lots of engagement but no discovery calls, it's not working yet — regardless of how it looks.

---

## THE 5-NUMBER WEEKLY DASHBOARD (minimum viable tracking — use even without Metricool)
1. New LinkedIn followers (this week vs. last week)
2. New email subscribers (this week vs. last week)
3. Email open rate (last email sent)
4. Discovery calls booked (this week)
5. First operations (this month to date)

If Metricool isn't connected yet, track these 5 by hand every Monday — 10 minutes, no tool required.

---

## THE 6-STAGE FUNNEL — WHAT "GOOD" LOOKS LIKE

| Stage | Key metric | Benchmark (Month 1-3) |
|---|---|---|
| 1. Awareness | LinkedIn follower growth | +50-100/week |
| 1. Awareness | Post engagement rate | 3-5% |
| 2. Capture | Newsletter signups/week | 20-50/week from LinkedIn |
| 3. Consideration | Email open rate | 35-45% |
| 3. Consideration | Email 3 (bridge) click rate | 5-8% |
| 4. Intent | Discovery calls booked/week | 5-15/week |
| 4. Intent | Call show rate | 70-80% |
| 5. Activation | Accounts → first operation | 60%+ within 30 days |
| 5. Activation | CA vs. self-directed split | 30%+ CA |
| 6. Retention/Referral | Referral rate | 15-20% of new clients |

## REAL BENCHMARKS — EMAIL (replaces the Stage 3 estimates above)

Source: real Mailchimp export, last 90 days (13 sends, 139,829 recipients).

| Metric | Estimated (above) | Real | 
|---|---|---|
| Open rate | 35-45% | **26.9%** |
| Click rate | 5-8% | **0.27%** |
| Delivery rate | — | 99.7% (healthy) |
| Unsubscribe rate | — | 0.08% (healthy) |
| Attributed revenue | — | $0 across 13 sends |

**This is a flag, not just a lower number.** A 0.27% click rate points to a subject line / CTA / segmentation problem, not a cadence problem. Investigate before simply resetting the benchmark downward — delivery and unsubscribe rates are both healthy, so the list itself isn't the issue.

**Rule of thumb when reading any export:** find the stage where the number is furthest below benchmark — that's where to focus, not wherever felt most visible that week.

---

## WHAT NOT TO CHASE
- Vanity metrics: total Instagram/Facebook followers
- Paid metrics (CPM, ROAS) — not relevant until Month 3+, and only if paid acquisition starts
- YouTube / X metrics — channels currently paused

---

## HOW TO USE THIS SKILL — THE PROMPT

```
Referencia /folionet-data.

Aquí está el export de Metricool / mis 5 números de esta semana:
[pegar datos]

Dime:
1. ¿Qué número se movió más — para bien o para mal?
2. ¿En qué etapa del funnel estamos más lejos del benchmark?
3. Una cosa concreta para hacer diferente la próxima semana.

No me des un resumen general — dame la decisión.
```

---

## MONTHLY REVIEW QUESTIONS (run once a month, not weekly)
- Which LinkedIn posts got the most engagement — what do they share (pillar, format, angle)?
- Which email subject lines had the highest open rates?
- How many discovery calls came from LinkedIn vs. email vs. referral?
- What % of new accounts are CA vs. self-directed?
- (Month 3+) Is the 3-profile ICP hypothesis holding up against who's actually opening accounts?

---

## SETUP STILL NEEDED
- [ ] Confirm Metricool is connected to LinkedIn + Instagram + Email (not yet confirmed as of this version)
- [ ] Weekly export scheduled for Friday, reviewed Monday morning before the trends-research session
- [ ] Platform CSV (registrations by country/source, first-operation status) — needed to set the Month 1 baseline for the north star

## UPDATE LOG
- v0 — July 2026 — built from the KPI framework doc. No real performance data yet — this skill tells you what to look for, not what happened. Update the first time a real Metricool export gets pasted in.
