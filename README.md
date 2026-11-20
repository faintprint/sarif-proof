# sarif-proof

A test repository for Faintprint's SARIF output (`faintprint scan --sarif`)
and its GitHub Action. It holds made-up MCP servers only — our own test
cases, under `example.com` names, not real servers — and it is kept as a
demonstration.

- `tools/date-formatter.json` — a made-up server whose poisoned tool was
  removed, to show its alerts closing as fixed (a valid file with no
  results).
- `tools/md-formatter.json` — a made-up server with one borderline passage
  (a note without the AI review; `sarif/replay-recorded-review.sarif` is the
  same passage after a recorded, replayed review — no AI call was made).
- `tools/clock.json` — a made-up clean tool list (a valid file with no
  results).
- `action/p01-tools.json` — a made-up server with hidden instructions,
  scanned by the Faintprint Action (`.github/workflows/action*.yml`, run by
  hand).
- `.vscode/mcp.json`, `action/mcp.json` — config files naming a made-up
  local server. Faintprint never starts a server; the command is a made-up
  name, not a program anyone publishes.

The files under `sarif/` were written by Faintprint 0.8.0, offline, and
`.github/workflows/sarif-files.yml` uploads them to GitHub code scanning.
