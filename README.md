# .github

Organisation-level defaults for Doryven.

| Path | Renders at |
|---|---|
| `profile/README.md` | <https://github.com/Doryven> — the organisation profile page |
| `profile/assets/` | brand artwork referenced by that page |

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
