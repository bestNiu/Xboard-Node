# fly001 node deployment

The component keeps the internal `xboard-node` binary, config paths and Go module name for upstream compatibility. Deployment-facing names use `fly001`.

Copy `.env.example` to `.env`, set a node token created by Xboard, then run:

```bash
docker compose -f compose.dev.yaml up -d --build
```

`FLY001_PANEL_URL` may point to an internal HTTP URL for development. Production must use an authenticated HTTPS endpoint. Never use a GitHub token as `FLY001_NODE_TOKEN`.

Commercial authorization documents are maintained outside the public source repository. Existing upstream attribution remains unchanged.
