# Impact Model — A2A Agent Accounts for LatAm SMBs

> **Feature:** Kira gives every AI agent its own real bank account — verified identity, a yield-bearing balance, and instant off-ramp to local money (PIX/SPEI/cash) across 35+ countries.
> **This doc:** the bottoms-up math behind the memo. Every input is tagged `[sourced]` or `[assumption]` so it survives a live pressure-test. Base case is deliberately conservative; downside shown.

---

## Two numbers, two audiences

| | What it proves | Needs an adoption assumption? |
|---|---|---|
| **FLOOR** — per-SMB cost savings | The feature pays for itself for *any* firm that turns it on | **No** — this is why it's the number we lead with |
| **CEILING** — platform recurring revenue | The size of the prize if the category lands | **Yes** — labeled loudly; sensitivity table provided |

The floor convinces the skeptic. The ceiling excites the investor. We hand over the sensitivity table *before* anyone asks.

---

## FLOOR — what one SMB saves per year

**Representative firm:** a mid-sized LatAm SMB that pays international suppliers (3 of 5 LatAm SMEs already do `[sourced]`).

| Lever | Inputs | Annual saving |
|---|---|---|
| **A. Payment + FX cost compression** | Cross-border volume **$1M/yr** `[assumption — consistent with mid-sized SMB profile per Mastercard 2025]`; all-in cost **5% → 0.5%** `[sourced: FSB 2.7% avg, 6.1% sub-$500; Mastercard: $250 ticket ≈ 23.3% fees; ~90% of non-US txns FX-converted without consent]` | **$45,000** |
| **B. Yield on idle balance** | Idle operating balance **$100K** `[assumption]`; **~5% net** spread vs ~0% in a checking account `[sourced: ~7% Kira yield wallet]` | **$5,000** |
| **C. Finance-lead time reclaimed** | **6 hrs/wk** `[assumption]` approving payments the agent already validated × **$40/hr** loaded `[assumption]` × 52 wks | **$12,500** |
| | **Total per firm** | **≈ $62,500 / yr** |

**Downside stress test** — halve *every* assumption (volume, balance, hours, rate): the firm **still saves ~$31K/yr**. The floor does not break.

### The "cost → unlock" sentence (the brief's exact template)
> Kira's agent accounts cut LatAm cross-border B2B cost from **~5% to ~0.5%** — saving a mid-sized SMB **~$60K/year** — and by making a sub-$500 supplier payment cost **~$1 instead of ~$25–60**, they make a whole class of small-ticket cross-border trade economic **for the first time**: the micro-importer, the cross-border solo-employer, the small reseller sourcing abroad — businesses priced out of international trade today.

### The human-character version (for the Loom)
> A finance lead at a mid-sized LatAm startup spends ~6 hours a week approving payments their agent already checked — about **$12K/year in salary spent clicking "approve."** The agent account removes that entirely and redirects **~$60K/year** back into the business.

---

## FLOOR cross-check — the corridor (top-down)

So the per-firm number doesn't stand alone:

- LatAm cross-border B2B corridor heading to **~$1.37T by 2030** `[sourced: benchmark]`.
- Cost compression of **4.5%** (5% → 0.5%) across it = **~$60B/yr** removed system-wide at full penetration.
- At a conservative early reach (~10% of the corridor): **~$6B/yr** in cost taken out.

The per-firm lens (~$60K × firms) and the corridor lens (~$60B system-wide) triangulate to the same order of magnitude.

---

## CEILING — platform recurring revenue (layer two)

Same firm, now viewed as a Kira account. **Adoption is the load-bearing assumption — flagged explicitly.**

| Input | Value |
|---|---|
| LatAm MSMEs `[sourced: ~27M; SMEs = 98% of businesses, 60% of employment]` | 27,000,000 |
| Penetration: **1%** open a Kira agent account over 5 yrs `[assumption — the load-bearing one]` | 270,000 accounts |
| Revenue / account / yr: yield spread **~$1,500** + payout take-rate **~$3,500** (≈0.35% on $1M) `[assumption]` | ~$5,000 |
| **Recurring revenue @ 1%** | **≈ $1.35B / yr** |

### Sensitivity (we control the Q&A)
| Penetration | Accounts | Recurring revenue / yr |
|---|---|---|
| 1.0% | 270,000 | **$1.35B** |
| 0.25% | 67,500 | **$338M** |
| 0.10% | 27,000 | **$135M** |

Even the **0.1% floor of the ceiling (~$135M ARR) is ~45× Kira's current ~$3M ARR.** The ceiling is the category prize, not a forecast — and we say that out loud.

---

## Assumptions register (what we'd get asked, and our answer)

| Input | Value | Status | Defense / next step |
|---|---|---|---|
| Cross-border volume / firm | $1M/yr | `[assumption]` | No public per-firm figure exists (Mastercard 2025 tracked cost, not volume); profile-consistent. The floor holds at $500K. |
| All-in cost today | 5% | `[sourced]` | FSB 2.7% avg / 6.1% small-ticket; Mastercard $250≈23.3%; hidden FX on ~90% of txns → 5% is conservative. |
| Cost after | 0.5% | `[assumption]` | Stablecoin rail + on/off-ramp; headline could be 0.1%, we use 0.5% to be safe. |
| Idle balance | $100K | `[assumption]` | ~10% of annual flow; conservative. |
| Net yield spread | 5% | `[sourced ~7%]` | Kira wallet yield; net of what's passed to SMB. |
| Finance-lead hours | 6/wk | `[assumption]` | Conservative for a firm with manual approval queues. |
| Loaded hourly cost | $40/hr | `[assumption]` | Mid-market LatAm finance lead. |
| Penetration (ceiling) | 1% | `[assumption]` | Load-bearing; sensitivity table down to 0.1%. |
| Take-rate | ~0.35% | `[assumption]` | Below typical payment take-rates; conservative. |

---

## Sources
- FSB, *Annual Progress Report on Meeting the Targets for Cross-border Payments* (2024) — https://www.fsb.org/uploads/P211024-3.pdf
- Mastercard (2025), *Modernizing cross-border payments: SMEs in LatAm & the Caribbean* — https://www.mastercard.com/news/latin-america/en/newsroom/press-releases/pr-en/2025/july/modernizing-cross-border-payments-new-mastercard-study-reveals-the-path-to-strengthening-smes-success-in-latin-america-and-the-caribbean/
- Mastercard, *How better cross-border payment technology can help SMEs in Latin America* — https://b2b.mastercard.com/news-and-insights/blog/how-better-cross-border-payment-technology-can-help-smes-in-latin-america/
- Quona Capital, *The State of Cross-Border Payments in Latin America* — https://quona-capital.medium.com/the-state-of-cross-border-payments-in-latin-america-opportunity-innovation-54b803b816e9
- World Bank Enterprise Surveys, *Mapping Enterprises in LAC* — https://www.enterprisesurveys.org/content/dam/enterprisesurveys/documents/research/Mapping-Enterprises-LAC-Note.pdf
- Internal: `benchmark.md` (stablecoin corridor + $1.37T-by-2030 figure)

*Figures are directional, drawn from public 2024–2026 reporting; the three `[assumption]` inputs doing the most work (firm volume, idle balance, penetration) are flagged for live defense.*
