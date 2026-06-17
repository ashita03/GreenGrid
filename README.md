# 🌱 GreenGrid

**Know your grid. Own your impact.**

GreenGrid is a sustainability intelligence platform built for data center operators making high-stakes, long-term energy decisions — where to site a facility, what to sign in a Power Purchase Agreement, and what their actual carbon footprint looks like right now.

Built in under 5 hours at **Code for Climate**, a hackathon hosted by **Mentor Me Collective** as part of **NYC Tech Week**. Winner of the **Most Impactful** award.

---

## Why this exists

Data centers are now one of the fastest-growing electricity consumers on the planet. Most operators outside of a handful of hyperscalers don't have the internal teams or budget to evaluate sites, contracts, and grid impact with real data. Decisions that lock in for 10–15 years are too often made with spreadsheets and gut instinct.

GreenGrid gives any operator — not just the largest ones — instant, data-backed answers to three questions:

1. **Where should we build?**
2. **Is this contract actually good for us?**
3. **What does our grid look like right now, and what are our alternatives?**

---

## What it does

GreenGrid has three modules, accessible from a single dashboard:

### 📍 Site Advisor
Score any US city across five sustainability dimensions — grid carbon intensity, water stress, climate suitability, renewable proximity, and renewable availability — and get a composite Green Siting Score with an AI-generated recommendation.

### 📄 Contract Analyzer
Upload or paste a Power Purchase Agreement and get an instant, AI-powered risk breakdown. Flags REC ownership issues, missing Scope 2 / GHG Protocol provisions, escalation risk, delivery guarantees, and termination terms — in plain English, in seconds.

### ⚡ Grid Reality Checker + Matchmaker
See your current grid's carbon intensity, renewable share, and fossil fuel mix, then get matched to community solar and REC options available in your region.

---

## Tech stack

| Layer | Tool |
|---|---|
| App build / hosting | [Base44](https://base44.com) — no-code/low-code app builder |
| AI contract analysis & recommendations | [Claude](https://www.anthropic.com) (Anthropic API) |
| Live grid carbon data | [Electricity Maps API](https://www.electricitymaps.com) |
| Community funding integration | [Givebutter](https://givebutter.com) (embedded campaign) |

GreenGrid was built entirely through vibe-coding on Base44 — natural language prompts translated directly into a working multi-module app, with structured data tables for city scores and renewable energy options, and live API calls for real-time grid intelligence.

---

## How it works

1. **Site Advisor** pulls a weighted composite score from five inputs, three of which are pre-loaded reference data and one of which (grid carbon intensity) can be sourced live from the Electricity Maps API.
2. **Contract Analyzer** sends uploaded or pasted PPA text to Claude with a structured prompt, which returns a JSON risk analysis — no document is ever stored.
3. **Grid Reality Checker** combines live or estimated grid data with a regional renewable options database to surface relevant community solar and REC opportunities, plus a community co-op funding option via Givebutter.

---

## Built by

Built by **[Your Name]** and **Shreya** at Code for Climate, hosted by Mentor Me Collective, NYC Tech Week — June 2026.

Thank you to the mentors and organizers who pushed our thinking in just a few short hours, and to everyone in the room building for the same reason we were.

---

## Disclaimer

GreenGrid is a hackathon prototype. City and renewable energy data is illustrative and pre-loaded for demonstration purposes. It is not a substitute for professional sustainability, legal, or compliance advice. Always consult a qualified advisor before making site selection or energy procurement decisions.
