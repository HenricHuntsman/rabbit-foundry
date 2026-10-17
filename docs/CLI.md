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

Runtime entry point (`rabbit_foundry.rabbit_code:main`). Run
`rabbit-code --help` for the available subcommands.

Use `rabbit <command> --help` for options of each command.
