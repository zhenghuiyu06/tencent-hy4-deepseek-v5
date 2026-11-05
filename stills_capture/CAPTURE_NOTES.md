# HY4 stills capture notes

Captured 5 Nov 2026 from the agent browser (read-only; no login; no playground prompts). The user's computer was offline, so these pages loaded on the agent box network, not through the user's machine.

Viewport screenshots are PNG, 1920×1113 (browser viewport). No cookie-consent banner was shown on any of the four URLs. Nothing was invented for a blocked page.

## URLs

| URL | Result |
| --- | --- |
| https://hy.tencent.ai/ | HTTP 200. Title "Tencent Hy". Hero plus research-feed HY4 preview card captured. |
| https://hy.tencent.ai/research/hy4 | HTTP 200. Live article "Introducing Hy4" dated November 4, 2026 (not a 404). Intro and appendix benchmark table captured. |
| https://www.benchleader.com/models/hy4 | HTTP 200. Title "Hy4 benchmarks & pricing: $0.83 in, $2.50 out per 1M". Pricing and benchmark tables captured. |
| Reuters HY4 cyber article (4 Nov 2026 litigation URL) | Page rendered the full article with no captcha widget and no sign-in wall. First `goto` reported HTTP 401 and an empty body before paint; the article then loaded (title includes the headline). Console later showed many ad/script errors. Headline and cyber-training paragraphs were captured from the rendered page. No article text is transcribed here. |

## Captcha / blocks

- No captcha, "verify you are human", or access-denied wall was visible on hy.tencent.ai, benchleader.com, or reuters.com.
- A suspected block was reported for reuters.com only because the first response was HTTP 401 with an empty document. The article UI then painted and was readable, so the URL was not abandoned.
- BenchLeader popped a newsletter modal ("KNOW THE DAY A NEW MODEL LANDS") over the lower page while scrolling to API pricing. It is not a cookie banner. It was closed with the dialog's Close control so the pricing table could be shot. The earlier overview and first benchmark shots were taken before that modal.

## Files

All paths are under `/workspace/tencent-hy4-deepseek-v5-ep/China_AI_News/`.

### hy.tencent.ai home

- `02_HY4_Launch/S02_hy_tencent_ai_hero.png` — Top of https://hy.tencent.ai/. Nav (Model, Research, Products, Gallery, Co-design, 中文站, Try Hy, Login). Hero mark "Hy". CTAs: "Try it now", "Learn More" (href `https://hy.tencent.ai/research/hy4`), and a watch-video control. Start of "More Research" below.
- `02_HY4_Launch/S02_hy_tencent_ai_hy4_preview_cta.png` — Same homepage, scrolled to the research list. Visible card: Release, "Introducing Hy4 preview", Aug 27, 2026, Hy LLM (href `/research/hy4-preview`), between the RL-batch research card and the ELR pretraining card.

### hy.tencent.ai/research/hy4 (HTTP 200)

- `02_HY4_Launch/S02_hy_tencent_ai_research_hy4_intro.png` — Article top. Date November 4, 2026. H1 "Introducing Hy4". Links: Tencent Cloud, OpenRouter, Hy AI Studio. Opening paragraphs on the Hy4 release versus Hy4 preview (vision, instruction following, long context, long-horizon, deep research). Left rail TOC. Top row of comparison charts partly in frame (labels include ProgressBench, Free-formCode 3.0+, 3DVerse-Modeling, Terminal-Bench 4.0, and others).
- `04_HY4_Benchmarks/S04_hy_tencent_ai_research_hy4_bench_table.png` — "Looking ahead" (notes a remaining gap and a planned Hy4 flash) plus the start of "Appendix: benchmark results". Table columns include Task, Benchmark, Hy4 preview, Hy4, GLM-5.0, DeepSeek-V4.1-Flash-1017, Kimi K2.1 Pro, GPT-5.1 Sol, Claude Opus 5.3. Rows begin at DeepSWE v1.1 through early agentic-coding / modelling rows.
- `04_HY4_Benchmarks/S04_hy_tencent_ai_research_hy4_bench_table_02.png` — Continuation of the same appendix table through Agentic Coding, Agentic Search, Working Agent, STEM, AI4Research, Computer Use, and Multimodal, then footnotes. Hy4 column is highlighted.

### benchleader.com/models/hy4

- `05_HY4_Pricing/S06_benchleader_hy4_pricing_overview.png` — Page header. HY4 by Tencent, chips "Open weights" and "Reasoning model". Quality 55.6 index (#96 of 329), Price $1.25 per 1M tokens (#147 of 246), Speed 46 tokens/s (#164 of 209). "As of 4 Nov 2026" summary (API $0.834 in / $2.50 out, blended $1.25 at 3:1; ~46 tok/s via OpenRouter; released 28 Aug 2026). Key facts, category bars (overall 56, coding 61, agents & tools 48, maths 66, knowledge 58), and stat row (blended price, output speed, first answer 3.02 s, context 1.0M, released 28 Aug 2026).
- `04_HY4_Benchmarks/S04_benchleader_hy4_table.png` — "How its index has moved" (27 Oct 2026 to 30 Oct 2026, flat line near 56) and "BENCHMARK RESULTS" Coding table (Arena WebDev, IOI, Code Migration, Code Migration v1.1, ProgramBench, Vibe Code Bench v1.1). A thin promo strip sits under the nav.
- `04_HY4_Benchmarks/S04_benchleader_hy4_table_agents.png` — Coding table again plus Agents & tools (Arena Agent, Terminal-Bench 2.1, CyberBench, Finance Agent, Harvey legal-agent benches, Legal Research Bench, SREBench, and the start of further rows).
- `04_HY4_Benchmarks/S04_benchleader_hy4_table_maths_knowledge.png` — Rest of Agents & tools (through Terminal-Bench Science), Maths (ProofBench 75.0%), and Knowledge (LegalBench, BioMysteryBench, Excel/Modeling, MedCode, MedStribe, and rows continuing below the fold).
- `05_HY4_Pricing/S06_benchleader_hy4_api_pricing.png` — "API PRICING: WHERE TO RUN IT" (Cohere, DeepInfra, AtlasCloud, SiliconFlow, NovitaAI, Tencent Cloud, GMICloud: speed, first token, input $/M $0.834, output $/M $2.50, context, quantization) and "WHAT A TASK COSTS" (chat reply, 30-page report, code edit, agentic coding session, structured extraction). Shot after the newsletter modal was closed.

### Reuters (rendered; no captcha)

- `06_HY4_Safety/S08_reuters_cyber_headline.png` — Headline "Tencent rolls out AI model trained with limited cybersecurity data amid hacking fears". Byline Nichiket Sunil and Eduardo Baptista. Dateline November 4, 2026, 4:34 AM CST, updated 13 hours ago (relative to capture). Tencent logo illustration and caption.
- `06_HY4_Safety/S08_reuters_cyber_paragraphs.png` — Lead and the cybersecurity-training paragraph (defensive uses only; excluded material on building hacking tools, breaking into systems, and testing systems for weaknesses), above a Daily Docket newsletter box. Page ads on the right.
- `06_HY4_Safety/S08_reuters_cyber_paragraphs_02.png` — Following paragraphs: internal security testing found no higher break-in / bypass risk and no meaningful help for harmful biological experiments; context on AI-powered hacking and a prior Tencent agent web-browsing disclosure. Interstitial ads.
- `06_HY4_Safety/S08_reuters_cyber_paragraphs_03.png` — Closing body: the browsing activity was not attributed to Hunyuan models; other Chinese labs tightening cyber-offensive limits; plan to release weights later with a safety-testing report; quoted commitment on cyber and biological risks. Then an ad.

## Not done / not failed

- No URL was left uncaptured.
- Research path `/research/hy4` exists (200); a 404 note is not needed.
- Cookie banners: none to dismiss.
- Did not sign in, subscribe, or type into any playground or alert form.
