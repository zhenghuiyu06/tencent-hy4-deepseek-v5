# Tencent HY4 & DeepSeek V5 — China AI News (Nico material pack)

Public clone:

```text
https://github.com/zhenghuiyu06/tencent-hy4-deepseek-v5
```

Original-quality demo / launch clips + locked VO + asset index for the episode covering
**Tencent Hunyuan HY4** and **DeepSeek V5**. Media under `raw/China_AI_News/` is
**byte-identical to the gather originals** — no re-encode, no recompress for this upload.

## What is in this repo

| Path | Contents |
|------|----------|
| `raw/China_AI_News/**/*.mp4` | **Original HQ MP4s** (Git LFS). ~279 MiB across 22 clips. Largest ~55 MiB. |
| `VO_LOCKED.md` | Locked VO for the episode |
| `DYNAMIC_INDEX.md` / `asset_manifest.md` | Dynamic clip index + asset manifest |
| `RIGHTS.md` / `SHORTLIST.md` / `GAPS.md` | Rights notes, shortlist, known gaps |
| `AUDIENCE_MATCH_BRIEF.md` / `TITLE.md` / `LOCK.md` / `SEED_URLS.md` | Briefing + lock + seeds |
| `EPISODE_README.md` | Original episode workspace README |
| `stills/` / `stills_capture/` | Stills + capture notes |
| `sources/` | Saved HTML / cards / rights research |
| `MANIFEST.sha256` | SHA-256 of every `raw/**/*.mp4` and key docs |
| `CLAUDE.md` | **Mandatory** quality rules for Claude Code / editors |

Not included (on purpose): Claude handoff `tar.gz` / zip packs under `packs_claude*`,
oversized split recompressions, and any proxy/preview encodes. Prefer `raw/` only.

## Claude Code — how to use this repo

1. **Clone with Git LFS** (required for real video bytes):

   ```bash
   git lfs install
   git clone https://github.com/zhenghuiyu06/tencent-hy4-deepseek-v5.git
   cd tencent-hy4-deepseek-v5
   git lfs pull   # if objects were not fetched during clone
   ```

2. **Never use LFS pointer files as video.** A pointer is a tiny text file starting with
   `version https://git-lfs.github.com/spec/v1`. Real MP4s are multi-MB binaries. If
   `find raw -name '*.mp4' -printf '%s\n' | sort -n | head` shows ~130 bytes, run `git lfs pull`.

3. **Verify integrity** against the committed manifest:

   ```bash
   sha256sum -c MANIFEST.sha256
   ```

4. **Obey the quality protection rules** (also in `CLAUDE.md`):

   1. 从 Git LFS 获取完整原始 MP4，不得使用指针文件代替视频。
   2. 下载后验证文件完整性。
   3. 保留原视频分辨率、帧率和尽可能高的画质。
   4. 可无损剪切的片段优先使用 stream copy。
   5. 必须重新编码时，优先使用高质量编码参数。
   6. 禁止不必要的降分辨率、虚假升帧和过度压缩。
   7. 导出后使用 FFprobe 对比原始素材与成片的参数。
   8. 禁止使用低清预览版本代替原始素材。

## Direct media tip

After a successful `git lfs pull`, open files under **`raw/China_AI_News/`**. Do not dig in
pack zips or preview folders for “lighter” substitutes.

## Local staging note

This tree was prepared as a GitHub-ready stage: originals hardlinked from the episode
workspace, LFS attributes set, manifest written. Push requires a public empty repo at the
URL above and a working GitHub credential on the pushing machine.
