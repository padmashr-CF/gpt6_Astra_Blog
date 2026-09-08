# GPT-6 Astra — Blog Article

**📖 Read it here: https://padmashr-CF.github.io/gpt6_Astra_Blog/**

Long-form article on OpenAI's GPT-6 Astra release (September 3, 2026) and what it means for the autonomous-AI question, with supporting charts, diagrams, evidence cards and a full source list.

## Contents

| Path | What it is |
|---|---|
| `GPT-6-ASTRA-ARTICLE/article/gpt6-astra-final.md` | The article, Markdown source of truth |
| `index.html` | The published GitHub Pages entry point — generated from the article HTML with asset paths rewritten for the site root |
| `GPT-6-ASTRA-ARTICLE/article/gpt6-astra-final.html` | Styled web version, source of truth for `index.html` |
| `GPT-6-ASTRA-ARTICLE/article/gpt6-astra-final.docx` | ⚠️ **Stale — see below** |
| `GPT-6-ASTRA-ARTICLE/charts/` | Four HTML charts (benchmark comparisons, competitive landscape) |
| `GPT-6-ASTRA-ARTICLE/diagrams/` | Four SVG diagrams (agent workflow, autonomy scorecard, evolution, capability model) |
| `GPT-6-ASTRA-ARTICLE/evidence/` | Evidence cards documenting quoted public statements |
| `GPT-6-ASTRA-ARTICLE/data/benchmark-data.csv` | All benchmark figures with sources and caveats |
| `GPT-6-ASTRA-ARTICLE/sources/sources.md` | Full source list, corrections log, and outstanding items |

## Viewing it locally

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

## Republishing after an edit

`index.html` at the repo root is generated, not hand-edited. After changing
`GPT-6-ASTRA-ARTICLE/article/gpt6-astra-final.html`, regenerate it:

```bash
python - <<'EOF'
import io
s = io.open('GPT-6-ASTRA-ARTICLE/article/gpt6-astra-final.html', encoding='utf-8').read()
for d in ['charts', 'diagrams', 'images']:
    s = s.replace('../%s/' % d, 'GPT-6-ASTRA-ARTICLE/%s/' % d)
s = s.replace('href="../sources/sources.md"',
              'href="https://github.com/padmashr-CF/gpt6_Astra_Blog/blob/main/GPT-6-ASTRA-ARTICLE/sources/sources.md"')
io.open('index.html', 'w', encoding='utf-8', newline='').write(s)
EOF
```

Then commit and push — GitHub Pages redeploys automatically.
