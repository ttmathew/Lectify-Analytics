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
| `admin-console.png` | README, features.md | The admin console: user/role management view |
| `audit-log.png` | features.md | The audit log viewer showing logged questions/answers/verification outcomes |
| `cost-observability.png` | README, features.md | Cost tracking dashboard: spend trend, breakdown by feature/department/user, flagged outliers |
| `agent-efficiency.png` | README, features.md | Agentic efficiency dashboard: tool-call trace with a flagged redundant call, call volume by tool |
| `rag-quality.png` | README, features.md | RAG quality dashboard: grounding rate trend, retrieval issues by category, flagged retrievals |
| `guardrails-safety.png` | README, features.md | Guardrails dashboard: triggers by category (scope/PII/injection/toxicity), trend, flagged events |

If your real capture is a GIF instead, name it `<filename>.gif` and update the one matching link in the README/features.md to the `.gif` extension.
