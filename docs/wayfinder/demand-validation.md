# Demand validation: surviving keyword sets

Effort: **Wayfinder map: profitable niche-utility app spec** (see [the map](https://github.com/nadav-galili/get-rich-or-die-trying/issues/1)). Resolves [Validate demand for surviving keyword sets](https://github.com/nadav-galili/get-rich-or-die-trying/issues/7).

**Method note — read first**: Apple Search Ads API access does not exist on this account, and no paid ASO tool is available. True ASA popularity scores (0–5) are **unobtainable here**. Instead, demand is triangulated from four free public proxies, each confidence-labeled:

1. **Captured demand** (high confidence): lifetime ratings + recent-review velocity on iOS (reviews RSS, most-recent 50 — tighter span = hotter), and Google Play install floors from detail pages.
2. **Supply-side conviction** (medium confidence): how many apps exist in the space and their age — a flood of brand-new 0-rating apps means builders *believe* there's demand, but proves nothing about searchers.
3. **Web-side query existence** (medium confidence): Google autocomplete completions — proves the phrase is typed on the *web*, which correlates with App Store search but is not the same population.
4. **Cross-store confirmation** (high confidence): the same niche on Play (install counts are public there).

All data pulled 2026-09-06, US store/geo. **Overall confidence: medium.** The one axis that would upgrade it — ASA popularity — requires an Apple Search Ads account and is worth revisiting only if the choice stays deadlocked.

---

## The demand-ranked table

| Rank | Idea / cluster | Demand verdict | Confidence | Evidence (proxies above) |
|---|---|---|---|---|
| **1** | **Pocket Archaeologist** (thrift/vintage ID + value) | **Validated** — real, captured, and *heating* | **High** | Only cluster where users demonstrably search-and-install: ThriftAI 20K iOS ratings with ~17 recent reviews/mo (50 reviews spanning Jun 10–Sep 1); Curio 15K @ ~12/mo; Zophi 10.6K; Gemli 4.1K iOS + **100K+ Play installs** (confirmed on detail page). Play search "thrift appraiser" surfaces ~10 dedicated apps; "Antique Identifier, Appraisal" shows 100K+ Play installs. Google autocompletes "app to check resale value of items" (direct app-intent) and a rich "thrift flipping" tail (clothes, furniture, reddit, business). |
| **2** | **Shelf Whisperer** ("should I buy" scanner) | **Unproven — gold-rush supply, zero captured demand** | Medium-low | iOS "should i buy": 14 results, **every one shipped Dec 2025–Sep 2026**, every one 0–2 ratings. A dozen indie builders just entered (names like "Should I Buy? AI Decision" smell of LLM-hype copycats) — but **not one has traction anywhere**, including Play (Should I Buy This? by KindLogic: 100+ installs). Google: "should i buy" is typed hugely but resolves to stocks/PS5/games; the aisle-shopping phrasing has no web tail ("should i buy this app" → Apple products). Interpretation: builders believe; no proof searchers do. First-mover window at the copycat layer is closing fast. |
| **3** | **Contract Cockpit** (plain-English lease reader) | **Unproven — web query exists, app demand unproven** | Medium-low | Google autocomplete for "lease analyzer" is real and app-flavored: "lease analyzer ai", "car lease analyzer", "lease deal analyzer" — the strongest web-existence signal of the blue-ocean set. But captured demand is zero everywhere: iOS incumbents 0–53 ratings (AI Contract Analyzer & Sign 53, all shipped 2025–26); Play "AI Legal Contract Analyzer" 100+ installs; LeaseLogic (AI Lease Review, Play) **15+ installs**. Nobody has found searchers; nobody has died trying either. |
| **4** | **Laundry Sorter** (care-tag decoder) | **Cold — web info-demand, not app-demand** | High | "laundry symbols meaning" has a rich evergreen autocomplete tail (chart, pdf, UK, Japan) — but it's *look-it-up-once* intent, served by web charts. App-side: iOS leader Laundry Lens has 278 lifetime ratings and only 26 recent reviews spanning **2020→2025** (~0.4/mo — cold). Play shows 10+ tiny dedicated apps (Laundry Symbols, Decoder, Care Guide, Scanner AI…) with no traction leader. Demand exists; it doesn't monetize as an app. |
| **5** | **Sim Sim** (haggling assistant) | **Unproven — bleakest; zero signals on every surface** | Medium-low | No captured demand (HaggleBuddy on Play: **10+ installs**). No web tail ("haggle app" autocompletes only to an Australian Pty Ltd and Hagglezon — an Amazon repricer, different intent). Play "haggle" top result is a pawn-shop *game*. Not even gold-rush supply interest. If demand exists, nothing on the public internet hints at it. |

---

## Separated clusters, as the ticket asked

**Validated demand (Pocket Archaeologist only)**: searchers provably install apps from this keyword space, on both stores, at indie scale. The cost: the space is no longer blue ocean — and it heated *while we watched*. **AntiqSnap: Antique Identifier** (Next Vision — the studio behind PictureThis, 1.1M ratings) shipped Oct 2025 and has **31K lifetime iOS ratings in ~11 months** with the hottest recent-review velocity of the cluster (~33/mo, 50 reviews spanning Jul 26–Sep 3). Cross-promotion from a 1.1M-rating sibling is how. The shortlist's "no big studios" read is now stale: a big-studio-adjacent player is in the exact space and winning.

**Blue-ocean unproven (Shelf Whisperer, Contract Cockpit, Sim Sim)**: zero captured demand on either store. Within that, a clear gradient:
- Shelf Whisperer has the most *activity* (13+ new indie entrants in 9 months — conviction, not proof; window closing)
- Contract Cockpit has the most *web evidence* ("lease analyzer ai" is a real typed query with no app serving it — the purest "gap" of the three)
- Sim Sim has neither.

---

## What this means for Choose the app idea

1. **The demand-vs-sharks tension sharpened, not resolved.** Pocket Archaeologist is the only validated-demand survivor, and it now carries a heating shark (AntiqSnap) plus five funded-feeling indies. Entering means out-executing a 33-reviews/mo incumbent with a 1.1M-rating megaphone.
2. **The blue-ocean survivors are a bet on invisible demand.** Shelf Whisperer: fast-closing window, cheapest to test. Contract Cockpit: rare-cadence premium fit, a real web query nobody serves, but zero proof searchers reach the App Store. Sim Sim and Laundry Sorter: demand evidence argues to drop both at choice time.
3. **A new option the data suggests**: Shelf Whisperer's LLM-cost profile was flagged as needing hard per-scan caps, but its natural phrasings ("should i buy", "is this worth anything") live adjacent to Pocket Archaeologist's *validated* value-verdict demand — a "should I buy this thrift find?" app could enter through the validated door (thrift keywords) while offering the broader purchase-verdict UX. The choice ticket should at least consider entering the validated cluster via a differentiated angle rather than treating validated-vs-blue-ocean as binary.

**Confidence ceiling for all of the above: medium.** True ASA popularity scores would firm up ranks 2–4; provisioning Apple Search Ads API access (~a day, requires an Apple developer + campaign setup) is a cheap follow-up if and only if the choice grills deadlock on this evidence.
