# Folionet — Referral Program Brief (Draft)
**Prepared by:** creator:you
**Date:** July 2026
**Built from:** 06-kpis-measurement (retention/referral benchmarks), folionet-icp, folionet-pitch
**Status:** Draft mechanic ready for CEO review. Tracking method has one open decision that depends on product (see below) — everything else is ready to move on.

---

## WHY THIS MATTERS NOW
Per the KPI framework, referral rate is the **leading indicator for Stage 6 (Retention & Referral)** and is currently called out as "Folionet's most powerful marketing channel — and the most underused." Per `folionet-icp`, referral from a trusted colleague is also the **#1 trigger for registration** across all 3 profiles. This isn't a nice-to-have add-on — it's the highest-trust acquisition channel Folionet already has, just not systematized.

**Target (per KPI doc):** 15–20% of new clients referred.

---

## THE MECHANIC

**Who can refer:** Any active Folionet client, CA or self-directed.
**What they do:** Introduce a colleague, friend, or family member who fits the ICP (accumulated capital, distrust of local institutions, wants US market access) — via the warm-intro template in `folionet-pitch`, not a generic referral link blast.
**What happens next:** Referred contact gets the same discovery-call path as any warm lead, with a note that they came through a referral (this matters for tracking — see below).

## THE INCENTIVE — OPTIONS FOR CEO DECISION
*Draft, not finalized — needs compliance and CEO sign-off before launch, since anything resembling a cash incentive for referring investment clients has regulatory sensitivity (FINRA rules on referral compensation apply).*

| Option | Mechanic | Compliance risk |
|---|---|---|
| A — Relationship-based, no formal reward | CEO personally thanks referrers; no monetary or fee incentive | Lowest risk — recommended starting point |
| B — Fee credit | Small reduction in advisory fee for the referring client once the referred contact opens a CA account | Needs compliance review — fee-based incentives for referrals are common in RIA practices but must be disclosed |
| C — Cash/gift incentive | Direct payment or gift for successful referrals | Highest compliance risk — likely requires registered solicitor arrangements under SEC rules; **do not implement without CCO/compliance sign-off** |

**Recommendation:** Launch with Option A now — it requires no new compliance review and matches the ICP's actual behavior (referrals already happen through trust, not incentive-chasing). Revisit Option B only after compliance review, once volume justifies the formal structure.

---

## TRACKING METHOD — THE ONE OPEN QUESTION
The plan flags `HowDidYouFindUs` as an existing but untracked field in the product. This program can't measure its own success without it being instrumented.

**What's needed from product (not marketing's build):**
- `HowDidYouFindUs` field actively captured at signup, with "referral" as a selectable option and (ideally) free text for who referred them
- This data feeding into the same platform export used for the ICP/funnel CSV, so referral rate becomes one of the 5 weekly dashboard numbers over time

**Interim workaround until that's built:** Ask directly on the discovery call ("¿cómo llegaste a nosotros?") and log manually. Not scalable, but keeps the number visible in the meantime.

---

## REFERRAL ASK — WHERE IT LIVES
Per `folionet-pitch`, the referral ask should never feel transactional. Use the existing template:

> "Si conoces a alguien en tu círculo — colega, socio, familiar — que tiene capital acumulado sin un plan claro para hacerlo crecer, con gusto tengo una conversación con ellos, igual que la tuve contigo. No hace falta nada formal, solo preséntanos."

**Where to place this ask:**
- Post-first-operation milestone (client just activated — highest goodwill moment)
- End of a positive support interaction (per Day 3 ticket audit, once that data exists)
- Quarterly check-in emails/calls, if those exist in the client lifecycle

---

## NEXT STEPS
1. CEO decides between Option A/B/C above (recommend starting with A)
2. Flag the `HowDidYouFindUs` instrumentation need to product (this is their build, not marketing's — same boundary as the rest of platform tracking)
3. Once live, referral rate becomes a permanent line in the `folionet-data` weekly dashboard

## UPDATE LOG
- v0 — July 2026 — draft mechanic based on KPI targets and ICP referral behavior. No incentive structure finalized, no tracking instrumented yet.
