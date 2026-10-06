# PESTILLENCE — Landing Page

A single-file gothic landing page (`index.html`) for the PESTILLENCE Wix store
(https://cazzzua.wixstudio.com/my-site-2). It features the 12 live tees from the
Wix Stores catalog, each linking to its real product page.

## Sections
1. Announcement bar
2. Hero ("Wear the Omen.") with a gothic-arch frame that crossfades between three designs
3. Scrolling marquee of design names
4. **The Reliquary** — product grid (numbered Nº I–XII, hover zoom and "View relic")
5. **The Creed** — brand manifesto over a blurred artwork background
6. **The Rites** — four reasons to buy
7. Final call-to-action and footer

Effects: film grain, cursor "candlelight" glow, scroll reveals. All motion switches off
for visitors who set "reduce motion" on their device.

## Add it to Wix Studio
1. Open the site in the Wix Studio editor.
2. Add a page (e.g. `/gothic`), or use the homepage.
3. **Add (+) → Embed → Embed HTML** (custom code), set to **Code**, and paste all of `index.html`.
4. Stretch the element to full width and make it tall enough (about 5200px on desktop).
   Check the mobile breakpoint and set its height there too.
5. Publish.

All links use `target="_top"`, so clicking a product opens the real store page, not
a page inside the embed.

**SEO note:** Google does not credit text inside an HTML embed to your page. If you
want this page to rank, rebuild the sections with native Wix Studio elements and use
this file as the design reference (colours, fonts and copy below).

## Design tokens
| Token | Hex | Use |
|---|---|---|
| Void | `#0a0807` | Page background |
| Crypt | `#14100e` | Cards and panels |
| Bone | `#e9e1d3` | Main text |
| Bone dim | `#a89d8c` | Secondary text |
| Blood | `#8b0d14` / `#c1121c` | Buttons and accents |
| Gold | `#b8955a` | Small labels and lines |

Fonts (Google Fonts): **UnifrakturCook** (headlines), **Cinzel** (labels and buttons),
**Cormorant Garamond** (body text).

## Updating products
Edit the `products` array at the bottom of `index.html`. Each row holds the name,
subtitle, product slug and Wix image ID.
