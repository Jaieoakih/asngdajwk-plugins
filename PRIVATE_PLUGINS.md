# Maintainer notes

Source repositories are private. This repo stores build pins under `plugins/` and publishes signed JARs to Pages.

Set Actions secret `REPO_CREDS` to `USERNAME:PAT` (classic `repo` scope or fine-grained read on each source).

Then run **Build hub** (workflow_dispatch).
