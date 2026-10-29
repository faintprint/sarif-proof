# sarif-proof

A test repository for Faintprint's SARIF output (`faintprint scan --sarif`).
It holds made-up MCP servers only — our own test cases, not real servers —
and a workflow that uploads SARIF files to GitHub code scanning. It is
deleted after the proof.

- `tools/date-formatter.json` — a tool list with hidden instructions (two alerts).
- `tools/md-formatter.json` — a tool list with one borderline passage (a note
  without the AI review; `sarif/replay-recorded-review.sarif` is the same
  passage after a recorded, replayed review — no AI call was made).
- `tools/time.json` — a clean tool list (a valid file with no results).
