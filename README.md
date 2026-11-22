# ple-harness

PLE (Physical Engineering's Last Exam) competition entry harness.

This repository currently holds the minimal skeleton taken from the official
kit's `sample_submissions/minimal` example in
[google-research/ple](https://github.com/google-research/ple) (Apache-2.0):
a short tool-calling loop (`serve.py`, built on `taskbridge.py`) that calls
the Google-sponsored `google-cloud/gemini-3.8-flash` model declared in
`submission.yaml`. It exists so the entry passes the kit's structural
checks; it is a starting point, not a tuned solution.

| File | Purpose |
|---|---|
| `submission.yaml` | Model declaration, build command, server startup command |
| `serve.py` | Agent loop and tool definitions |
| `taskbridge.py` | Serve protocol implementation (from the official kit) |
| `requirements.txt` | Pinned `openai` and `websockets` dependencies |

`artifacts/` is not included yet: it is produced by running the harness on
the public dev set with `eval/run.py` from the official kit.
