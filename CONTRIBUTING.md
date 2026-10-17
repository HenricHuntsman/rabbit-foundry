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
