# GPT-6 Astra — Blog Article

Long-form article on OpenAI's GPT-6 Astra release (September 3, 2026) and what it means for the autonomous-AI question, with supporting charts, diagrams, evidence cards and a full source list.

## Contents

| Path | What it is |
|---|---|
| `GPT-6-ASTRA-ARTICLE/article/gpt6-astra-final.md` | The article, Markdown source of truth |
| `GPT-6-ASTRA-ARTICLE/article/gpt6-astra-final.html` | Styled, self-contained web version (embeds the charts and diagrams) |
| `GPT-6-ASTRA-ARTICLE/article/gpt6-astra-final.docx` | ⚠️ **Stale — see below** |
| `GPT-6-ASTRA-ARTICLE/charts/` | Four HTML charts (benchmark comparisons, competitive landscape) |
| `GPT-6-ASTRA-ARTICLE/diagrams/` | Four SVG diagrams (agent workflow, autonomy scorecard, evolution, capability model) |
| `GPT-6-ASTRA-ARTICLE/evidence/` | Evidence cards documenting quoted public statements |
| `GPT-6-ASTRA-ARTICLE/data/benchmark-data.csv` | All benchmark figures with sources and caveats |
| `GPT-6-ASTRA-ARTICLE/sources/sources.md` | Full source list, corrections log, and outstanding items |

## Viewing it

The HTML article references sibling folders, so serve from the article root rather than opening the file directly:

```bash
cd GPT-6-ASTRA-ARTICLE
python -m http.server 8137
# then open http://127.0.0.1:8137/article/gpt6-astra-final.html
```

## ⚠️ Known issue: the .docx is out of date

`gpt6-astra-final.docx` predates a fact-checking pass and **still contains incorrect benchmark figures** — including fabricated competitor scores for ARC-AGI-3, OSWorld 2.0, FrontierMath and ScreenSpot-Pro. It has not been regenerated.

**Use the `.md` or `.html` version.** The `.docx` should be re-exported from one of those before it is distributed anywhere.

## A note on the benchmark data

Unless explicitly labelled otherwise, all competitor comparison scores (GPT-5.6 Sol, Claude Fable 5.1, Claude Opus 5, Gemini 3.8 Flash) are **OpenAI's own published figures** from its launch materials — a vendor scoring itself against its competitors on evaluations it selected and ran. Only the ARC Prize Foundation and Artificial Analysis figures represent independent third-party measurement.

Where sources disagree on the same benchmark (notably Terminal-Bench 4.0, where the reported Astra/Fable gap ranges from +0.3 to +7.1 depending on the harness), the article shows the range rather than picking one number.

A full corrections log is at the bottom of [`sources/sources.md`](GPT-6-ASTRA-ARTICLE/sources/sources.md).
