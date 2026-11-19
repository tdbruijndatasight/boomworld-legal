# boomworld-legal (redirect shell)

The Boombaland legal pages and support page moved to **https://www.boombaland.com/** (repo
`tdbruijndatasight/boombaland-site`). This repo only keeps the old github.io URLs answering:

| Old URL (tdbruijndatasight.github.io/boomworld-legal/…) | Goes to |
|---|---|
| `/` | https://www.boombaland.com/ |
| `/privacy/` | https://www.boombaland.com/privacy/ |
| `/terms/` | https://www.boombaland.com/terms/ |
| `/support/` (keeps `#delete-your-account-and-data`) | https://www.boombaland.com/support/ |
| any other path (`404.html`) | https://www.boombaland.com/ |

Each page answers 200 with a canonical link, `noindex`, an instant meta refresh and a script redirect that keeps the
`#anchor`. `app-ads.txt` and `.nojekyll` are unchanged.

**Keep this repo published.** Old game builds may still open these URLs, and the root must keep answering (HTTP 200
with a `Date` header) for any build whose clock check still points here. Do not delete the repo while such a build is
in use.
