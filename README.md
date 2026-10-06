# PESTILLENCE — Landing Page

Two pages for the PESTILLENCE Wix store (https://cazzzua.wixstudio.com/my-site-2),
both in the PESTILLENCE design system (black + one electric blue accent).

| File | What it is |
|---|---|
| `index.html` | The landing page: a mini collection of 3 tees (Last Rites, Horned Madonna, Sainted Scream) with real store photos, price, sizes and a Buy now button to each product page, plus a 3-step "how to buy" and one "see more" link. |
| `guide.html` | Plain-language guide: how the landing page connects to the store, how to set up every button in Wix Studio, the customer journey from ad to checkout, and tracking. |

## Before running ads
- The site is on the Wix **Free plan**. Wix needs a paid plan with eCommerce to take payments.
- `index.html` runs inside an HTML embed, which can't add items to the Wix cart. Its buttons open the
  real product pages. For "Add to Cart" directly on the landing page, use Wix Stores elements
  (see `guide.html`, section 2b, Option 1).
- Collection links use `/category/all-products`, `/category/t-shirts` and `/category/hoodies`.
  Open each once to confirm. They're set in one place: the `LINKS` object at the bottom of `index.html`.

## Add the landing page to Wix Studio
1. Add a page, for example `/gothic-drop`.
2. **Add Elements (+) → Embed code → Embed HTML**, choose **Code**, paste all of `index.html`.
3. Stretch it to full width and set the height (about 3800px on desktop, 4900px on mobile).
4. Publish.

All links use `target="_top"`, so they open the real store page, not a page inside the embed.

**SEO note:** Google doesn't credit text inside an HTML embed to your page. For a page that should
rank, rebuild the sections with native Wix Studio elements using the tokens below.

## Design tokens (PESTILENCE design system)
| Token | Hex | Use |
|---|---|---|
| `--p-black` | `#0a0a0a` | Page background |
| `--p-near-black` | `#101014` | Cards |
| `--p-charcoal` | `#1a1a1f` | Borders, dividers |
| `--p-washed` | `#232328` | Image placeholders, hover borders |
| `--p-neon` | `#0080FF` | The only accent: main buttons and one hero glow (keep under ~5% of the screen) |
| `--p-text` | `#e8e8ea` | Main text |
| `--p-text-dim` | `#8a8a92` | Secondary text, labels |
| `--p-text-ghost` | `#4a4a52` | Outlined display words |

Fonts (Google Fonts): **Anton** for headlines, **Space Mono** for body text and labels,
**UnifrakturCook** (bold) for the logo only. The guide uses **Archivo** for long body text.

## Updating products
Edit the `relics` array at the bottom of `index.html`: name, type, product slug, Wix image ID and the two lines of text.
