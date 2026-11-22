# Vanguard Website

Static prototype of the vanguard.com.sa rebuild. `index.html` plus `img/`. No build step.

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
