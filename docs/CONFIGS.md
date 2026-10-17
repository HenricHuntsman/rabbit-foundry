# Config reference

Files in `configs/`:

| File | Purpose |
| --- | --- |
| `model_gateway.example.json` | Local model gateway: provider endpoint/model, Rabbit endpoint alias and permissions. See [MODEL_GATEWAY.md](MODEL_GATEWAY.md). |
| `experiment.example.json` | Fixed-vs-adaptive training experiment: seeds, skills, frozen evaluation settings. |
| `sources.example.json` | Read-only source ingestion manifest: repository, full commit SHA, licence, paths, and allowed licences. |
| `bunny_lineage.json` | Bunny lineage policy (no weights in git, holdout separation, Greenlight promotion). See [BUNNY_LINEAGE.md](BUNNY_LINEAGE.md). |
| `space_bunny_sources.json` | Space Bunny research sources. |
| `kilo.compat.jsonc` | Kilo compatibility config pointing at the local Rabbit endpoint (`http://127.0.0.1:8765/v1`). |
| `opencode.compat.jsonc` | OpenCode compatibility config pointing at the same endpoint. |

Files named `*.example.json` are templates: copy and edit them. Never put
credentials in these files.
