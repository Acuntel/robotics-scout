# Robotics Scout

A 30-day autonomous research loop hunting for the single best publicly investable company in the robotics/humanoid supply chain ("the picks-and-shovels play").

- **Owner:** Brady Schwartz (bradyschwartz25@gmail.com)
- **Run window:** 2026-08-08 through 2026-09-06 (30 daily runs, 12:00 UTC / 7:00 AM Chicago)
- **Mechanism:** A scheduled Claude cloud agent clones this repo daily, reads everything learned so far, executes the day's research rotation per `PROTOCOL.md`, updates `SCOREBOARD.md`, appends `log/YYYY-MM-DD.md`, and pushes.
- **Endgame:** On 2026-09-06 the agent writes `FINAL_VERDICT.md` (the pick, evidence chain, entry logic, invalidation criteria) and drafts an email summary to Brady.

## Files

| File | Purpose |
|---|---|
| `CRITERIA.md` | The fixed scoring rubric. Do not change weights mid-run without logging why. |
| `PROTOCOL.md` | Daily rotation, research rules, and final-verdict spec. |
| `SCOREBOARD.md` | Live weighted rankings + changelog. |
| `log/` | Append-only daily research logs. Never delete or rewrite history. |
| `FINAL_VERDICT.md` | Written once, at the end. Its existence means the run is over. |

## After the verdict

Disable the routine at https://claude.ai/code/routines (runs after the verdict are no-ops but still cost a session spin-up).
