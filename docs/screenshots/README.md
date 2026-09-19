# Screenshot Shot List

The `.png` files in this folder are **illustrative mockups** (labeled as such in the corner of each image) standing in for the real product UI, referenced from the [README](../../README.md) and [feature walkthrough](../features.md). They're placeholders — not a claim about the actual interface, except `business-workspace.png`, which is a real captured design screen (see below).

Each mockup — apart from `business-workspace.png` — also has a matching `.svg` source file (same base name) — that's the editable version if you want to tweak one; the `.png` is the rendered file actually linked from the docs. All mockups share one visual language: warm cream background (`#F3F2F2`), **Cormorant Garamond** (serif) for headings and large figures, **Lora** (serif) for body text, and a gold/amber accent (`#B68235`) with small (3–4px) corner radii throughout. Keep new mockups consistent with this palette.

`business-workspace.png` is a screenshot of an actual designed screen (captured from a Claude Design canvas), not a hand-drawn `.svg` mockup like the rest — there's no source file to edit here; treat it as a real asset.

## Replacing a mockup with a real screenshot

Just overwrite the `.png` file with your real screenshot/GIF, using the **same filename**. The README and feature walkthrough already point at these exact paths, so no link changes are needed. Once you're happy with it, you can delete the matching `.svg` source (no longer needed).

| Filename | Used in | What to capture |
|---|---|---|
| `business-workspace.png` | README, features.md | The workspace overview screen: computed metrics, source-linked citations, Q&A, peer benchmarking, anomaly detection |
| `qa-chat.png` | README, features.md | The Q&A interface: a natural-language question and its verified, plain-language answer |
| `verification-status.png` | features.md | A verified figure and, ideally, one flagged as unverifiable — showing both states |
| `company-report.png` | README, features.md | An automated company report (performance, peer comparison, drivers of change) |
| `peer-comparison.png` | README, features.md | A peer comparison visualization, ideally mid-drill-down into a data point |
| `industry-benchmark.png` | README, features.md | An industry benchmark chart: a company plotted against its whole industry's range and percentile, distinct from a named peer comparison |
| `admin-console.png` | README, features.md | The admin console: user/role management view |
| `audit-log.png` | features.md | The audit log viewer showing logged questions/answers/verification outcomes |
| `cost-observability.png` | README, features.md | Cost tracking dashboard: spend trend, breakdown by feature/department/user, flagged outliers |
| `agent-efficiency.png` | README, features.md | Agentic efficiency dashboard: tool-call trace with a flagged redundant call, call volume by tool |
| `rag-quality.png` | README, features.md | RAG quality dashboard: grounding rate trend, retrieval issues by category, flagged retrievals |
| `guardrails-safety.png` | README, features.md | Guardrails dashboard: triggers by category (scope/PII/injection/toxicity), trend, flagged events |

If your real capture is a GIF instead, name it `<filename>.gif` and update the one matching link in the README/features.md to the `.gif` extension.

## Why these are `<img width="...">` tags, not `![]()`

Every file here is rendered at 2x the size it's actually displayed at (e.g. `qa-chat.png` is 1280px wide but shown at 640) — sharp on retina/high-DPI screens without looking oversized inline. This only works through an HTML `<img width="...">` tag; plain Markdown `![]()` has no way to constrain display size, so GitHub would show the full 1280px file inline. Keep this pattern for any new screenshot: render at 2x whatever width you intend to display it at, then set `width` to the *display* size, not the file's actual pixel size.

Note the tradeoff: clicking through to open the file directly still shows it at its full native resolution (2x), since that's controlled by GitHub's own image viewer, not by this markdown — that's expected, not a bug.
