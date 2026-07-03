# Overleaf (free tier)

GitHub import is **Overleaf Premium**. Use one of these free paths instead.

## Option A — Upload zip (fastest)

1. [Overleaf](https://www.overleaf.com) → **New Project** → **Upload Project**
2. Upload [`HW-Triage-Bench-Paper-overleaf.zip`](HW-Triage-Bench-Paper-overleaf.zip)
3. Rename project to **`HW-Triage-Bench-Paper`**
4. Menu → Settings → Compiler: **pdfLaTeX** → Recompile

## Option B — Blank project + agent upload

1. **New Project** → **Blank Project** → name **`HW-Triage-Bench-Paper`**
2. Tell the Cursor agent: *"Overleaf project created"*
3. Agent pushes `main.tex` and `references.bib` via Overleaf MCP and compiles

## Option C — Copy files manually

1. **New Project** → **Blank Project**
2. Delete default `main.tex` content; paste from [`latex/main.tex`](latex/main.tex)
3. **New file** → `references.bib` → paste from [`latex/references.bib`](latex/references.bib)
4. Recompile (pdfLaTeX)

## Not recommended for this paper

| Import type | Why skip |
|-------------|----------|
| **GitHub sync** | Premium only |
| **Markdown / Word** | Loses IEEE LaTeX structure, citations, and conference formatting |

Canonical git source: [github.com/piyushbag/open-test-triage/tree/main/paper/latex](https://github.com/piyushbag/open-test-triage/tree/main/paper/latex)

## Author block (public)

```
Piyush Jagadish Bag
Test Automation Engineer, Platform Hardware
piyushbag4@gmail.com
```

No employer name in the paper author block.
