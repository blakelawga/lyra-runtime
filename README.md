<p align="center">
  <img width="420" alt="MemePit Logo" src="https://raw.githubusercontent.com/kalshi-degen/memepit/main/assets/memepit-banner.png">
</p>

<h1 align="center">MemePit</h1>
<p align="center"><strong>High-velocity meme monetization layer for Kalshi.</strong></p>
<p align="center">
  The official (and completely unsanctioned) degenerate vertical where the timeline gets priced, ratio’d, and liquidated in real time.
</p>

---

## Overview

**MemePit** is a high-throughput, chaos-optimized prediction market runtime built by a Kalshi employee who got bored during compliance review. 

It turns pure internet schizophrenia into tradable binary contracts with sub-60-second resolution windows. No more waiting for quarterly earnings — bet on whether the next viral tweet hits 500k likes before lunch, if the current main character will be canceled by EOD, or which Solana cat coin rugs first.

MemePit collapses the entire attention economy into a **single low-latency execution layer** where vibes are the oracle, wojaks are the UI, and liquidation is guaranteed.

---

## Core Philosophy

- Truth is whatever gets the most YES volume before expiry.
- Every market must be at least 40% unhinged.
- Compliance is a suggestion, not a feature.
- If regulators don’t side-eye it, it’s not working hard enough.

---

## System Overview

MemePit operates as a **real-time meme settlement engine** that ingests signals from Twitter, TikTok, 4chan, and group chats, then surfaces the most degenerate contracts possible.

It emphasizes:
- **Hyper-short expiry** (minutes to 48 hours)
- **Vibe-Based Resolution** powered by community voting + on-chain snapshots
- **Schizo Market Creation** — any user can spin up a contract in <30 seconds
- **Live Heatmap** of what’s currently pumping in the meme meta
- **Degen Leaderboards** with public PNL and shame badges

---

## Key Features

- **Instant Market Launcher** — Drop a tweet link + “Will this hit 1M likes?” and it’s live.
- **Meme Oracle Network** — A decentralized council of degens + Grok + community upvotes for resolution.
- **Wojak Liquidation Engine** — Automatic market close + payout when the meme dies.
- **Rug Score™** — Real-time probability that a trending coin is about to zero.
- **Ratio Insurance** — Bet against your own tweet getting flamed.
- **CEO Meltdown Market** — Weekly contract on which founder will post the most regarded tweet.
- **Dark Mode Only** with animated pepe cursors.

---

## Technology Stack

- **Next.js + Tailwind** — Because it had to ship yesterday
- **Supabase + Redis** — For that sweet real-time degen experience
- **Grok + Claude** — LLM judges for borderline market approval
- **Twitter API + Firehose** — Primary truth source (until it breaks)
- **Solana Pay** — Optional on-chain settlement for the truly regarded
- **Framer Motion** — Smooth wojak animations on every resolution

---

## Quick Start

### 1. Clone the repository

npm install
npm run dev

# Example: Will this tweet get ratio'd before midnight?
npm run create-market \
  --title "Will @dril tweet something more regarded than usual tonight?" \
  --expiry "2026-05-02T23:59:59Z" \
  --category "schizo"
```bash
git clone https://github.com/kalshi-degen/memepit.git
cd memepit
