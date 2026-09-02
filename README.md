# schplay.com

**A fast, lightweight browser games site.**

schplay.com hosts 300+ HTML5 and WebGL games that run instantly in the browser — no downloads, no installs, no account required to play.

**Live site:** https://schplay.com

---

## Table of contents

- [About](#about)
- [Games](#games)
- [Features](#features)
- [Adding a game](#adding-a-game)
- [Reporting content](#reporting-content)
- [Contributing](#contributing)

---

## About

schplay was built around one idea: browser games should load fast and work on cheap hardware. Pages are static and the shell is small enough to render on a low-end Chromebook over a slow connection.

The catalog is curated rather than scraped. Each game is checked for playability in-browser and whether it works without plugins before it goes live.

## Games

Game pages live at `schplay.com/games/<game-name>`.

<!-- GAMES_LIST_START -->

- [Minecraft](https://schplay.com/games/minecraft)
- [Slope](https://schplay.com/games/slope)
- [Geometry Dash](https://schplay.com/games/geometry-dash)
- [1v1.LOL](https://schplay.com/games/1v1-lol)
- [Plants vs. Zombies](https://schplay.com/games/plants-vs-zombies)
- [Papa Louie Arcade](https://schplay.com/games/papa-louie-arcade)
- [Subway Surfers](https://schplay.com/games/subway-surfers)
- [Five Nights at Freddy's](https://schplay.com/games/five-nights-at-freddys)
- [Slither.io](https://schplay.com/games/slither-io)
- [Agar.io](https://schplay.com/games/agar-io)
- [Basketball Stars](https://schplay.com/games/basketball-stars)
- [Drift Hunters](https://schplay.com/games/drift-hunters)
- [Getaway Shootout](https://schplay.com/games/getaway-shootout)
- [Temple Run 2](https://schplay.com/games/temple-run-2)
- [Cut the Rope](https://schplay.com/games/cut-the-rope)
- [Spelunky](https://schplay.com/games/spelunky)
- [People Playground](https://schplay.com/games/people-playground)
- [Raft: The Final Chapter](https://schplay.com/games/raft-the-final-chapter)
- [Bendy and the Ink Machine](https://schplay.com/games/bendy-and-the-ink-machine)
- [Quake](https://schplay.com/games/quake)

<!-- GAMES_LIST_END -->

Browse the full catalog at [schplay.com](https://schplay.com).

## Features

**Instant play.** Games load in an isolated frame with no install step.

**Curated catalog.** 300+ titles, sorted into featured and popular shelves on the homepage, with search across the full library.

**Lightweight shell.** Static HTML, CDN-backed assets, minimal JavaScript on the landing page.

**Game requests.** Players can request titles directly from the site.

## Adding a game

1. Add an entry to the catalog file:

```json
{
  "slug": "game-slug",
  "title": "Game Title",
  "genre": "Puzzle",
  "thumbnail": "/thumbs/game-slug.webp",
  "embed": "/games/game-slug/index.html"
}
```

2. Drop assets in `/public/games/game-slug/`.
3. Write the description by hand. Don't generate it — templated descriptions across hundreds of pages get flagged as scaled content and won't index.
4. Open a PR.

## Reporting content

If you're a rights holder and believe something on the site infringes your work, open an issue on this repository and it will be taken down while the claim is reviewed.

## Contributing

Issues and PRs welcome. Useful contributions:

- Performance work on the catalog page
- Accessibility fixes
- Bug reports with a browser and device listed
