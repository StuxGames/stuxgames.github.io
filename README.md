<p align="center">
  <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.games/logo-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.games/logo-dark.png"><img src="https://global.media.stux.games/logo-dark.png" height="100" alt="Stux.Games Logo"></picture>
</p>

# Stux.Games GitHub Pages Redirect

### *Sends `stuxgames.github.io` to [github.com/StuxGames](https://github.com/StuxGames).*

Anyone who visits [stuxgames.github.io](https://stuxgames.github.io) is forwarded straight to the Stux.Games GitHub
organisation. Stux.Games' own sites (stux.games, games.stux.games, status.stux.games) are served on their own domains,
not from here.

## How it works

`index.html` is a single static page with a meta refresh and a canonical link, both pointing at
`https://github.com/StuxGames`. `.github/workflows/pages.yml` deploys it to GitHub Pages with Actions on every push to
`main`, so each deploy is an ordinary, visible CI run.

To change where it goes, edit both URLs in `index.html`:

```html
<meta http-equiv="refresh" content="0;url=https://github.com/StuxGames" />
<link rel="canonical" href="https://github.com/StuxGames" />
```

## Want one of your own?

This repo isn't a template. Use [StuxGroup/GitHubPagesRedirect](https://github.com/StuxGroup/GitHubPagesRedirect),
the template it's based on.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## Versioning

This project uses [Date Versioning](https://datevers.ing): each release is numbered by its UTC release date as `YY.MM.DD` (for example `26.10.23`), with `-1`, `-2`… for later releases the same day. See [CHANGELOG.md](CHANGELOG.md) for what changed in each release.

Releases are made on the `test` branch and go live when its pull request into `main` is merged; see [CONTRIBUTING.md](CONTRIBUTING.md#branches).

## Copyright

Copyright © 2026 Stux Group Ltd. All rights reserved.

---

*Built & Maintained by <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.games/icon-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.games/icon-dark.png"><img src="https://global.media.stux.games/icon-dark.png" height="14" alt="Stux.Games" valign="middle"></picture> [Stux.Games](https://github.com/StuxGames), Hosted by <img src="https://github.com/Stuxedo.png" height="14" alt="Stuxedo" valign="middle"> [Stuxedo](https://stuxedo.com).  
Stux.Games is a part of the <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.group/icon-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.group/icon-dark.png"><img src="https://global.media.stux.group/icon-dark.png" height="14" alt="Stux.Group" valign="middle"></picture> Stux.Group brand of businesses.*
