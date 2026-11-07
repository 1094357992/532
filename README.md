# HydroGate: Evidence-Bounded Maintenance Decisions (ECE 532 final project proposal)

Yilong Peng, graduate track.

| File | What it is |
|---|---|
| `config/smoke.yaml`, `config/cpu.yaml` | Proposed smoke and full CPU configurations |
| `docs/DATA_ACCESS.md`, `data/manifest.json` | Data-access confirmation (UCI #447, CC BY 4.0) and SHA-256 of every data file |
| `docs/SCALEUP.md` | Optional scale-up justification (separately labeled; none requested) |
| `experiments/` | Evidence bundle: course schema-1.0 receipts, audits, compute records, decision traces |

`experiments/receipt.json` is the full CPU run's receipt, and it passes
`python -m utilities.verification.validate --strict experiments/receipt.json`.
The dataset itself is not committed. Download it from the source URL in `data/manifest.json`.
