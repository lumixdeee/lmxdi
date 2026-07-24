# Chat-to-SM Ingest Report

**Version:** v0.001  
**UTC:** 2026-07-23T07:08:49Z  
**Status:** SM_READY

## Input

- Source: `sources/chat/chat_log.md`
- Source bytes: 22,411
- Source SHA-256: `74ec5fd22233a4aab7df7a0d8b18eb7bd14617bec9371b9a37ffed8820cbeaaf`
- Scope: visible user and assistant messages available at the checkpoint
- Excluded: system, developer, tool, and transient progress traffic

## Ingest result

- Added sources: 1
- Added units: 85
- Added retrieval keys: 3,002
- Added postings: 18,285
- Pointer failures: 0
- SQLite integrity: `ok`
- FTS rows: 160,420
- Master: `sm/SM_MASTR_v0.2_chat.sm`
- Master bytes: 155,815,936
- Master SHA-256: `1726c6e71bf888a77c44c76a76995e285e799aebf2f1b128f754f11320f204dc`

## Master totals

- Sources: 3,703
- Units: 4,255
- Keys: 160,420
- Postings: 1,203,247
- FTS keys: 160,420

## Segmentation

Each visible message is one non-overlapping unit. A unit stores:

- role-derived route
- message slot
- line start and end
- byte start and end
- exact-span SHA-256
- retrieval keys
- audit metadata

The sidecar is `sm/chat_log.sm`.

## Regression queries

- `wide seer prompts covetest` -> `M0013 USER`
- `only test is god` -> `M0019 USER`, `M0020 ASSISTANT`
- `SM first` -> route-audit units
- `proper shop basket found` -> `M0084 ASSISTANT`
- `zzzxxyyqqq_not_present_47291` -> `SM_MISS`

## Evidence boundary

The chat source is a checkpoint record assembled from visible conversation context. It is not described as a platform-native export. Hashes prove byte identity of the stored checkpoint and its message spans. They do not prove that any claim inside the chat is true.
