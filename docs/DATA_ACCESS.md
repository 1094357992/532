# Data-access confirmation

**Status: confirmed (downloaded and verified 2026-11-06).**

| Item | Value |
|---|---|
| Dataset | Condition monitoring of hydraulic systems, UCI Machine Learning Repository #447 |
| Creators | N. Helwig, E. Pignanelli, A. Schütze (ZeMA gGmbH / Saarland University) |
| License | CC BY 4.0 (public; no account, application, or payment) |
| Source | https://archive.ics.uci.edu/static/public/447/condition+monitoring+of+hydraulic+systems.zip |
| Archive size | 76,601,704 bytes |
| Archive SHA-256 | `24128aad2ee45eea7e6b63ebbd9992cdf25d0483a2cebefbfc13bc69079af1f2` |
| Contents | 17 sensor files (2205 cycles each), `profile.txt` (labels), 2 documentation files |
| Per-file hashes | `data/manifest.json` (loader fails closed on any mismatch) |

Setup is the only networked step: `python scripts/fetch_data.py`. Every later step reads the
verified local files plus a binary cache derived from them.

Content checks we ran:
- 2205 cycles; each sensor has rate × 60 samples (PS1–6 and EPS1: 6000; FS1–2: 600; the rest: 60).
- Label distributions match the dataset documentation (e.g. valve 100/90/80/73 % = 1125/360/360/360 cycles).
- No missing values.

Ethics: these are laboratory measurements from a test rig. They contain no personal data and no human subjects.
