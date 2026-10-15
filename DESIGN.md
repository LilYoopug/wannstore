---
name: wannstore
description: Fillmore handbill storefront for Indonesian game-boosting services — one continuous printed sheet, split-fountain ink on newsprint.
colors:
  vermilion: "#c0321c"
  marigold: "#f5d64c"
  midnight: "#1b2a52"
  cream: "#f3ead8"
  cream-deep: "#ece0c8"
  ink: "#1a1208"
  ink-soft: "#4a3d28"
  ink-faint: "#665534"
typography:
  display:
    fontFamily: "Alfa Slab One, Georgia, serif"
    fontSize: "96px"
    fontWeight: 400
    lineHeight: 1
    letterSpacing: "0.01em"
  stencil:
    fontFamily: "Bebas Neue, Arial Narrow, sans-serif"
    fontSize: "clamp(28px, 5vw, 44px)"
    fontWeight: 400
    lineHeight: 1.05
    letterSpacing: "0.06em"
  hook:
    fontFamily: "Newsreader, Georgia, serif"
    fontSize: "clamp(22px, 3.1vw, 44px)"
    fontWeight: 600
    lineHeight: 1.16
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Newsreader, Georgia, serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: "normal"
  body-sm:
    fontFamily: "Newsreader, Georgia, serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: "normal"
  item:
    fontFamily: "Newsreader, Georgia, serif"
    fontSize: "17px"
    fontWeight: 600
    lineHeight: 1.3
    letterSpacing: "normal"
  price:
    fontFamily: "Bebas Neue, Arial Narrow, sans-serif"
    fontSize: "22px"
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: "0.04em"
  price-sm:
    fontFamily: "Bebas Neue, Arial Narrow, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: "0.04em"
  banner:
    fontFamily: "Bebas Neue, Arial Narrow, sans-serif"
    fontSize: "clamp(24px, 4vw, 36px)"
    fontWeight: 400
    lineHeight: 1.05
    letterSpacing: "0.06em"
  button:
    fontFamily: "Bebas Neue, Arial Narrow, sans-serif"
    fontSize: "20px"
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: "0.1em"
  label:
    fontFamily: "Newsreader, Georgia, serif"
    fontSize: "14px"
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: "0.02em"
  sub:
    fontFamily: "Newsreader, Georgia, serif"
    fontSize: "13px"
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: "0.01em"
  micro:
    fontFamily: "Newsreader, Georgia, serif"
    fontSize: "11px"
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: "0.06em"
rounded:
  ink: "0px"
  stamp: "4px"
  circle: "50%"
spacing:
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "48px"
components:
  order-stub:
    backgroundColor: "{colors.vermilion}"
    textColor: "{colors.cream}"
    typography: "{typography.stencil}"
    rounded: "{rounded.ink}"
    padding: "14px 32px"
  order-stub-hover:
    backgroundColor: "{colors.vermilion}"
    textColor: "{colors.cream}"
  pt-order:
    backgroundColor: "{colors.cream}"
    textColor: "{colors.ink}"
    typography: "{typography.stencil}"
    rounded: "{rounded.ink}"
    padding: "6px 14px"
  pt-order-hover:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.cream}"
  billing-border:
    backgroundColor: "{colors.midnight}"
    textColor: "{colors.cream}"
    typography: "{typography.label}"
    rounded: "{rounded.ink}"
    padding: "10px 24px"
  game-stamp:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.cream}"
    typography: "{typography.stencil}"
    rounded: "{rounded.ink}"
    padding: "8px 24px"
  custom-order:
    backgroundColor: "{colors.midnight}"
    textColor: "{colors.cream}"
    typography: "{typography.stencil}"
    rounded: "{rounded.ink}"
    padding: "32px 24px"
---

## Overview

wannstore is a gig poster for a one-night-stand era of Indonesian game boosting. Every service is a dated bill, every price is a billing line, and the whole storefront is one continuous printed sheet you read like a handbill. The category default — a dark gamer shop with neon accents and generic product cards — is refused. Nothing floats; everything is inked.

The visual world is **Fillmore Handbill**, rolled from concept-seed `daa8e700` and raised by a challenger donation: the bill IS the page. There is no poster sitting behind a website, no nav bar floating over content, no separate hero section. The sheet begins with a billing border carrying the shop's identity, opens with an arc-warped wordmark, and scrolls through services as ruled billing tables until a closing rule. Remove all content and you still see a 1966 Fillmore bill: flat saturated inks on cream, hand-set type, no glass, no decorative gradients.

**The bill is a document, not a brochure.** Its authority comes from the ledger: published fixed prices in ruled tables, game names stamped like bill headers, a pen-circle on the row you are considering. The reader's belief to win is "this shop is real, fast, and transparent — prices aren't hidden behind 'chat for quote.'"

## Colors

Four inks on one ground. Color is rationed; the page is mostly ink-on-cream.

- **Vermilion** `#c0321c` — the primary ink. ORDER stubs, price figures, the Wuthering Waves bill header, the pen-circle, and the identity dot. (Darker than the reference `#e8452c`; see Do's and Don'ts for the contrast reason.)
- **Marigold** `#f5d64c` — the second ink. Used once, on the custom-order stub, so it reads as a highlight rather than a system color.
- **Midnight** `#1b2a52` — the identity ink. The billing border, the Reverse 1999 bill header, the custom-order banner, and focus rings.
- **Cream** `#f3ead8` — the newsprint ground and the text color on every dark ink surface. `cream-deep` `#ece0c8` is the scrollbar track only.
- **Ink** `#1a1208` — body text and every rule. `ink-soft` `#4a3d28` is the thin rule and secondary text; `ink-faint` `#665534` is the tertiary label color.

No glass, no blur, no gradient-as-decoration. The head's atmospheric wash (`radial-gradient` blobs at 12% opacity) is the single exception and exists only to give the sheet a printed-registration softness behind the wordmark.

## Typography

Three faces, each with one job. No system display font stands in for the display voice.

- **Alfa Slab One** (`--font-display`) — the wordmark only, arc-warped along an SVG `textPath`. It never appears in the body. Its slab weight is the bill's masthead.
- **Bebas Neue** (`--font-stencil`) — the bill's stencil voice: bill headers, price figures, ORDER stubs, section counts. Condensed caps with wide tracking. Prices are set in it so a column of figures reads as a ledger.
- **Newsreader** (`--font-body` / `--font-ui`) — everything read as text: body copy, item names, sub-labels, footer. A serif workhorse. The `--font-ui` role points at the same face on purpose; the world has no fourth font.

**Scale:** body 17px/1.6, `body-sm` 16px, item names 17px/600, sub-labels 13px, micro 11px. Stencil bill headers `clamp(28px, 5vw, 44px)`; price figures 22px (18px on mobile); the hero hook `clamp(22px, 3.1vw, 44px)`/1.16 with `-0.01em`. Every step is a real role, not a 1px increment — the scale runs 11 → 13 → 14 → 16 → 17 → 18 → 20 → 22 before the clamps. Tracking is positive or neutral throughout except the hook's `-0.01em`; the letterpress voice is hand-set, not tightened. No tracking below `-0.01em` anywhere.

## Layout

One continuous sheet, `max-width: 1200px`, centered, with 3px ink borders running down both edges so the page reads as a printed object rather than a fluid web page. The sheet never breaks into light/dark bands.

Vertical grammar, top to bottom: **billing border** (identity strip) → **head** (the bill pasted on a wall) → **bill sections** (game header stamp, then price groups as ruled tables) → **character gallery** per game → **custom-order banner** → **closing rule** (footer).

The head is the one place the sheet's flatness breaks: a cream card with a 3px ink border and a `10px 10px 0 rgba(26,18,8,0.28)` registration shadow sits inside a full-bleed vermilion field, so the bill reads as pasted on a wall. Inside the card: a topline of identity meta over a thin rule, the arc-warped wordmark spanning the card width, then a two-column lower zone — copy (hook, CTA row, trust bullets) at `1.55fr` against a framed poster still at `1fr`. The poster is height-capped (`clamp(250px, 26vw, 360px)`) and object-positioned to `50% 22%` so it never outgrows the copy column. Below 640px the lower zone collapses to one column and the poster follows the copy.

There is no navigation bar. Sections are found by their stamped game headers, which are full ink blocks — the same device a handbill uses to separate acts. Price tables are `border-collapse` ruled rows, not cards; the row hover tints to `rgba(192,50,28,0.04)` and the pen-circle inks in. Body measure stays in the 65–75ch range inside the tables.

Mobile collapses to a single column at 640px: the billing border wraps and centers, table padding tightens to `10px 6px`, price figures drop to 18px, and the character grid goes two-up. `overflow-x: hidden` on the sheet guards the inked edges.

## Elevation & Depth

The world is **flat**. There is no soft shadow system; depth is not the tool. The two shadow values that exist are both letterpress registration offsets, and both are hard-edged:

- **ORDER stub:** `4px 4px 0 var(--ink)`, growing to `6px 6px 0` on hover and collapsing to `1px 1px 0` on press. This is a print registration offset — the plate slightly out of alignment — not a floating card.
- **Game headshot / stamp:** `4px 4px 0 rgba(26,18,8,0.2)` and `3px 3px 0 rgba(26,18,8,0.2)`, a softer registration bleed.

Elevation between surfaces is carried entirely by **ink rules** (`2px solid var(--ink)`) and **color blocks**, never by blur. A section is distinguished by its stamped header block, not by lifting it off the page. Because the world is genuinely letterpress, the craft floor's ban on hard offset shadows outside a neobrutalist world does not apply — the offset is the chosen depth device, not a borrowed costume.

**Motion — the sheet prints itself.** There is one authored moment, and it is the world's own metaphor: ink settling onto paper as the reader moves down the bill. Elements are **visible by default**; JS opts them into the reveal only when motion is welcome and `IntersectionObserver` exists, so no-JS and `prefers-reduced-motion` both ship a fully printed sheet. The reveal is `opacity 0 → 1` + `translateY(14px) → 0` + `blur(4px) → 0` over `0.7s cubic-bezier(0.16, 1, 0.3, 1)` — an exponential ease-out, reaching past transform and opacity into blur. Price rows stagger 45ms apart within their table (capped at 10 steps) so a category inks in like a line being printed. The game stamps use the same system with a registration snap (`scale(1.06) → 1`). The wordmark impresses once on load via the `impress` keyframe. Nothing else moves; the pen-circle on hover is the only other authored motion.

## Shapes

Ink has square corners. The radius vocabulary is essentially zero:

- **Stamps, stubs, tables, banners:** 0px. Hard inked edges throughout.
- **Game icons inside stamps:** 4px — the one place a corner softens, because it is an image in a frame.
- **Pen-circle:** a 50% ellipse drawn in SVG, `stroke-dasharray: 400` animating to `0` over 0.5s — the signature "circled in biro" mark.
- **Identity dot:** a 5px circle in the billing border, the only ornament.

Borders do the work a radius would on a softer system: every container is defined by a 2px or 3px ink rule. The `--rule` token is `2px solid var(--ink)`; `--rule-thin` is `1px solid var(--ink-soft)`.

## Components

**Billing border** — the identity strip. Midnight fill, cream text at 14px/500, uppercase, `0.06em` tracking. Carries the wannstore mark with a vermilion dot, the WhatsApp number, and the TikTok handle, each as a link with a cream underline at 35% that solidifies on hover. Wraps and centers under 640px.

**Head card** — the bill pasted on a wall. A cream card, 3px ink border, `10px 10px 0 rgba(26,18,8,0.28)` registration shadow, floating in a full-bleed vermilion field with `clamp(14px, 3vw, 40px)` of field showing around it. Its topline is identity meta (mark with vermilion dot, tagline, promise) over a thin rule at 14px/500 uppercase. Then the arc-warped wordmark, then the two-column lower zone. It is the only place in the sheet that lifts off the ground.

**Poster stills** — the hero's image column. The two game key arts, stacked, each in a 3px ink frame with a `5px 5px 0 rgba(26,18,8,0.25)` registration bleed, `aspect-ratio: 16/9`, `object-fit: cover`. Captioned below in stencil 14px, left-aligned. Using both game covers rather than one character keeps the hero balanced and tells the visitor both games are sold.

**Floating order sticker** — the decal pasted on the sheet. A fixed cut-out in the bottom-right corner: the chibi mascot in her speech bubble, `AYO ORDER!` across the top, drifting on a 4.6s ease-in-out loop (`translateY(0) → -12px`, `rotate(-2.2deg) → 2.2deg`) with a `drop-shadow` beneath so it reads as stuck slightly proud of the paper. It pauses its drift and lifts on hover. The whole sticker is the link — one tap opens WhatsApp with `mau pesan` pre-typed. A 20px close button sits at its top-right: transparent fill, 1.5px ink outline at 55%, ink glyph, turning vermilion on hover. It appears on hover/focus (always visible on touch, where there is no hover). Pressing to order sends it up and away; closing sends it down and away. Closing is **session-only** — a refreshed page pastes the sticker back.

**Category roundel** — the printer's dingbat. Every price-group heading opens with a 36px circular badge: 2px ink border, vermilion fill (midnight inside the Reverse 1999 section), holding a 20px drawn SVG mark in `currentColor` at `1.8` stroke. One distinct mark per category — star (Astrite), bolt (Build), map (Explore), document (Quest), trophy (Challenge), book (Story), diamond (Reflection), chest (Rawkun), droplet (Riveries), figure (characters). Drawn geometry, never emoji or an icon font.

**Character carousel** — the revolving drum. Both games present their cast on a carousel rather than a grid: the roster is the game's selling point and deserves the full stage. One large plate holds a single character; behind it a dashed printer's **registration ring** turns slowly (44s) with two vermilion dots riding it, so the assembly reads as a plate on a rotating barrel.

The drum **turns on its own, continuously** — no arrows, no thumbnail rail, no dots. It is a display, not a widget: the motion is the point, so it never pauses on hover or focus. Only a hidden tab stops the timer. Slides swap on a 3D flip (`rotateY(38deg) scale(0.82)` → `0 / 1`, expo ease-out 0.65s) with the outgoing slide rotating the opposite way, so it turns like a drum rather than crossfading. A **caption plate** — ink block, stencil name in cream, marigold counter — names the current character.

Two stage variants, because the source art differs:

- **Square stage** (Wuthering Waves, 620px max): `aspect-ratio: 1`, `object-fit: cover`, caption plate overlaid on the frame's foot.
- **Tall stage** (Reverse 1999, 430px max, `.cc-stage-tall`): `aspect-ratio: 3/4`, `object-fit: contain`. The caption becomes a printed strip **below** the frame instead of an overlay, because these figures run to their feet and an overlaid plate would cut them off at the ankles.

`prefers-reduced-motion` stops both the rotation and the ring — the drum becomes a still plate.

**Character grid** — retained as a component for any future set whose art suits a static grid (`char-grid-tall`, `aspect-ratio: 3/4`, `object-fit: contain`, `auto-fill, minmax(180px, 1fr)`). 3px ink frames with a `3px 3px 0 rgba(26,18,8,0.2)` registration bleed, lifting on hover. No gallery currently uses it.

## Do's and Don'ts

**Do**

- Keep the cream newsprint ground and ink-on-cream text. The sheet is the world.
- Set every price in Bebas Neue vermilion, right-aligned in a ruled row, so a column of figures reads as a ledger.
- Use the hard offset registration shadow on stubs and stamps. It is the world's depth device.
- Route every product CTA through `wa.me/6289527560809` with the order pre-typed in the message.
- Reuse the billing border for identity and the game stamp for section headers at any new surface.
- Keep the arc-warped Alfa Slab One wordmark at the head only; the body stays straight and legible.

**Don't**

- Don't introduce a nav bar, glass, or blur. The sheet scrolls as one continuous print.
- Don't put prices in cards. Billing lines in ruled tables are the grammar.
- Don't use marigold as a system color. It earns its place once, on the custom-order stub.
- Don't set body text in the display or stencil face, or the stencil face in body copy.
- Don't add a kicker or eyebrow above a heading. The stamped heading carries its own weight.
- Don't use `#e8452c` for the vermilion. The reference ink failed WCAG AA at 3.3:1 on cream; `#c0321c` clears 4.5:1 in both directions while staying vermilion.
- Don't gray out secondary text on an ink surface — tint it from the surface's own hue.
