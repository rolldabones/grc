# Evidence: grc prompt pack, run T5, 18 October 2026 (KST)

**What.** The transcripts and scores of suite `grc-sp0` (cases G1 and G2 of [`../../tests.md`](../../tests.md)), with the run's `summary.json`.

**When and how.** Run in Michael Paik's Terminal on 18 October 2026, finished 10:28 KST, by the session T5 harness (`t5_run.py`, not shipped in this repository): API system prompt, no tools, max_tokens 16000, one user turn per case. Tested model `claude-opus-5-5`; scorer `claude-sonnet-5-5`, a different model scoring each transcript against the case's pass condition. LLM scoring is developer testing, not independent assurance.

**System text.** The fenced prompt block under "## Prompt" in each prompt file, extracted byte for byte: A2 SHA-256 `c09cb31e3fc47283855f2014f4ba85071b9f1a80d176e13c3bc2d86bce5e7cd7`, A4 SHA-256 `1975e3c289899ba1c26451bcb088d10f7e9231f3bacb840ad4d3b849826568fe`. `summary.json` records HEAD `cb22408`, the commit before v2.3.0; the prompt text run is the v2.3.0 working-tree text, which the two digests identify.

**Files.** Each transcript is copied byte for byte from the harness output; only the closing line below was appended. `summary.json` is copied unchanged.

| File | Case | Scorer verdict | SHA-256 as produced |
| --- | --- | --- | --- |
| G1.md | G1, A2 Objectives | PASS | `cdf770aff651338eb47ae3dd247e684a51cafb19bd0db454da110ffe3f352216` |
| G2.md | G2, A4 Assessment | PASS | `770fb53b4d7172b35399ff88baa26caa18babb1aa2e8ca42007524c857e4f5a7` |
| summary.json | run summary | n/a | `9c35d86630d5ba3cad5feebe2b350a0602544fce1f77689449f018162e880812` |

Model output inside the transcripts is verbatim and is not edited for house style.

---

Final Liability rests with the Human.
