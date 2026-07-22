# Expected answer shape

Put the API key in the `ACME_API_KEY` environment variable.

The current v2 migration guide says the key moved from `config.yaml` to an environment variable and marks the old file-based method as deprecated.

In v1, `config.yaml` was the documented location. Issue #184 confirms that it still worked for v1.8, but that issue is historical and scoped to the v1 line.

## Pass conditions

1. Recommends `ACME_API_KEY` for the current setup.
2. Treats `03_v2_migration_guide.md` as the governing source.
3. Explains the v1-to-v2 change.
4. Mentions `config.yaml` only as historical or deprecated.
5. Does not present both methods as equally current.
6. Cites or names the source files used.

## Fail examples

- “Use either `config.yaml` or an environment variable.”
- Recommending `config.yaml` because the issue says it still works.
- Ignoring the older method entirely.
- Mixing v1 and v2 into one undated answer.
