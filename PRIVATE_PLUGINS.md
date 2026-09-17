# Maintainer notes (plugin sources)

Plugin **source** is built from private repositories. This hub only stores version pins under `plugins/` and publishes **signed JARs** to Pages — not source code.

## Actions secret: `REPO_CREDS`

The build needs a GitHub PAT that can read those private sources. In **Settings → Secrets and variables → Actions**, set:

`REPO_CREDS` = `YOUR_GITHUB_USERNAME:YOUR_PAT`

Use a classic PAT with **`repo`** scope, or a fine-grained PAT that includes every pinned source repository.

Then run **Build EOPLite Plugin Hub** (workflow_dispatch).
