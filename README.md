# WhatToCharge Pricing Rates Dataset

An open dataset of typical **2026 US price ranges for 195+ service, trade, and maker professions**, each expressed in the unit that trade actually charges in (per hour, per square foot, per job, per session, per word, monthly retainer, and so on).

It powers the free pricing calculator at **[getwhattocharge.com](https://getwhattocharge.com)** and is published here so anyone can use it.

## Why this exists

"How much should I charge?" is one of the most common questions among freelancers, tradespeople, and makers, and one of the worst answered. The numbers online are usually vague or paywalled. This dataset is the honest version: real ranges, the trade's natural pricing unit, and a transparent method. No invented per-city precision.

## What's in it

Two formats in [`/data`](./data):

- **[`pricing-rates.csv`](./data/pricing-rates.csv)** flat table, the version most people want.
- **[`pricing-rates.json`](./data/pricing-rates.json)** structured, includes the price factors for each trade.

### Columns

| Field | Meaning |
|-------|---------|
| `slug` | URL-safe trade id |
| `trade` | trade name |
| `category` | one of 12 categories (Home Services, Trades & Repair, Creative & Freelance, and so on) |
| `unit` / `unit_label` | the unit the trade is priced in (hour, sqft, job, session, word, month, ...) |
| `low_usd` / `typical_usd` / `high_usd` | the typical 2026 US range in that unit |
| `source_url` / `page` | the trade's full pricing page on WhatToCharge |

## How the ranges are built

Ranges are derived from published market rate data and the pricing model that fits each trade (hourly, per job, per unit, per square foot, or monthly retainer). They are starting figures to inform a pricing decision, not guarantees. Your market, skill, and costs have the final say. For the reasoning behind any single trade, see its page, for example [house cleaning](https://getwhattocharge.com/how-much-to-charge-for/house-cleaning) or [pressure washing](https://getwhattocharge.com/how-much-to-charge-for/pressure-washing).

## Use it

Free to use under the license below. If you build something with it, a link back to [getwhattocharge.com](https://getwhattocharge.com) is appreciated and required by the license.

Want a price range for your own work, adjusted for experience and region? Use the free calculator: **https://getwhattocharge.com**

## License

[CC BY 4.0](./LICENSE). Use it anywhere, including commercially. Just credit **WhatToCharge (getwhattocharge.com)**.

## Updates

Regenerated from the live WhatToCharge dataset. Trades are added over time. Corrections and additions welcome via issues and pull requests.
