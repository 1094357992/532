# HydroGate: Evidence-Bounded Maintenance Decisions (ECE 532 final project proposal)

Yilong Peng, graduate track.

| File | What it is |
|---|---|
| `config/smoke.yaml`, `config/cpu.yaml` | Proposed smoke and full CPU configurations |
| `data/condition_monitoring_of_hydraulic_systems.zip` | The dataset: original UCI #447 archive, CC BY 4.0 (see `data/README.md`) |
| `docs/DATA_ACCESS.md`, `data/manifest.json` | Data-access confirmation and SHA-256 of the archive and every file in it |
| `docs/SCALEUP.md` | Optional scale-up justification (separately labeled; none requested) |
| `experiments/` | Evidence bundle: course schema-1.0 receipts, audits, compute records, decision traces |

`experiments/receipt.json` is the full CPU run's receipt, and it passes
`python -m utilities.verification.validate --strict experiments/receipt.json`.
The dataset archive is included under `data/`; its hash matches `data/manifest.json`.
