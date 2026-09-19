# python-anthropic

`python:3.12-slim` with the [`anthropic`](https://pypi.org/project/anthropic/) Python SDK preinstalled — for jobs that need it without paying a `pip install` at every run.

```
ghcr.io/gergelyzs/python-anthropic:0.69.0
ghcr.io/gergelyzs/python-anthropic:latest
```

Built for `linux/amd64` and `linux/arm64`.

To bump the pinned SDK version: update `ARG ANTHROPIC_VERSION` in the `Dockerfile` and push to `main` (or run the "Build and push" workflow manually with a different `anthropic_version` input).
