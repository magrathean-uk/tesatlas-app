# tesatlas-app (Tesatlas public documentation)

Public App documentation only: EULA, privacy, terms, subscription and trademark copy for
the Tesatlas iOS app. No application code, build system or test suite. Remote:
`magrathean-uk/tesatlas-app` (public).

## Working rules

- Keep the separate Teslatlas Hub name and links; do not conflate the App and the Hub.
- Preserve purchase and bundle identifiers, subscription terms and original evidence
  exactly. Legal files are owner-controlled: change `LICENSE`, `EULA.md`, `PRIVACY.md`,
  `TERMS.md`, `SUBSCRIPTION.md`, `TRADEMARKS.md` only on the owner's explicit instruction.
- Apply `NEXT-RELEASE-URLS.md` at the next release (product sites -> `https://magrathean.uk/solutions/<slug>/`, support -> `contact+<slug>@magrathean.uk`), then remove that file.

## Validation

Documentation only: `git diff --check`, check relative links and headings, confirm the
App Store facts match the shipped app. No build is needed; say what was checked.

## Models

Any agent for prose edits (Claude Sonnet 5.5, or Codex `gpt-6.1-sol`). Keep changes small
and factual; do not invent product claims.

<!-- clean-development-policy:v4 (clean-development 0.6.0; canonical: bolyki-dev/clean-development/docs/policy-snippet.md) -->
## Clean development (mandatory)

- Storage is routed for you: every zsh loads `~/dev/machine/env.zsh`; hooks pin the mode per session (`$CLEAN_DEV_MODE` is `external` when the 4TB is attached, else `internal`). Do not wrap commands, override or unset the routed variables.
- Temp files go to `$TMPDIR` (session scratch, deleted at session end), throwaway build output to `$CLEAN_DEV_BUILDS`, caches wherever their variables point. Never write caches, builds or temp files into `~`, `~/dev` or this repo outside its git-ignored build directories.
- Internal mode: before any download or build likely over 5 GB, stop and ask G (suggest waiting for the 4TB).
- This repo's `.clean-development.json` (schema v2) lists its git-ignored `buildDirs`/`depDirs`; keep it accurate when the build layout changes.
- No dot-folders in `~` or `~/dev`. `.env` files stay git-ignored; read them only when the task needs them; never commit them.
