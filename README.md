# python-anthropic

`python:3.12-slim` with the [`anthropic`](https://pypi.org/project/anthropic/) Python SDK preinstalled — for jobs that need it without paying a `pip install` at every run.

```
ghcr.io/gergelyzs/python-anthropic:0.69.0
ghcr.io/gergelyzs/python-anthropic:latest
```

Built for `linux/amd64` and `linux/arm64`.

To bump the pinned SDK version: update `ARG ANTHROPIC_VERSION` in the `Dockerfile` and push to `main` (or run the "Build and push" workflow manually with a different `anthropic_version` input).

## Claude Code variant

`claude-code.Dockerfile`: `node:22-bookworm-slim` + `python3` + the Claude Code CLI, for jobs that call `claude -p` on a Claude subscription (`CLAUDE_CODE_OAUTH_TOKEN` from `claude setup-token`) instead of API credits.

```
ghcr.io/gergelyzs/python-anthropic:claude-code-2.1.302
```

To bump: update `ARG CLAUDE_CODE_VERSION` and push to `main`.
