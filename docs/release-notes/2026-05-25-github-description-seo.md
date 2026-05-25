# Release notes: 2026-05-25 — github-description-seo

**Status:** Ready for review  
**Repo:** li-langverse/li-net  
**Author:** agent (WP-A4)

## Summary (one sentence)

Replace template `Li package li-net` GitHub description with HPC/scientific networking blurb; README + `.github/repo-description`.

## Agent continuation (required)

1. Read: `.github/repo-description`.
2. Run: `gh repo view li-langverse/li-net --json description`; post-merge `gh repo edit` if needed.
3. Then: package implementation work on `main`.
4. Blocked on: WP-H2 LICENSE — **none**.

## Changed (specific)

- `.github/repo-description`, `README.md`, `CHANGELOG.md`.

## Not changed (scope fence)

- `src/`, `lic` build, `li-httpd` — **not** touched.
- SPDX/LICENSE mass-edit — WP-H2.
- `benchmarks` ingest — **not** in this PR.

## Breaking changes

None.

## Security

N/A.

## Performance

N/A.

## Downstream

N/A.
