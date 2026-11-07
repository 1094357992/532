# Optional scale-up justification (separately labeled; not graded)

**Request: none.** Every graded requirement runs on CPU: the smoke run took seconds, and the full
`config/cpu.yaml` evaluation took the runtime recorded in `experiments/cpu/compute.json`. No GPU hours, API
credit, or personal spending is requested or assumed.

If the team revisits this after the Dec 1 progress gate, the only candidate is a small 1-D CNN on raw
100 Hz pressure and power waveforms, to test whether a learned A1 representation lifts accumulator accuracy.
That request would stay under 2 GPU hours, with cached embeddings committed for deterministic CPU replay. It would
be reported separately and would not replace the CPU baseline.
