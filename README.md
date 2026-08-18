# .github

Organisation-level defaults for Doryven.

| Path | Applies to |
|---|---|
| `profile/README.md` | <https://github.com/Doryven> — the organisation profile page |
| `profile/assets/` | brand artwork referenced by that page |
| `SECURITY.md` | every Doryven repository without its own |
| `CONTRIBUTING.md` | every Doryven repository without its own |
| `CODE_OF_CONDUCT.md` | every Doryven repository without its own |
| `.github/ISSUE_TEMPLATE/` | issue forms, org-wide |
| `.github/PULL_REQUEST_TEMPLATE.md` | pull request template, org-wide |

GitHub falls back to these files for any repository that does not ship its own, so a new
repository arrives with a security policy and contribution rules already in place. A
repository that needs different terms overrides them by committing its own copy — the
per-repository file always wins.

The addresses in these policies (`security@`, `conduct@`) must exist before anyone relies
on them. A published security contact that bounces is worse than none.

Artwork here is **copied** from [`doryven-brand`](https://github.com/Doryven/doryven-brand),
which stays the source of truth. Re-copy from there rather than editing in place, so the
identity cannot drift between the two.

The logo is committed and referenced by raw URL rather than drag-and-dropped into the
editor: an uploaded attachment lives outside version control and is tied to the uploading
account, so it cannot be reviewed, replaced in a commit, or restored if lost. `<picture>`
serves the white cut on dark themes and the navy cut on light ones.

## Visibility

**The profile page only renders while this repository is public.** A private `.github`
renders nothing at all -- not to the public and not to organisation members. (The
members-only equivalent is a separate repository named `.github-private`.)

To publish the profile:

```sh
gh repo edit Doryven/.github --visibility public --accept-visibility-change-consequences
```
