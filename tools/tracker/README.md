# Tracker (local web page for the job tracker)
Signed: Claudio · Career PM (Claude), 2026-10-28.

Code only. The data, `work/applications-tracker.xlsx`, is git-ignored (lead and contact details stay out of this public repo until Carlos makes it private).

- Run: `tools\tracker\open-tracker.bat` (local, 127.0.0.1:8765), or `python -I tools/tracker/server.py`.
- Reads and writes `work/applications-tracker.xlsx`, shared with the daily rerun. Override with `TRACKER_XLSX` and `TRACKER_PORT` (always do this for tests: never test on the real file).
- It only records. Applying and sending stay with Carlos (AGENTS.md rule 6).
- Check: `selftest.md`.
