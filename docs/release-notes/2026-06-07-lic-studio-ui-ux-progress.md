# Release notes: 2026-06-07 — lic studio-ui-ux-progress pin

**Status:** Pending merge  
**Repo:** li-langverse/li-net  
**PH / REQ:** ecosystem-upstream / meta-governance  
**Author:** code_implementer

---

## Summary

Bump `li-toolchain.toml` `lic_version` from `0.1.0` to upstream tag `studio-ui-ux-progress` on `li-langverse/lic` (World Studio UI/UX progress release).

## Agent continuation

1. Read: `li-toolchain.toml` and `.github/workflows/ci.yml` (lic checkout still tracks `main`)
2. Run: merge after CI green on the bump PR; close #8 via `org-close-issue.py`
3. Then: sibling repos (lip, li-demo, li-httpd) bump independently via their ecosystem-upstream issues
4. Blocked on: none for this pin-only change

## Changed

| Area | What | Evidence |
|------|------|----------|
| Toolchain | `lic_version` → `studio-ui-ux-progress` (`55defd82`) | `li-toolchain.toml` |
| Changelog | Unreleased entry | `CHANGELOG.md` |

## Not changed

- `src/lib.li` trusted TCP `extern` surface — unchanged
- `.github/workflows/ci.yml` lic checkout ref — still `main` (pin is downstream tracking metadata)
- `lic` compiler source — no edits in this repo

## Breaking changes

None.

## Security

N/A — dependency pin metadata only.

## Performance

N/A.

## Downstream

| Repo | Action |
|------|--------|
| lip, lit, li-demo, li-httpd | Independent `lic_version` pins via ecosystem-upstream issues |

## CHANGELOG entry

```markdown
### Changed
- Ecosystem: bump `lic_version` pin to `studio-ui-ux-progress` (upstream `li-langverse/lic` release).
```
