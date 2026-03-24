# Constraint-Architecture Repository Archive Hash

This document records the cryptographic hash of the sealed repository
archive produced on 2026-03-24, following the hardening pass.

---

## Archive Details

| Field | Value |
|---|---|
| File | `Constraint-Architecture-main-2026-03-24.zip` |
| Date sealed | 2026-03-24 |
| Algorithm | SHA-256 |
| Hash | `2DA95899744AFCFF3A9C13AADFB47BE11166BDC262002A53CA7E8B46964F6CE5` |

---

## What This Hash Covers

This hash covers the complete repository state as downloaded from
`github.com/JonathanMastersWatson/Constraint-Architecture` on
2026-03-24, following the hardening pass which included:

- README.md — terminology hardening, three-layer stack table,
  corrected CVS name (Sidecar not System), role language hardened,
  canonical repo links added, repository structure section completed

---

## Verification

To verify this hash, download the archive and run:
```powershell
(Get-FileHash "Constraint-Architecture-main-2026-03-24.zip" -Algorithm SHA256).Hash
```

The output must match the hash recorded above exactly.

---

## Note on Archive Sequence

This is the first sealed archive for this repository.

The Constraint-Architecture repo defines the upstream constraint
definition discipline that sits above the 512 and CVS canonical
repos. All three repos are sealed on the same date as part of a
coordinated hardening pass.

| Repo | Archive date | Hash |
|---|---|---|
| 512 | 2026-03-24 | `DF27F6C5C8DDBBD5341FB15EA943D92B3388331B386C26F44A145673F6C8D218` |
| CVS | 2026-03-24 | `0DA1ABA3A7257B636C0A364920C5CE643843257D217C0DBD68BA5DB64712BE17` |
| Constraint-Architecture | 2026-03-24 | `2DA95899744AFCFF3A9C13AADFB47BE11166BDC262002A53CA7E8B46964F6CE5` |
