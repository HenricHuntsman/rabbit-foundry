# Troubleshooting

- **`rabbit: command not found`** — activate the virtualenv or add
  `~/.local/bin` to `PATH`, then run `rabbit doctor`.
- **`No module named torch`** — only training/backend tests need it:
  `pip install -e ".[training]"`. On Fedora see the torch section of the README.
- **No models listed** — install and start Ollama, pull a model, then run
  `rabbit models`.
- **Tests fail on import** — install dev extras: `pip install -e ".[dev]"`.
