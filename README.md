# SCSOI tools — Scoop bucket

Personal bucket for the four SCSOI Windows tools. It is not an official Scoop bucket; add it like any other:

```powershell
scoop bucket add scsoi https://github.com/shuyingegit/scoop-bucket
scoop install scsdrive
```

| Package | What it does | Site |
|---|---|---|
| `scsdrive` | Mount a NAS / WebDAV share as a real local drive letter | https://drive.scsoi.com |
| `scssubst` | Give an existing local folder its own drive letter | https://subst.scsoi.com |
| `scsdedup` | Find duplicate files by content hash | https://dedup.scsoi.com |
| `scsexpand` | Grow a partition using free space on the same disk | https://expand.scsoi.com |

Notes:

- Windows 10 / 11 (64-bit) only.
- Each tool has a 7-day full-feature trial; no ads, no forced subscription.
- `scsdrive` installs the open-source user-mode driver it needs (Dokany, LGPL) on first launch; the other three need no driver and no administrator rights.
- Manifests are plain singletons; `scoop update scsdrive` picks up a new version, then reinstall to upgrade.
