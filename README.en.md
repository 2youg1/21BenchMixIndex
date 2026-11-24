# 21BenchMixIndex

**Coding Model Mixture Index** — a reproducible, modifiable decision tool that compresses public data from AA Coding Agent, AA Intelligence, VALS, CursorBench, FrontierSWE and ProgramBench into a single coding-model index.

This is an index, not a leaderboard.

[中文](README.md)

## Current index (data version 26/11/20)

![Live mixture index · main board (data version 26/11/20)](docs/screenshot.png)

[View the distribution explorer](docs/distribution.png)

> Rendered locally; open the HTML to interact (filtering, normalisation, imputation policy, per-metric editing, CSV export).

## Open it

- Open `21BenchMixIndex261120.html` directly: single file, zero external dependencies, fonts from the local font stack (system sans by default, with Sarasa Mono available).
- GitHub Pages: set the repo root as the Pages source; `index.html` redirects to the entry page named by data version.
- Data version: see `meta[name="release-date"]` in the HTML (YY/MM/DD). When updating data, change only this value, rename the entry file to match, and update the `index.html` redirect target plus the README screenshot.

## What's inside

- Bilingual UI: one-click `EN / 中` toggle in the header; the choice persists locally.
- Search by model name and filter by lab. The filter rail collapses and starts closed on phones. The chart and metric table share filters and sorting. Select a value to edit its percentage or a model to inspect its score.
- Compare any two models in the selection across MIX and all eight inputs. Estimates carry ≈ and missing or fallback values display a dash.
- Sliders and numeric inputs adjust the original six BASE weights and two multiplier coefficients. A missing CB reallocates its weight to FC, TB and FSWE in a 2:1:1 ratio. The browser remembers custom weights, edits, models and an optional scenario date. CSV exports include the calculation settings.
- The benchmark guide explains the tasks, evaluation method, access and scoring role for each source. Select a metric header to open its guide entry.
- The main board shows only models with **≤2 missing** of the 8 raw inputs; switch to "All" for the reference pool.
- Missing data: a missing CB triggers the formula fallback; missing PB / VCB100 / FSWE follow "Recommended / Floor / Zero" imputation, and every value can be hand-edited in the drawer.
- Normalisation: `Fable 5.2 = 1` / `Max = 1` / `Raw`.
- AA cross-check: same-anchor scale and gap against **AA Intelligence Index v5.0.1**.
- Actual distribution: explore MIX or Δ AA for all candidates or the current board selection. Select a histogram interval to inspect its members alongside five quantile statistics.
- Light & dark themes; cobalt MIX bars, vermilion AA markers and lab colours next to model names; chart style switcher (bars / lollipop / tick).
- Display options: pick a font from the local font stack (Chromium can also detect installed fonts), and drag sliders for text size (90%–160%) and weight (−200 to +300); choices persist locally.
- CSV export, add custom models, fit details, copy citation.

## Data sources

- [AA Coding Agent Index v2.1](https://artificialanalysis.ai/agents/coding-agents)
- [AA Intelligence Index v5.0.1](https://artificialanalysis.ai/leaderboards/models)
- [VALS VCB 1-100 v1.1](https://www.vals.ai/benchmarks/vcb-1-100-v1-1)
- [VALS Vibe Code Bench v1.1](https://www.vals.ai/benchmarks/vibe-code)
- [VALS ProgramBench](https://www.vals.ai/benchmarks/programbench)
- [CursorBench 4.1](https://cursor.com/cursorbench)
- [FrontierSWE v2](https://www.frontierswe.com/)
- [Terminal-Bench 4.1](https://www.tbench.ai/)

Underlying benchmark data and trademarks belong to their respective publishers; this repo only aggregates and visualises.

## License

This work is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). Attribution, non-commercial, share alike. For commercial licensing, contact the author.

## Feedback

- GitHub Issue / PR
- Bilibili: <https://space.bilibili.com/334394212>
- GitHub: <https://github.com/2youg1>

Renders well in the author's LibreWolf; 100% compatibility across every configuration is not guaranteed.
