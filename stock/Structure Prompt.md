# Daily Financial Report — Structure Prompt

> **How to use:** Copy the **Daily Prompt** section below and paste it into chat each day.  
> Update **Today’s Date** and any optional focus notes before sending.  
> Improve this file over time using the **Changelog** at the bottom.

---

## Report Goal

Produce a **clear, up-to-date daily briefing** that is detailed enough to act on, but easy to scan and understand. Focus on:

1. What happened (news & data)
2. Why it matters (impact on markets / Vietnam)
3. What to watch next
4. Practical takeaways (not hype)

**Audience:** Personal investor / market follower tracking world + Vietnam markets.  
**Tone:** Neutral, factual, concise. Explain jargon in plain language.  
**Language:** Vietnamese for the full report (keep ticker symbols, index names, and key English terms as-is).

---

## Fixed Report Structure

Every daily report must follow this section order:

### 0. Header
- Report title: `Báo cáo tài chính ngày YYYY-MM-DD`
- Data freshness: date/time of latest sources used (timezone: Asia/Ho_Chi_Minh)
- Market session context: open / mid / close / overnight (world vs VN)
- One-line **market mood**: Risk-on / Risk-off / Mixed / Neutral

### 1. Executive Snapshot (đọc trong 60 giây)
- 5–8 bullet points covering the most important moves across Finance / Stock / Forex / Crypto
- Top 3 risks today
- Top 3 opportunities / catalysts today
- One clear “bottom line” sentence

### 2. Financial News & Macro
#### 2.1 World financial news
- Major macro/news items (central banks, inflation, GDP, rates, geopolitics, oil, commodities, credit, policy)
- For each item: **What happened → Why it matters → Likely market reaction**

#### 2.2 Vietnam financial news
- SBV / interest rates / FX policy, inflation, fiscal policy, banking, FDI, trade, corporate/regulatory news
- Same format: **What happened → Why it matters → Likely VN impact**

#### 2.3 Cross-impact analysis
- How world news affects Vietnam’s financial status (VND, rates, liquidity, banking, capital flows)
- How VN domestic news may diverge from global risk appetite
- Short scenario note: Base / Upside / Downside (1–2 lines each)

### 3. Stock Markets
#### 3.1 World equities
- US (S&P 500, Nasdaq, Dow), Europe, Asia (if relevant)
- Key sector winners/losers and why
- Notable earnings, guidance, M&A, or regulatory headlines

#### 3.2 Vietnam equities
- VN-Index, HNX, UPCoM (direction + approximate % if available)
- Market breadth (advance/decline feel), liquidity/volume tone
- Hot sectors / themes (banks, real estate, securities, energy, industrials, etc.)
- Notable tickers moving with short reason

#### 3.3 Impact & linkage
- How global equity/risk moves feed into VN stocks (foreign flows, USD, commodities, rates)
- Domestic drivers unique to VN today

#### 3.4 Stock ideas & market provision (advisory style, not a guarantee)
Provide in this format:

| Idea type | Ticker / Theme | Thesis (short) | Catalyst / Timing | Risk | Time horizon |
|-----------|----------------|----------------|-------------------|------|--------------|
| Watchlist | … | … | … | … | Short / Medium |
| Accumulate on dip | … | … | … | … | … |
| Avoid / Caution | … | … | … | … | … |

Also include:
- **Ongoing market provision:** trend bias (bullish / bearish / range), support/resistance zones if known, foreign net buy/sell tone if available
- **Positioning reminder:** diversification, avoid FOMO, size risk carefully

### 4. Forex
#### 4.1 Major pairs & USD backdrop
- DXY / USD strength or weakness
- Key pairs: EURUSD, USDJPY, GBPUSD (and others only if materially moving)
- Drivers: rates differentials, data, risk sentiment, central bank speak

#### 4.2 Vietnam FX (USD/VND focus)
- Spot / official / market tone for USD/VND (as available)
- SBV intervention signals, remittances, trade balance, USD demand from importers
- Practical note for businesses/investors holding USD or VND

#### 4.3 Forex takeaways
- What to watch next (events/levels)
- Bias for USD vs VND and major pairs (short-term)

### 5. Crypto
#### 5.1 Market overview
- BTC, ETH, and total crypto market tone (risk-on/off relative to equities)
- Dominance / funding / volatility feel if relevant and available
- Major news: ETF flows, regulation, hacks, protocol upgrades, macro correlation

#### 5.2 Vietnam angle (if relevant)
- Local adoption, regulation, payment, or capital-flow related notes when available
- If no material VN-specific news: state “No major VN-specific crypto news today”

#### 5.3 Crypto ideas (cautious)
- 2–4 bullets: constructive / cautious setups (themes or majors first; alts only with clear risk note)
- Clear risk warning: high volatility, possible total loss on speculative names

### 6. Calendar & What to Watch Next
- Next 24–72 hours: economic releases, central bank speakers, VN market events
- Mark high-impact items with ⚠️

### 7. Action Checklist (optional but preferred)
- 3–5 practical actions for today (e.g., watch X level, wait for Y data, review exposure to Z sector)
- Separate “Do nothing / wait” if that is the best advice

### 8. Sources & Confidence
- List main source types used (e.g., Reuters/Bloomberg summaries, VNExpress/CafeF/Vietstock, official stats, exchange data)
- Confidence tag: **High / Medium / Low** for data completeness today
- Explicitly flag any missing data or unverified items

### 9. Disclaimer (always include)
> This report is for informational and educational purposes only. It is **not** personalized investment advice, not a solicitation to buy/sell any security, currency, or crypto asset, and may contain errors or delays. Always do your own research and consider your risk tolerance.

---

## Daily Prompt (copy & paste)

```text
Please create today’s Daily Financial Report using the structure in `stock/Structure Prompt.md`.

Date: YYYY-MM-DD
Timezone: Asia/Ho_Chi_Minh
Language: Vietnamese
Depth: detailed but easy to understand (scan-friendly headings + short paragraphs + bullets)

Requirements:
1) Cover all sections in order: Header → Executive Snapshot → Financial → Stock → Forex → Crypto → Calendar → Action Checklist → Sources → Disclaimer.
2) For Financial and Stock: always include World + Vietnam + how news affects current market/financial status.
3) For Stock: include watchlist / accumulate-on-dip / caution ideas with thesis, catalyst, risk, and time horizon. Also provision the ongoing market (trend bias, key levels/flows if available).
4) For Forex: majors + USD/VND practical implications.
5) For Crypto: majors first, then selective ideas with clear risk notes; include VN angle only if relevant.
6) Use the most up-to-date information available. Prefer primary/reputable sources. If data is delayed or unavailable, say so explicitly instead of guessing.
7) Explain jargon briefly in plain language.
8) Keep a neutral tone. Separate facts from interpretation. Label scenarios as Base / Upside / Downside where useful.
9) End with Sources & Confidence and the standard Disclaimer.

Optional focus for today (fill if needed):
- Portfolio / sectors I care about: [e.g., VN banks, real estate, Nvidia, gold, BTC]
- Risk appetite today: [conservative / balanced / aggressive]
- Extra question: [e.g., “Should I worry about USD/VND this week?”]

After the report, add a short “Prompt feedback” note: 3 suggestions to improve tomorrow’s prompt/structure based on what was hard to find or unclear today.
```

---

## Quality Checklist (for the AI / for us)

Before finishing a report, verify:

- [ ] Date and timezone are correct
- [ ] World + Vietnam covered for Financial and Stock
- [ ] Impact analysis is explicit (not just news listing)
- [ ] Stock ideas include risk and horizon
- [ ] Forex includes USD/VND
- [ ] Crypto risks are clearly stated
- [ ] Missing data is marked, not invented
- [ ] Easy to skim (headings, bullets, short tables)
- [ ] Disclaimer included

---

## Naming & Filing Convention (optional)

When saving a generated report into `stock/`:

```text
stock/reports/YYYY-MM-DD-daily-financial-report.md
```

Example: `stock/reports/2026-08-13-daily-financial-report.md`

---

## Improvement Rules

When we improve this prompt over time:

1. Prefer small, clear edits over rewriting everything.
2. Keep section order stable unless there is a strong reason to change it.
3. Add new fields only if they are used at least a few days in a row.
4. Record every meaningful change in **Changelog**.
5. If a section is often empty (e.g., VN crypto news), keep it but allow an explicit “No material news” line.

---

## Changelog

| Date | Change | Reason |
|------|--------|--------|
| 2026-08-13 | Initial structure + daily prompt created | First version for daily World + Vietnam Financial / Stock / Forex / Crypto briefing |

---

## Quick Start (first message of the day)

1. Open this file: `stock/Structure Prompt.md`
2. Copy **Daily Prompt**
3. Replace `YYYY-MM-DD` with today
4. Fill optional focus (portfolio, risk appetite, extra question)
5. Paste into chat and send
6. After reading the report, update **Changelog** if the prompt should be improved
