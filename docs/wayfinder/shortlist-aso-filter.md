# Shortlist: ASO shark filter results

Effort: **Wayfinder map: profitable niche-utility app spec** (see [the map](https://github.com/nadav-galili/get-rich-or-die-trying/issues/1)). Resolves [Shortlist ideas by ASO shark filter](https://github.com/nadav-galili/get-rich-or-die-trying/issues/3).

**Method**: iTunes Search API, US store, `entity=software`, top-10 per candidate keyword. Rating counts are **lifetime** (the public API exposes no recent-only window) — used as the "recent reviews" proxy, so thresholds skew conservative. Google Play (`gl=us`) spot-checked for every survivor and borderline cut. Locked heuristic: disqualify if 3+ of top-10 are big studios/brands, or if all top-10 have 10K+ ratings; opportunity zone = indies under ~1K ratings with visible velocity.

**Result: 5 of 15 survive** — ranked below.

---

## Survivors (ranked)

### 1. Shelf Whisperer — "should I buy this?" scanner

| Keyword | Top-10 evidence |
|---|---|
| "should i buy" | **9 results, every one an indie with 0–2 lifetime ratings** (Should I Buy This? – Worth It: 0; ShouldIBuy: 0; Should I Buy This? – Spending: 2). No brand in sight. |
| "shopping advisor" | Sharky — Consumer Reports 64K, LTK 460K, Voodoo 4.5K. Discard this phrasing; the natural-query phrasing is the asset. |
| Play "should i buy this" | One dedicated app (com.kindlogicworks.shouldibuythis, **100+ downloads**) among otherwise unrelated giants. Space effectively unclaimed. |

**Read**: cleanest blue ocean of the longlist — zero sharks, zero real incumbents, and the keyword reads like a real search query. **Caveat**: all that open water may mean nobody searches it — demand unproven (see demand-validation ticket).

### 2. Contract Cockpit — plain-English lease/agreement reader

| Keyword | Top-10 evidence |
|---|---|
| "lease analyzer" | Intent-relevant incumbents: SafeSign 0, Ratifi 6, Auto LeaseLens 3, Lease Decoder 1 ratings. The rest is lease-to-own brands (Katapult, Progressive, Snap) — different intent. |
| "contract reader" | Versed 0, ClauseIt 0, ContractIQ 0, AI Contract Analyzer 53. Brands present (Adobe Acrobat 650K, Signeasy 34K) are all *PDF-tool* intent, not contract comprehension. |
| Play "contract reader plain english" / "lease analyzer rental" | Scatter of tiny indies (contractcheckai, thecontractact, legaladvisor) and rental-management tools. Nothing with traction. |

**Read**: blue ocean on both phrasings — big brands only on adjacent intent. Rare-cadence signing naturally meters LLM cost and fits premium. **Caveat**: incumbents' zero ratings could equally mean thin search volume; positioning must dodge "legal advice".

### 3. Pocket Archaeologist — thrift/vintage ID + value

| Keyword | Top-10 evidence |
|---|---|
| "thrift store appraiser" | All indies, but a heating cluster: ThriftAI 20K, Curio 15K, Antique Identifier Zophi 10K, Relic 6.9K, Gemli 4.1K, Appraiser.AI 468 ratings. No big studios — **passes the filter**. Play: Gemli 100K+, WhatsitAI 50K+ downloads. |
| "identify vintage" | AntiqSnap 31K (Next Vision — big-ish), ThriftAI 20K, Curio 15K + a tail of 0–1.4K indies. |
| "is this worth anything" | 6 results, all tiny (How Much Is It Worth 228; Flipsight 0). Phrasing wide open. |

**Read**: the only survivor with **proven demand** — the cluster's traction (ThriftAI 20K ratings, Gemli 100K+ Play downloads) proves people search this. Trade-off: it's a crowded indie niche now, not blue ocean. Differentiation must win the value-verdict phrasing, not the ID phrasing.

### 4. Sim Sim — haggling assistant

| Keyword | Top-10 evidence |
|---|---|
| "marketplace price check" | Sharky — OfferUp 4.4M, ADESA 3.2K (brand), Swappa 2.2K (brand), PriceCharting 26K. Indies exist (Value AI 91, Price Checker 15) but drowned. |
| "haggle helper" (Play) | HaggleBuddy: **10+ installs**. The negotiation phrasing is completely unserved. |
| "negotiate price assistant" (Play) | Price-alert tools, no negotiation app. iTunes "yard sale appraiser": Treasure Map 36K + the thrift cluster (see above). |

**Read**: survives on genuinely novel haggle phrasing — zero incumbents. Demand unproven, and the price-check side of the value prop lives in shark water; the app must be found via the haggle/negotiate phrasing.

### 5. Laundry Sorter — care-tag decoder (weak survivor)

| Keyword | Top-10 evidence |
|---|---|
| "laundry symbols" | Laundry Lens **278 ratings, 4.79** leads; AI Scanner 16, Laundry Day 60, rest 0–1. Payment apps (CSC GO 171K) pollute but are wrong intent. |
| "laundry tag" | Stain Snap 1 rating; payment/utility brands dominate — wrong intent. |

**Read**: passes the filter (decode-intent incumbents are all tiny indies) — the predicted shark-food turned out to be merely **weak**: Laundry Lens already does photo-decode and owns the position with modest traction. Differentiation must be plain-slang advice + fabric guidance, and it's thin. Included as #5 for completeness; reasonable to drop at choice time.

---

## Cuts (10), with evidence

| Idea | Killing keyword evidence |
|---|---|
| **Receipt Lens** | "receipt scanner": Fetch 7.6M, Ibotta 1.96M, Genius Scan 1.36M, Receipt Hog 268K — 4 big studios. "receipt organizer": SimplyWise 37K + QuickBooks 264K adjacent. Personal-hoarding phrasing doesn't rescue the space. |
| **Menu Mind** | "menu translator": Google Translate 84K, Translate Now 361K, iTranslate 529K, Google Photos 1.5M — 4 big brands. Survival only via "menu scanner allergy", already contested by OneLabel 3.5K and Fig 16K. |
| **Plant Doctor Snap** | "plant doctor": PictureThis 1.1M, Planta 114K, Plantum 119K, Plant Parent 91K, Blossom 69K — 5 big/funded. "plant identifier": same walls. |
| **Pantry Oracle** | "cook with what i have": NYT 545K, Tasty 433K, SuperCook 21.7K, ATK 17K — 3+ brands. "recipe from fridge": zombie 0-rating apps + NYT. |
| **Noise Detective** | No clean keyword maps to the intent: "sound identifier" → Shazam 8.8M / Merlin 111K; "decibel meter" → commodity (Decibel X 162K et al); "what is that noise" → white-noise sleep apps (TMSOFT 275K). ASO-led distribution has no entry point. |
| **Trip Twitch** | "travel itinerary": Tripadvisor 480K, TripIt 309K, Wanderlog 35K, Amadeus. "spontaneous travel" surfaces no spontaneous-planning incumbent — but integration weight + sharky adjacency kills it. |
| **Form Whisperer** | "form filler helper" → airSlate 32K / pdfFiller doc-tool brands (wrong intent). "visa form helper" → Atlys 3.4K, iVisa 11K funded. No keyword serves the how-to-fill intent. |
| **Wi-Fi Whisperer** (control) | "wifi analyzer": Ubiquiti 40K, Fing 116K, Ookla 28K — 3 big. "wifi doctor": eero 201K, NETGEAR 706K, Cox 132K. Confirmed shark-food, as predicted. |
| **Voice Note Alchemist** | "voice memo organizer": technically passes the letter (only Apple 1.08M is big; recorders are 1–13K indies) — but the *category* is pressed by Otter 78K, Speechify 522K, Wispr Flow 15K on the transcribe phrasing plus free OS-level transcription. Fails the spirit: the differentiator (organize/search) is a feature those players can add. |
| **Gig Grammar** | "gig earnings tracker": Gridwise 28K, Stripe Express 30K, Solo 13K, Mystro 9.9K, Para 7K — funded cluster. "doordash tracker": Stride 96K, MileIQ 112K, Everlance 52K mileage/tax brands. |

---

## The real tension for the next ticket

- **Validated-but-crowded vs blue-but-unproven.** Pocket Archaeologist is the only survivor whose keyword space demonstrably has searchers; the blue-ocean survivors (Shelf Whisperer, Contract Cockpit, Sim Sim) have zero-rating incumbents, which cuts both ways — no sharks, but possibly no demand either.
- This is exactly what the new **demand-validation research ticket** adjudicates: Apple Search Ads popularity per surviving keyword set, before the choice grills.

## Notes for the next tickets

- For **Choose the app idea**: rank order above is the filter's output, not the choice — the choice must weigh demand evidence (ticket to come) against build cost and LLM-cost profiles.
- LLM-cost patterns carried forward: Shelf Whisperer needs hard per-scan caps (vision + reasoning per query); Contract Cockpit's rare cadence is a natural premium fit and may need no backend at MVP; Pocket Archaeologist can lean on deterministic comps (eBay sold data) with vision-ID.
- Keyword-strategy seeds: primary phrasings that survived are *natural-language queries* ("should i buy", "is this worth anything", "lease analyzer") — long-tail ASO, not category labels.
