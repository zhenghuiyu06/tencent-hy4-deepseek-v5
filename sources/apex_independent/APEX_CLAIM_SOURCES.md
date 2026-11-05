# Apex Agents 75.2 — claim sources (BENCHMARK_NOT_VERIFIED kept)

Gather 2026-11-05 Asia/Taipei. Independent Artificial Analysis APEX-Agents-AA board does **not** list Hy4 at 75.2.

## Verdict
Keep **BENCHMARK_NOT_VERIFIED**. VO may say 75.2; on-screen must say “Tencent-reported” / “not independently verified.”

## Independent boards checked
| Source | URL | Hy4 75.2? | Local |
|--------|-----|-----------|-------|
| Artificial Analysis APEX-Agents-AA | https://artificialanalysis.ai/evaluations/apex-agents-aa | **No** — AA independent implementation; headline models are Gemini/Qwen/Kimi class, not Hy4 75.2 | `artificialanalysis_apex_agents_aa.html` + `artificialanalysis_apex_og.png` → also `China_AI_News/04_HY4_Benchmarks/S04_apex_AA_independent_board_og_01.png` |
| BenchLM APEX-Agents catalog | https://benchlm.ai/benchmarks/apexagents | Lists Hy4 75.2% **but** BenchLM note: stores provider-run values; excluded from weighted score; **not** AA independent run | `benchlm_apexagents.html` — treat as redistributor of provider/Tencent figures |

## Better claim / critique sources (still not independent verification)
| Source | URL | Note | Local |
|--------|-----|------|-------|
| A2Agent — What the Charts Actually Show | https://a2agent.me/blog/tencent-hy4-benchmarks | Transcribes Tencent appendix; APEX preview 53.9 → 75.2; footnotes on * own testing | `a2agent_hy4_benchmarks.html` |
| FourWeekMBA | https://fourweekmba.com/ai-tencent-hy4-edges-opus-on-own-agent-test-at-1-8-output-price/ | Explicit: “Tencent’s scores have not been independently verified.” | `fourweekmba_hy4.html` |
| Official research appendix stills | https://hy.tencent.ai/research/hy4 | Tencent-reported tables already in `04_HY4_Benchmarks/S04_hy_tencent_ai_research_hy4_bench_table*.png` | HQ stills |
| Community redistributes | kimmonismus / CodeByNZ / aloo / AiBattle X posts | Already in manifest as PARTIAL | China_AI_News/04 |

## Edit rule
Prefer official appendix table + A2Agent/FourWeekMBA “Tencent-reported” framing. Do **not** cut AA board as if it proves 75.2.
