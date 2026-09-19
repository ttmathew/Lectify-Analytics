# Roadmap

This roadmap describes where the project has been, where it is now, and where it's headed. It's organized by phase rather than by date, since scope and priority are still evolving with what we learn from early use.

## Current Phase — Core Q&A, Verification, and Reporting

The foundation of the system: the ability to ask a natural-language question about a public company's SEC Annual and Quarterly Reports and get back an answer that has been independently checked against source data before being shown.

- Natural-language question answering over SEC Annual and Quarterly Report data
- Independent verification of every numeric claim before it reaches the user
- Narrative grounding for qualitative "why" explanations
- Automated static company reports: performance over a period, peer comparison, industry comparison, insights from annual report narrative, and drivers of change
- Industry-wide benchmarking — comparing a company against the broader industry it belongs to, not just a named set of peers
- Audit logging of questions, answers, and verification outcomes

**Status: functional.**

## Near-Term Phase — Visualization, Access Control, and Trust Layer

Building out the surrounding experience and the controls needed to move from a working core to something usable by more than one person at a time.

- Interactive data visualizations with drill-down into the underlying data points behind a chart
- Role-based authentication and an admin console for user and access management
- A guardrails and observability layer for ongoing safety and quality monitoring

**Status: functional, actively being refined.**

## Next Phase — Cloud-Native Migration for Pilot Deployments

Migrating the system to a cloud-native architecture (AWS) to move beyond local development and support pilot deployments with early users. This includes:

- Cloud-native deployment of the application and its data stores
- Infrastructure to support multiple concurrent users reliably and securely
- Operational tooling (monitoring, scaling, backup/recovery) appropriate for a pilot with real users rather than a single-developer environment
- Cost-efficient use of managed cloud services suited to an early-stage, usage-driven workload

This is the phase the project is entering next, and it's the basis for pursuing cloud partner programs and credits — the goal is to get real early users on a properly hosted, reliable deployment rather than continuing to iterate in a local-only environment.

## Beyond

Longer-horizon directions under consideration, contingent on pilot feedback:

- Expanded coverage across company universes and report types
- Broader industry-classification coverage and deeper comparative analytics
- [TODO: fill in additional forward-looking items as priorities firm up]
