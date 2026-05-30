# Kira PM Exercise 3 — The Bank of the Future
**Candidate:** Gerson Quintero · **One feature, defended hard.**

## The feature
> **Let agents bank — not just pay.**
> Kira gives every AI agent its own real bank account: a verified identity, a yield-bearing balance, and instant payout to local money (PIX/SPEI/cash) across 35+ countries — so the agents about to run LatAm's businesses can *hold, earn, and move* money themselves, not just spend on a human's card.

Everyone this year shipped how an agent *pays* (Visa, Mastercard, Google AP2, Coinbase x402, AWS). Nobody shipped the **account it pays *from***. That layer is empty, and it's exactly Kira's shape: KYB + a yield wallet + local rails in 35+ countries + an agent-native core.

## Repo map
| File | What it is |
|---|---|
| [`memo.md`](memo.md) | **The 1-page memo** — feature, why this one, who it changes, impact math, what would have to be true. Start here. |
| [`impact-model.md`](impact-model.md) | The bottoms-up math — **floor** (~$60K/yr saved per SMB, no adoption assumption) + **ceiling** (~$1.35B/yr at 1% adoption), every input tagged sourced/assumption. |
| [`benchmark.md`](benchmark.md) | The landscape read — 4 innovation waves (2015–2020, 2020–2025, failing-today, frontier) + cross-wave takeaways. |
| [`loom-script.md`](loom-script.md) | The 5-min pitch script with timing markers and delivery notes. |
| [`evidence/ai/`](evidence/ai/) | The AI reasoning loop — debate logs, not narration (see below). |

## `evidence/ai/` — the reasoning loop
| Log | The debate |
|---|---|
| [`01-candidate-generation-and-kill-the-pet.md`](evidence/ai/01-candidate-generation-and-kill-the-pet.md) | 5 candidates → steelman/kill-shot each → one winner + named rejections. |
| [`02-competitive-pressure-test.md`](evidence/ai/02-competitive-pressure-test.md) | The debate that reframed the pitch: "nobody builds for agents" is false → "nobody builds the *bank* for them." |
| [`03-impact-math-pressure-test.md`](evidence/ai/03-impact-math-pressure-test.md) | Floor-vs-ceiling; why the floor leads; grounding every input. |
| [`04-a2a-steelman-teardown-and-defense.md`](evidence/ai/04-a2a-steelman-teardown-and-defense.md) | The hardest 4-argument teardown of the idea, and the 4 defenses it survived. |

## Links
- **Loom (5-min pitch):** https://www.loom.com/share/96b2f1b3dec3448c9bf4d5557c235822
- **1-page memo:** [`memo.md`](memo.md)

---
*Built with Claude as a thinking partner — used to pressure-test and steelman the idea, not to summarize. The debate logs in `evidence/ai/` are the receipts.*
