# .github

Organisation-level defaults for Doryven.

| Path | Renders at |
|---|---|
| `profile/README.md` | <https://github.com/Doryven> — the organisation profile page |
| `profile/assets/` | brand artwork referenced by that page |

Artwork here is **copied** from [`doryven-brand`](https://github.com/Doryven/doryven-brand),
which stays the source of truth. Re-copy from there rather than editing in place, so the
identity cannot drift between the two.

**This repository is private, so the profile page is currently visible to organisation
members only.** Making it public publishes the profile to everyone:

```sh
gh repo edit Doryven/.github --visibility public --accept-visibility-change-consequences
```
