# Vanguard Website

Static prototype of the vanguard.com.sa rebuild. `index.html` plus `img/`. No build step.

## Pages and addresses

Every page has its own address: `/about`, `/services/strategy`, `/work/esports-world-cup` and so on. They are all served by `index.html`; `vercel.json` sends any address without a file to it. Old `/#about` style links still land on the right page.

Opening `index.html` straight from disk no longer works, because the addresses need a server. To preview locally, run this in the project folder and open the address it prints:

```bash
npx serve -s
```

## Before launch

- **Search engines:** `vercel.json` sends `X-Robots-Tag: noindex, nofollow` on every page. Remove that header to let the site be indexed.
- **Share image:** `img/share.jpg` is the picture shown when a link is pasted into a chat or social post. Most apps need its full address, so once the final domain is known, change `og:image` in `index.html` from `/img/share.jpg` to the full `https://…/img/share.jpg`.
- **Forms:** the contact and booking forms open the visitor's email app with the enquiry filled in, addressed to hello@vanguard7.com. Sending straight from the page needs an email or form service.

## Team portraits

Files are `img/p-<name>.webp`, 480 × 600. The current set has had its backgrounds replaced with one shared dark backdrop so the row reads as a set. New portraits should be shot or cut out against a plain dark background to match.

## Partner logos

Partner names on the home page and the Partners page are logo slots. Add a file to `img/logos/` with the name below and it replaces the typed name automatically. SVG is preferred; a `.png` with the same name also works. Any colour is fine: logos are shown in single-colour white on dark backgrounds and black on light ones. Crop files tight to the mark, with no padding.

If a mark reads too big or too small next to the others, set its size in `LOGO_SCALE` in `index.html`, e.g. `{'stc-play':0.8}`.

| Organisation | File |
| --- | --- |
| Esports World Cup Foundation | `esports-world-cup-foundation.svg` |
| Savvy Games Group | `savvy-games-group.svg` |
| Saudi Esports Federation | `saudi-esports-federation.svg` |
| stc play | `stc-play.svg` |
| Global Esports Federation | `global-esports-federation.svg` |
| Saudi Arabian Football Federation | `saudi-arabian-football-federation.svg` |
| International Esports Federation | `international-esports-federation.svg` |
| Misk Foundation | `misk-foundation.svg` |
| Saudi Sports for All Federation | `saudi-sports-for-all-federation.svg` |
| West Asian Football Federation | `west-asian-football-federation.svg` |
| National Events Center | `national-events-center.svg` |
| King Abdulaziz City for Science and Technology | `king-abdulaziz-city-for-science-and-technology.svg` |
| Riot Games | `riot-games.svg` |
| Blizzard Entertainment | `blizzard-entertainment.svg` |
| Tencent Games | `tencent-games.svg` |
| Electronic Arts | `electronic-arts.svg` |
| Epic Games | `epic-games.svg` |
| Ubisoft | `ubisoft.svg` |
| Krafton | `krafton.svg` |
| Moonton | `moonton.svg` |
| Embark Studios | `embark-studios.svg` |

### Current logo files

| File | Source | Note |
| --- | --- | --- |
| `esports-world-cup-foundation.png`, `saudi-esports-federation.png`, `misk-foundation.png` | vanguard.com.sa | Good resolution |
| `savvy-games-group.png`, `stc-play.png`, `global-esports-federation.png`, `saudi-arabian-football-federation.png`, `international-esports-federation.png`, `riot-games.png` | vanguard.com.sa | Small (about 150px wide), soft on high-resolution screens: replace with SVGs from each organisation |
| `blizzard-entertainment.svg`, `electronic-arts.svg`, `ubisoft.svg` | Wikimedia Commons | Vector |

Still needed: Saudi Sports for All Federation, West Asian Football Federation, National Events Center, King Abdulaziz City for Science and Technology, Tencent Games, Epic Games (a single-colour version: the standard shield logo loses its lettering), Krafton, Moonton, Embark Studios.
