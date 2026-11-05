# GAPS.md — Tencent HY4 & DeepSeek V5

Honest gaps after gather-only pass (2026-11-05 Asia/Taipei). No other episode started.

## Critical flags (must surface in edit)

### PRICE_VO_CONFLICT
- Locked VO says roughly **«83»** input + **$2.50** output framing (keep Tensson/Hue slips verbatim).
- BenchLeader verified: **$0.834 / $2.50** per 1M tokens (`sources/` + `S06_pricing_benchleader_og_01.png`).
- Tencent press paraphrases ~**$0.90 / $2.70** (secondary).
- **Edit rule:** keep VO audio as locked; on-screen card should prefer BenchLeader VERIFIED numbers and/or burn-in a small “sources differ” note. Do not silently “fix” VO.

### BENCHMARK_NOT_VERIFIED
- VO Apex Agents **75.2** appears only as **Tencent-reported / redistributed** claim (kimmonismus, CodeByNZ, FourWeekMBA, A2Agent — see EN cards).
- **No independent original Apex Agents leaderboard chart** captured this run.
- Assets under `04_HY4_Benchmarks/` are PARTIAL claim stills + **silent** aloo montage — label on-screen “Tencent-reported” / do not present as third-party verified.

### V5 = reported plan only
- DIGITIMES + TechNode: DeepSeek **reportedly plans** V5 training on Huawei Ascend (950 / Ascend family); not a shipped V5 model.
- No official DeepSeek V5 weights, blog “we ship V5”, or product page found.
- All S15–S16–S18–S21 V5 B-roll must stay **plan / report** tone. Do not invent release UI.

### GAME_DEMO_NOT_VERIFIED
- Secondary sites (hy4.online EN card) claim Unreal/Unity/Godot / “zombie” MCP-style demos.
- **No verified downloadable HY4 gameplay** (zombie Unreal MCP) located from official `@TencentHunyuan` or hy.tencent.ai.
- Unrelated Claude/Unreal MCP YouTube hits **rejected**.
- For S11–S13: use capability claim stills + official productivity reel game/finance beats only; do not fake a game demo.

## Seed / HQ gaps (computerUse wishlist for parent)

| Priority | Need | Why |
|----------|------|-----|
| **P0** | Full-page HQ screenshot + scroll capture of `https://hy.tencent.ai/` and `https://hy.tencent.ai/research/hy4` | curl/WebFetch only got SPA shell (~7KB). Need official product/research UI stills for Opening + Ending. |
| **P0** | Reuters article full text + key graphic: `…tencent-rolls-out-ai-model-trained-with-limited-cybersecurity-data…2026-11-04` | Captcha/JS wall; Wayback empty. Needed for S08–S10 VERIFIED wire pixels. |
| **P1** | Live hy.tencent.ai “Try HY4” / playground session screen (no self-fabricated UI) | Portal motion currently only NousResearch third-party. |
| **P1** | Independent Apex Agents / LMSYS / Artificial Analysis chart that actually lists HY4 at 75.2 (if exists) | Else keep BENCHMARK_NOT_VERIFIED forever. |
| **P1** | Official DeepSeek statement on V5 / Ascend (blog, X @deepseek_ai, CN press) | Currently DIGITIMES/TechNode “reportedly”. |
| **P2** | Verified HY4 Unreal/Unity gameplay downloadable asset or official Hunyuan gamedev reel tagged HY4 | Clears GAME_DEMO_NOT_VERIFIED. |
| **P2** | Hugging Face / ModelScope weights page when published | VO S07 “weights planned” — still pending per community stills. |
| **P3** | Full DIGITIMES body beyond OG/headline (paywall) | Headline confirmed; deep quotes optional. |

## Folder-level thin spots

| Folder | Status |
|--------|--------|
| `01_Opening` | Thin — TechNode dual-story still only; needs hy HQ computerUse |
| `02_HY4_Launch` | Strong (official + YT) |
| `03_HY4_Capabilities` | Strong (official 4 Real + computer-use) |
| `04_HY4_Benchmarks` | Weak verification (claims only) |
| `05_HY4_Pricing` | Pricing OG + weights pending stills |
| `06_HY4_Safety` | YT + X relays; missing Reuters original |
| `07_HY4_Game_Demo` | **Gap** — claim stills only; no verified demo |
| `08_Transition` | OK bridge YT |
| `09_DeepSeek_V5` | OK for plan-only; no product |
| `10_DeepInfer` | Strong (X + YT + GH archive) |
| `11_Ending` | Thin — needs HQ + DIGITIMES reprise |

## Top P0 GAPS (report-back)

1. hy.tencent.ai + /research/hy4 full HQ screenshots (computerUse).
2. Reuters 2026-11-04 cyber article original capture (computerUse).
3. Independent Apex 75.2 chart — or permanently keep BENCHMARK_NOT_VERIFIED.
4. Verified HY4 game demo — or keep GAME_DEMO_NOT_VERIFIED and cut S11–S13 to claim cards + official productivity.

## HQ stills merge (computerUse 2026-11-05)
Parent captured read-only PNGs — closes several P0 seed gaps:
- `02_HY4_Launch/S02_hy_tencent_ai_hero.png` + preview CTA + `research/hy4` intro (HTTP 200, not SPA stub)
- `04_HY4_Benchmarks/S04_hy_tencent_ai_research_hy4_bench_table*.png` — official appendix tables
- `04_HY4_Benchmarks/S04_benchleader_hy4_table*.png` — BenchLeader tables
- `05_HY4_Pricing/S06_benchleader_hy4_pricing_overview.png` + `S06_benchleader_hy4_api_pricing.png`
- `06_HY4_Safety/S08_reuters_cyber_*.png` — Reuters 2026-11-04 cyber paragraphs (loaded after brief 401; no captcha)
See `stills_capture/CAPTURE_NOTES.md`.

**Still open:** BENCHMARK_NOT_VERIFIED for independent Apex 75.2; GAME_DEMO_NOT_VERIFIED; PRICE_VO_CONFLICT (VO «83» vs BenchLeader $0.834 — pricing stills now support on-screen correction card).


## 总指挥 HQ coexist (2026-11-05)
`*HQ*.png` from 总指挥 kept alongside our stills_capture set. Reuters: 总指挥 notes paywall body; our run captured paragraph PNGs — use those for S08–S10; keep title HQ as backup.

## Gap-fill pass 2026-11-05 (executor)

### Closed / strengthened
1. **Apex 75.2** — Independent AA APEX-Agents-AA checked: **Hy4 not listed**. BenchLM lists 75.2 as provider-run catalog (excluded from weighted score). Claim-critique pack archived under `sources/apex_independent/` (`APEX_CLAIM_SOURCES.md`). Flag remains **BENCHMARK_NOT_VERIFIED**.
2. **Game demo** — Harder X+YT search; no official @TencentHunyuan Unreal/zombie MCP downloadable. Rejected list → `sources/game_demo_rejected/REJECTED_LIST.md`. Flag remains **GAME_DEMO_NOT_VERIFIED**.
3. **HQ dedupe** — Scanned `China_AI_News/**HQ*` + computerUse stills. Only true duplicate hash: `S01_hy_tencent_ai_landing_HQ_01.png` ≡ `S21_hy_tencent_ai_landing_HQ_01.png` (same landing reused Opening/Ending — keep both paths, one physical twin OK). 总指挥 HQ + our CU set coexist with distinct hashes (no row merge needed beyond existing Append). Manifest already lists both sets without duplicate rows for distinct pixels.
4. **Reuters mirrors** — Public mirrors archived: Rappler (full body HTML + OG still `S08_reuters_mirror_rappler_og_01.jpg`), CNA, Deccan Chronicle. StreetInsider 403. Prefer existing CU `S08_reuters_cyber_paragraphs*.png` for body; mirrors backup if paywall returns.

### Still open
- Independent Apex chart proving 75.2 — **MISSING** (keep flag)
- Verified HY4 Unreal/zombie MCP gameplay — **MISSING** (keep flag)
- PRICE_VO_CONFLICT — unchanged (VO «83» vs $0.834)
- V5 = plan only — unchanged
- DIGITIMES full body beyond OG — still paywall
