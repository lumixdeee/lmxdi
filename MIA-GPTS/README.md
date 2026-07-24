# Shopping Method Study v0.001

This package contains the four requested stages in strict order:

1. Pre-chat-ingest paper in Markdown and PDF
2. Chat source ingested into a new SM master
3. SM-with-chat edition of the paper in Markdown and PDF
4. Difference discussion in Markdown and PDF

## Papers

- `papers/Shopping_Old_Way_vs_New_Way_v0.001.md`
- `papers/Shopping_Old_Way_vs_New_Way_v0.001.pdf`
- `papers/Shopping_Old_Way_vs_New_Way_SM_v0.001.md`
- `papers/Shopping_Old_Way_vs_New_Way_SM_v0.001.pdf`
- `papers/Discussion_PreIngest_vs_SM_v0.001.md`
- `papers/Discussion_PreIngest_vs_SM_v0.001.pdf`

## SM additions

- `sources/chat/chat_log.md`
- `sm/chat_log.sm`
- `sm/SM_MASTR_v0.2_chat.sm`

The new master extends `SM_SHOP_v0.1` and does not overwrite it. Existing corpus pointers still depend on the original source archives. The new chat pointers resolve inside this package.

## Reports

- `reports/INGEST_REPORT.md`
- `reports/QUERY_AUDIT.json`
- `reports/PDF_VERIFY.md`
- `MANIFEST.sha256`
