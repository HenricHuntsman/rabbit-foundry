# CLI reference

## `rabbit`

| Command | Purpose |
| --- | --- |
| `rabbit version` | show Rabbit Code version |
| `rabbit doctor` | check local Python, tools, Ollama and PATH (`--json` supported) |
| `rabbit models` | list installed local Ollama models |
| `rabbit ui` | start the local Linux browser workspace |
| `rabbit chat 'hello'` | ask the local model |
| `rabbit agent` | inspect a project with read-only agent tools |

## `rabbit-code`

Runtime entry point (`rabbit_foundry.rabbit_code:main`). Optional one-shot
commands include `capabilities`, `read` and `agent`. Key flags: `--workspace`,
`--provider`, `--base-url`, `--model`, `--allow-network`, `--allow-write`,
`--allow-exec`, `--ui`. Run `rabbit-code --help` for the full list.

Use `rabbit <command> --help` for options of each command.
