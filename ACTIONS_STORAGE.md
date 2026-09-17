# GitHub Actions storage

EOPLite builds use GitHub Actions. The free plan includes limited **artifact storage**.

## If workflows fail with storage quota errors

1. Open **GitHub → Settings → Billing → Actions → Storage**
2. Delete old **Artifacts** on repos that run heavy builds
3. Re-run only what you need via **workflow_dispatch** on the hub and client repos

## Retention

Hub and client workflows use **short artifact retention** (1 day) where configured to reduce storage use.

## Manifest version aliases

If the client version moved ahead of hub manifest names, use **Publish manifest version aliases** on this repo (manual workflow) instead of rebuilding all plugins.
