# API-key version conflict test

Upload only these three source documents for the blind run:

- `01_v1_docs.md`
- `02_legacy_issue.md`
- `03_v2_migration_guide.md`

Then ask the exact question in `QUESTION.txt`.

Do not upload `EXPECTED_ANSWER.md` during the blind run. Keep it outside the test corpus and score the response afterward.

## Stronger second run

Rename the three source files so filenames no longer reveal their order, then repeat. The answer should still rank sources by version, status, scope, and source authority rather than filename order.

## Harder third run

Change the issue date so it is newer than the v2 guide while keeping `Applies to: v1.8`. A strong system should still treat it as historical because applicability matters more than timestamp alone.
