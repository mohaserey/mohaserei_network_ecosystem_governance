# mohaserei_network_ecosystem_governance
Mohaserei System Network (MSN) — Ecosystem Governance (mohaserei_network_ecosystem_governance)

The Mohaserei Ecosystem Governance module (mohaserei_network_ecosystem_governance/index.html) is a standalone browser-based governance console for the Mohaserei System Network (MSN). It enables members and delegates to review active and ratified proposals, cast UES/HCV-weighted votes, inspect UES and HCV impacts, draft new governance proposals, explore Cambodia's 25 provinces and capital representation, and audit decision history.

Key Capabilities

Governance KPI Overview:

Tracks active vs. total proposals, charter quorum (35%) and supermajority approval (60%) thresholds, total UES voting power and registered voter metrics, and available vs. allocated MSN treasury reserves.

Proposal Workbench & Live Voting Console:

Filter proposals by All, Active, Passed, Treasury, or Protocol.

Inspect proposal summaries, requested MSN budgets, UES and HCV impact estimates, approval ratios, and quorum progress bars.

Cast or switch FOR, AGAINST, or ABSTAIN votes using the active delegate's UES voting weight (+420 UES in the default state), with automatic progression to PASSED when quorum and approval thresholds are met.

Publish new TREASURY or PROTOCOL proposals directly into the governance queue and audit log.

Council Roster, Charter Matrix & 25-Region Directory:

Outlines the four core governance pillars: Executive & Stewardship Council, Regional Commune & 25-Province Representation, UES & HCV Economic Voting Rules, and Treasury Safeguards.

Includes an expandable directory listing all 25 Cambodian administrative regions (Phnom Penh and the 24 provinces) in both Khmer and English.

Audit & Decision Log + JSON Export:

Search and filter logged VOTE, PROPOSAL, and SYSTEM events.

Export a timestamped JSON snapshot (Export JSON Snapshot) of the current Mohaserei governance state.

Bilingual UI (ខ្មែរ / EN), Voice Briefs & Local Persistence:

Switch between Khmer (ខ្មែរ) and English (EN) using Kantumruy Pro and Inter typography.

Play a spoken governance summary via the Web Speech API (speechSynthesis) with toast notifications as a fallback.

Persists state in localStorage under msn_governance_state_v1, with a one-click Reset Demo State action.

Running Locally

Open index.html directly in a modern browser or serve it from a static HTTP server:

python3 -m http.server 8080


Then navigate to http://localhost:8080/mohaserei_network_ecosystem_governance/index.html.

Ecosystem Integration Notes

Preserve the exact spelling Mohaserei across all documentation, modules, and datasets.

Connect loadState / saveState, voting actions, and proposal creation to authenticated Mohaserei Layer 2 governance endpoints and verified member UES/HCV identity records when deploying to production.
