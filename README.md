# Following the Money in Crypto Markets

**Reproduction package** for the Computation + Journalism 2026 short paper.

The printed QR code opens the short landing page: https://github.com/0xkleio/following-the-money-crypto-markets

This repository keeps the full package that used to live there.

> Kleio Kalamaridi, Catherine Sotirakou, Constantinos Mourlas.  
> *Following the Money in Crypto Markets: A Reproducible Blockchain-Forensic Workflow for Investigative Journalism.*  
> Computation + Journalism Symposium, October 2026, Evanston, Illinois.

This repository publishes the on-chain identifiers, tool links, sampling rules, and step-by-step procedure that the short paper could not fit. A second researcher should be able to open the linked explorers, recover the same addresses and paths, and separate **direct observations** from **third-party labels** and **inferences**.

The case study is drawn from the practical chapters of:

> Kleio Kalamaridi. 2026. *Investigative Journalism and Blockchain Forensics: An On-Chain Analysis of Celebrity and Political Memecoin Launches on Solana.* Undergraduate thesis, National and Kapodistrian University of Athens.

**Repo:** https://github.com/0xkleio/following-the-money

[Short paper](https://docs.google.com/document/d/1AIvPk2ACmHWIjopIiVs_E40KIiaQ5Jsl) · [Thesis](https://docs.google.com/document/d/1nloWcF4I7noLu75W5TOXTuEqTXzHjFqMe-2h2bJGKVA)

---

## How to use this package

1. Read the **interpretive caution** below.
2. Open the token and wallet tables in [`artifacts/`](artifacts/).
3. Follow the five stages in order. Do not skip to a later token unless Stage 3 or Stage 4 produced a direct lead.
4. Grade each link with the evidence-strength rubric.
5. Cross-check the Figma graph and the walkthrough video only after you have reproduced the path in a block explorer.

### Interpretive caution

This package reports **address-to-address transactions** and **time-stamped third-party labels**. It does **not** identify wallet controllers, beneficial owners, or legal responsibility.  
**Entity A** in the short paper is a neutral pseudonym for a third-party analytics label (Arkham Intelligence: *Kelsier Ventures*). The label is a lead, not proof of ownership, control, or liability.

---

## Visual and video supplements

| Resource | URL | What it shows |
|---|---|---|
| Full transaction graph (Figma) | [Thesis board, node `2983-802`](https://www.figma.com/board/On7B3joUExUT0xtcoTpICB/Thesis?node-id=2983-802) | End-to-end map of wallets, bridges, and cash-out hops used in the thesis |
| Overview of the same board | [Thesis board, node `0-1`](https://www.figma.com/board/On7B3joUExUT0xtcoTpICB/Thesis?node-id=0-1) | Entry view of the graph |
| Walkthrough video | [YouTube: `V7PD2sIA2eo`](https://www.youtube.com/watch?v=V7PD2sIA2eo) | Screen-recorded reconstruction from the $WAP social-media seed through $LIBRA and $MELANIA |

The Figma graph is the complete visual artifact; thesis figures and the short-paper figures are excerpts from it.

---

## Tools (all public)

| Stage | Tool | Role |
|---|---|---|
| Seed / price | [GMGN](https://gmgn.ai/), Dexscreener | Launch date, market-cap collapse, first-buyer ranking |
| Holder clusters | [Bubblemaps](https://v2.bubblemaps.io/) | Visualize early holders; distinguish *cluster* from *bundle* |
| Solana verification | [Solscan](https://solscan.io/) | Creator address, oldest funding tx, token mint |
| Cross-chain (transparent) | [deBridge](https://app.debridge.com/) | Backward trace of Solana funding to an EVM source |
| Cross-chain (opaque / mixer-like) | FixedFloat, SideShift | Correlate deposits and payouts by time and value |
| Graph + labels | [Arkham Intelligence](https://www.arkhamintelligence.com/) | Path visualization and third-party entity labels |
| USDC interchain | [Range](https://usdc.range.org/) | Forward / return USDC flows |

No paid API and no leaked records are required.

See the previous commit history of `following-the-money-crypto-markets` if you need the original long README verbatim. The stage-by-stage notes, addresses, and sampling files are preserved in `artifacts/`.
