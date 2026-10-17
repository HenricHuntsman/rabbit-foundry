# Contributing

```bash
python -m venv .venv
source .venv/bin/activate
pip install -e ".[dev]"            # lightweight CLI/UI tests
pip install -e ".[dev,training]"   # adds torch for the full suite
pytest -q
```

- Keep changes small and covered by tests in `tests/`.
- Frozen evaluation cases must never be moved into training data.
- Do not commit checkpoints, credentials or captured trajectories.
- Only advertise capabilities that really work.

## Which tests need torch?

Tests that import `torch` (adaptive training, candidate/frozen evaluation,
export readiness, model, preview server, train episodes, weight continuation,
bunny train, experiment) need `pip install -e ".[dev,training]"`. All other
tests, including the CLI, installer, web UI and Linux desktop tests, run with
`pip install -e ".[dev]"`. To run only the lightweight set, ignore the
torch-dependent files with `pytest --ignore=tests/test_model.py ...`.
