<div align="center">

<img src="https://raw.githubusercontent.com/GestaltBI/gestaltbi-core/master/src/assets/images/gestaltbi-logo.png" alt="GestaltBI" width="120" />

# GestaltBI

**la forma all'origine del significato**
*the shape at the origin of meaning*

Performance Intelligence for the people who actually have to read their numbers — owners, general managers, family-business operators. Drop a CSV, get the analyses that matter, decide better.

[**Live demo**](https://gestaltbi.github.io/gestaltbi-core/) · [Sample config](https://gestaltbi.github.io/gestaltbi-core/gh/GestaltBI/sample-config) · [`@gestaltbi/stream`](https://www.npmjs.com/package/@gestaltbi/stream)

</div>

---

## What it is

GestaltBI surfaces the story your numbers are telling. Longitudinal comparisons, synchronic comparisons across customers / products / territories, and change-force decomposition (what's driving the move — volumes, prices, costs, or some combination) — across maps, charts, and tables.

The methodology comes from a tradition of management accounting that puts **gross margin** at the apex of the analysis pyramid: the only synthetic indicator with the right cadence (updated by every transaction), objectivity (matching principle, no allocation guesswork), and operational utility for daily learning. Profitability ratios like ROI, RONA, and ROE are too slow; budget deviations are too unrealistic over horizons that matter.

The interface is opinionated about which cuts to show first — to avoid the analysis-paralysis that generic BI tools breed — and gets out of the way once you know what you're looking at.

## What's here

| Repo | What it is |
|---|---|
| [`gestaltbi-core`](https://github.com/GestaltBI/gestaltbi-core) | The Angular 21 client. MapLibre 5, ECharts 6, ag-Grid 33, Material 21 (M3). Deploys to GitHub Pages. |
| [`sample-config`](https://github.com/GestaltBI/sample-config) | A worked example of the six config files (`data.csv`, `structure.json`, `processing.json`, `modes.json`, `mapping.json`, `it.json`) that drive a GestaltBI instance. |
| [`stream`](https://github.com/GestaltBI/stream) | Framework-agnostic streaming pipeline — RxJS + JSON-defined process graphs of named ops. Published as [`@gestaltbi/stream`](https://www.npmjs.com/package/@gestaltbi/stream). |
| [`olap-cube-js`](https://github.com/GestaltBI/olap-cube-js), [`pandas-js`](https://github.com/GestaltBI/pandas-js), [`parquetjs`](https://github.com/GestaltBI/parquetjs) | Maintained forks of upstream-abandoned data libraries we depend on. |

## The `/gh/<org>/<repo>` route

`gestaltbi-core` ships with a feature that turns any GitHub repo into a live GestaltBI instance — no rebuild, no deploy. Visit:

```
https://gestaltbi.github.io/gestaltbi-core/gh/<your-org>/<your-repo>
```

…and the client fetches your six config files via jsDelivr and renders a fully-configured visualization stack against them. Pin a commit SHA in the URL (`/gh/<org>/<repo>/<sha>`) for reproducible demos.

To author your own: fork [`sample-config`](https://github.com/GestaltBI/sample-config), swap `data.csv`, adjust `structure.json` tags so the right columns flow through the right ops, push, share the link.

## License

MIT, except where individual fork READMEs state otherwise.

---

<div align="center">

*la forma all'origine del significato*

</div>
