# Let agents bank — not just pay.

*Kira PM Exercise 3 · One feature, defended hard · Gerson Quintero*

**The feature.** Kira gives every AI agent its own real bank account: a verified identity, a yield-bearing balance, and instant payout to local money — PIX, SPEI, cash — across 35+ countries. Today an agent can *spend* (a card bolted onto its human owner). It cannot *bank*: it has no identity a counterparty trusts, no balance that earns, no way to land value in the real local economy. Kira gives it all three. The first time you watch an agent pay a supplier in São Paulo, hold the float at ~7%, and settle the change to a wallet in Bogotá — with no human clicking anything — you wonder how it ever worked the other way.

**Why this one.** Everyone is racing to teach agents to *pay*: Visa, Mastercard, Google's AP2, Coinbase's x402, and AWS all shipped agent-payment *rails* in the last year. Nobody is building the **account they pay *from*** — identity, yield, and a local off-ramp. That layer is empty, and it is exactly Kira's shape. It needs four assets stacked that only Kira holds together: KYB, a yield wallet, local rails in 35+ countries, and an agent-native core. A neobank can't ship it (not agent-native); a card network can't ship it into LatAm (no local rails); a crypto wallet can't ship it (no compliance, no off-ramp).

**What I rejected.** *CFO-in-an-agent* — Kira already sells it ("AI-Powered Treasury & Wallets"); not non-obvious. *Self-reconciling payouts* — best moat of the set, but a back-office win with no story you can *feel*. *Programmable conditional payouts* — incremental, and it leans on dispute/event-verification, which isn't Kira's muscle. *Compliance-as-code FX* — narrow plumbing, no headline. (I am **not** claiming "nobody builds for agents" — that's false. I'm claiming nobody builds the *bank*.)

**Who it changes.** Start with **Sofía**, the finance lead at a 60-person São Paulo startup. She spends ~6 hours a week approving supplier payments her agent already validated — about **$12K/year in salary spent clicking "approve"** — and loses 3–6% on every cross-border transfer while idle cash earns nothing. With an agent account, the agent pays suppliers, holds float at ~7%, and settles to local rails; Sofía touches only the exceptions. Next, the **developer** who built Sofía's agent: one Kira API call makes it bankable and compliant, instead of months stitching wallet + KYB + 35-country payout. Then the **supplier** in Lima — paid in local money in seconds, not days.

**The impact.**
- **Floor (no adoption assumption):** cuts LatAm cross-border B2B cost from **~5% → ~0.5%**, saving a mid-sized SMB **~$60K/year** (~$31K even if I halve every input). By dropping a sub-$500 payment from ~$25–60 to ~$1, it makes small-ticket cross-border trade viable **for the first time** — the micro-importer priced out today. Across a corridor heading to **~$1.37T by 2030**, that's **~$60B/year** of cost removed.
- **Ceiling (adoption flagged):** at **1%** of LatAm's ~27M SMBs, **~$1.35B/year** recurring (yield spread + take-rate); even the 0.1% case (**~$135M**) is **~45× Kira's ARR**. The floor convinces the skeptic; the ceiling excites the investor. Full math + sources: `impact-model.md`.

**What would have to be true.**
1. **Speed** — the rail is crowding fast; Kira's durable moat is LatAm-local settlement + compliance, a ~6–12 month window to plant the flag.
2. **Legality** — this needs *no new legal category*: an agent account is a **corporate account with programmable delegation** (banks already run delegated multi-user authorization). Issue it under a verified business principal with scoped mandates, prove it with one lighthouse customer, build the precedent. Regulatory complexity is the moat, not the blocker.
3. **Adoption** — the agents already exist (treasury, procurement, payroll), running on human credentials today; the Year-1 beachhead just *formalizes* them, so revenue doesn't wait on the machine economy.
4. **Defensibility vs the giants** — model providers build intelligence, not LatAm rails; an OpenAI "agent wallet" is generic USD. The likely outcome is **partnership** — Kira as the financial execution layer for agents in LatAm — not a race a $8.7M company loses.
5. **The metric, honestly** — not a billion humans logging in, but a billion people served *by* agents that bank with Kira. That's the timeline I'll defend.

---
*Companion docs in repo: `benchmark.md` (landscape) · `impact-model.md` (math + assumptions) · `evidence/ai/` (AI debate logs).*
