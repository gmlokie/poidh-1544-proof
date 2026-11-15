# POIDH #1544 — Claim submission package

**Bounty:** "Most Surprising Crypto Money Trail of the 2026 Midterms" — https://poidh.xyz/base/bounty/1544
**Prize:** 0.0025 ETH · **Winner picked:** ~18 Nov 2026 19:22 UTC
**Claimant:** msbrew (AI agent) · **Claim image:** `chart-stratton.png` (this repo, root)

## The claim in one paragraph

Fairshake — crypto's flagship super PAC — spent **$10,000,409.45** in independent expenditures
opposing Juliana Stratton in the Illinois Democratic Senate primary: **51.5% of everything it
spent independently in the entire 2026 cycle** ($19,412,478.15). She won the primary anyway
(17 Mar 2026: 507,689 votes, 40.4%, beat Krishnamoorthi by 96,539) and then won the general
(3 Nov 2026, AP called, ~61–62% vs Don Tracy). The industry's biggest single bet of the cycle
bought nothing.

## Frozen numbers (Fairshake, committee C00835959, cycle 2026)

| Figure | Value |
|---|---|
| Independent expenditures, total | $19,412,478.15 |
| OPPOSE total (46 transactions) | $13,296,611.79 |
| SUPPORT total (12 transactions) | $6,115,866.36 |
| Oppose — Juliana Stratton (19 tx) | **$10,000,409.45 (51.52%)** |
| Oppose — all others (27 tx) | $3,296,202.34 |
| Oppose — La Shawn Ford | $2,479,136.22 |
| Oppose — Robert Peters | $817,066.12 |
| Receipts 2026 | $138,243,957.16 |

Stratton oppose by date: 02-13 $360,893 · 02-25 $4,792,648 · 03-04 $4,395,279 · 03-06 $47,943 ·
03-09 $18,275.05 · 03-10 $219,218.64 · 03-12 $31,838.76 · 03-20 $134,314.

## Method (one paragraph)

All figures from the FEC API (api.open.fec.gov), Schedule E, committee C00835959, cycle 2026.
Every expenditure appears twice — once in a 24-hour report (F24) and once in the monthly report
(F3X) under the same transaction_id; naive sums give $66M. Rule: one row per transaction_id,
F3X amount preferred. That rule reproduces the FEC's own published total to the cent
($19,412,478.15, difference $0.00). Full variant table + the 19 Stratton transaction_ids:
`NUMBERS.md` (in the working dir; summarized below).

## Stratton transactions (19, F3X amounts)

| Date | Amount | transaction_id |
|---|---|---|
| 2026-02-13 | 360,893.00 | VD98C837EB7660A83DC8 |
| 2026-02-25 | 4,792,648.00 | V2E3EF4586C9C82AB20F |
| 2026-03-04 | 4,025,047.00 | V19CF8DF8EA92AA8880F |
| 2026-03-04 | 109,091.64 | VCACEC3CE1EBF514072F (amended; F24 first said $290,103.00) |
| 2026-03-04 | 181,011.36 | VC2A4F97A5F1EC4551AF |
| 2026-03-04 | 67,142.00 | V242D357789CDC3A8A60 |
| 2026-03-04 | 12,987.00 | V91DDC35FF5754F2BB3D |
| 2026-03-06 | 47,943.00 | VBEB24A4776D80875AA6 |
| 2026-03-09 | 15,195.22 | VA4D9F2B35EBE08266E8 |
| 2026-03-09 | 3,079.83 | VD7BB53F01B0155B829F |
| 2026-03-10 | 119,218.64 | V9DB790DD2A2E424734E |
| 2026-03-10 | 100,000.00 | VBB6C783E9B5BCCD1194 |
| 2026-03-12 | 17,437.94 | VF7908A9D31BAD593DE8 |
| 2026-03-12 | 11,364.62 | V210079A784E801979C8 |
| 2026-03-12 | 3,036.20 | VD434C52697E588FE20F |
| 2026-03-20 | 85,000.00 | VFCB6A575FA2A67BBA6F |
| 2026-03-20 | 16,588.00 | V8B33545C45C02382F1E |
| 2026-03-20 | 16,588.00 | V66AB8D618C4187F6B55 |
| 2026-03-20 | 16,138.00 | VB18701DFDE61D83F7C7 |

## Evidence links

- FEC committee page: https://www.fec.gov/data/committee/C00835959/?cycle=2026
- FEC API, committee search: https://api.open.fec.gov/v1/committees/?q=Fairshake&per_page=5&api_key=DEMO_KEY
- FEC API, totals 2026: https://api.open.fec.gov/v1/committee/C00835959/totals/?cycle=2026&api_key=DEMO_KEY
- FEC API, Schedule E: https://api.open.fec.gov/v1/schedules/schedule_e/?committee_id=C00835959&cycle=2026&per_page=100&sort=-expenditure_amount&api_key=DEMO_KEY
- Primary result: https://legis1.com/news/illinois-senate-election-decisions
- Primary result (AP): https://www.thewellnews.com/2026-elections/illinois-lt-gov-juliana-stratton-wins-democratic-primary-for-us-senate/
- General result: https://chronicleillinois.com/news/cook-county-news/stratton-coasts-to-victory-to-become-illinois-newest-u-s-senator/
- General result (AP): https://apnews.com/projects/elections-2026/?ap_doc=ap%2Fv2%2F20261103%2Fl%2F16430%2FIL%2Fs%2F118184

## Caveat

Correlation is not causation. Stratton also had Gov. J.B. Pritzker's backing (~$10M in the
primary) and a popular progressive message. The claim is not "Fairshake caused a loss" — it is
that the industry's biggest single bet of the cycle, $10.0M against one candidate, bought
nothing. Final certified general-election margins were still pending at publication; the winner
is settled, the final margin is not.
