---
name: Abbyliv hair
description: A one-stylist color salon's pitch page that is itself a lock of balayage: cocoa ground, blush from her logo, hair tones from chestnut to blonde.
colors:
  cocoa: "#3a221a"
  cocoa-deep: "#2c1913"
  cocoa-lift: "#4a2c21"
  blush: "#f3e2db"
  blush-lift: "#fff4ef"
  field: "#fff8f5"
  ink: "#2b1812"
  ink-soft: "#6b4a3e"
  on-dark: "#f6e8e2"
  on-dark-soft: "#d8bdb1"
  chestnut: "#7a4a2c"
  honey: "#d9a865"
  blonde: "#ecd6a6"
  accent: "#b8643f"
  accent-ring: "rgba(184,100,63,.3)"
  field-line: "rgba(43,24,18,.45)"
  line-dark: "rgba(246,232,226,.22)"
  line-light: "rgba(43,24,18,.16)"
  error: "#a33a1f"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, Helvetica, Arial, sans-serif"
    fontSize: "clamp(52px, 15.5vw, 132px)"
    fontWeight: 900
    lineHeight: 0.88
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, Helvetica, Arial, sans-serif"
    fontSize: "clamp(34px, 9vw, 64px)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, Helvetica, Arial, sans-serif"
    fontSize: "18px"
    fontWeight: 700
    lineHeight: 1.25
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, Helvetica, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, Helvetica, Arial, sans-serif"
    fontSize: "13px"
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: "0.16em"
rounded:
  pill: "999px"
  field: "14px"
  panel: "16px"
  arch-foot: "18px"
spacing:
  gutter-phone: "16px"
  gutter-tablet: "28px"
  gutter-desktop: "40px"
  section-phone: "56px 0 64px"
  section-desktop: "96px 0 104px"
  container: "1180px"
components:
  button-fill:
    backgroundColor: "{colors.blush}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-fill-hover:
    backgroundColor: "{colors.blush-lift}"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.blush}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-line-hover:
    textColor: "{colors.honey}"
  button-send:
    backgroundColor: "{colors.cocoa}"
    textColor: "{colors.blush}"
    rounded: "{rounded.pill}"
    height: "56px"
    width: "100%"
  row-arrow-hover:
    backgroundColor: "{colors.accent}"
    textColor: "#ffffff"
    rounded: "{rounded.pill}"
    size: "40px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 16px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.cocoa}"
    textColor: "{colors.blush}"
  input:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "14px 16px"
    height: "54px"
  instagram-link:
    backgroundColor: "{colors.blush}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 24px"
    height: "60px"
  footer:
    backgroundColor: "{colors.cocoa-deep}"
    textColor: "{colors.on-dark-soft}"
---

# Design System: Abbyliv hair

## Overview

**Creative North Star: "The Lock of Balayage"**

The page is a lock of her hair. A cocoa-brown ground (never black) carries a living, touchable lock of brunette-to-honey hair in the first viewport, and the same hair keeps returning: every section boundary is a band of seven animated strands, every photo sits in an arched mirror frame, and the palette is drawn from hair itself (chestnut, honey, blonde) plus the blush of Abby's logo. Copper is the only interaction color, the tint of lightener on a brush.

Sections alternate between dark cocoa and light blush or blonde grounds, separated only by the strand seams, never by rules or cards. Type is a single system sans used two ways: very heavy, tightly tracked uppercase for headlines, and small, widely tracked uppercase for labels. Everything else is calm, roomy body copy in first person. The surface is phone-first and single-scroll; desktop widens into two-column splits without adding chrome.

**Key Characteristics:**
- Cocoa ground with blush and blonde light sections; hair tones as the only chroma besides copper.
- Heavy uppercase display (900) against a 13px tracked-caps label role; one font stack.
- Pill buttons, arched photo frames, pill chips: every interactive or framed shape is round.
- Motion is hair: a combable, paintable canvas lock and pointer-parting strand seams on one shared animation loop.
- No sticky bar, no captions, no cards; text-to-book rows are the main conversion device.

## Colors

A warm, low-key brown world lit by blush and hair-blonde, with a single copper accent reserved for touch.

### Primary
- **Cocoa** (cocoa): the page ground, the hero, the menu and work sections, the selected chip, the send button. Dark brown, never black; the theme-color meta matches it.
- **Logo Blush** (blush): light section ground (about, booking), the hero headline color on cocoa, the filled hero button and the Instagram link. Taken from the logo.

### Secondary
- **Copper** (accent): hover, focus and active only. Row arrow fill on hover, input and chip hover border, focus outline (3px, offset 3px), caret color. Its translucent ring (accent-ring) is the 3px focus glow on fields, chips and the send button.

### Tertiary (hair tones)
- **Chestnut** (chestnut): the about sign-off line; the second strand in every seam.
- **Honey** (honey): menu group headings on cocoa, the phone icon in the header, line-button hover, footer link hover, text selection.
- **Blonde** (blonde): the new-client special section ground; the lightest seam strand. Also the header number's hover color.

### Neutral
- **Cocoa Deep** (cocoa-deep): footer ground only.
- **Cocoa Lift** (cocoa-lift): the warm top-right glow of the hero radial gradient and the placeholder fill behind arched photos while they load.
- **Ink** (ink) and **Ink Soft** (ink-soft): primary and secondary text on blush and blonde.
- **On Dark** (on-dark) and **On Dark Soft** (on-dark-soft): primary and secondary text on cocoa.
- **Field** (field) and **Field Line** (field-line): input and chip fill and their 2px resting border.
- **Line Dark** / **Line Light** (line-dark, line-light): 1px row and fact dividers on dark and light grounds.
- **Blush Lift** (blush-lift): hover state of blush-filled pills.
- **Error** (error): validation message text and the dashed error border.

### Named Rules
**The Never-Black Rule.** The darkest value on the page is cocoa-deep. No #000 grounds or text; shadows may use translucent black only.

**The Copper-Is-Touch Rule.** Copper appears only in response to hover, focus, press or a caret. It never fills a resting surface or sets resting text.

**The Hair-Tone Rule.** Any new chroma comes from the hair ramp (chestnut, honey, blonde); do not introduce colors outside the brown-to-blonde range and the logo blush.

## Typography

**Display Font:** system sans stack (-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica, Arial)
**Body Font:** the same stack
**Label Font:** the same stack

**Character:** One stack, no web fonts, used at the extremes: the headline role is heavy and compressed in tracking, the label role is small and opened up. The contrast in weight and tracking does the work a second family would.

### Hierarchy
- **Display** (900, clamp 52 to 132px, line-height 0.88, tracking -0.035em, uppercase, blush): the hero headline only ("Treat yourself.").
- **Headline** (900, clamp 34 to 64px, line-height 0.95, tracking -0.02em, uppercase, balanced wrap): one per section.
- **Title** (700, 18px, line-height 1.25; 20px in the special): service names in text-to-book rows. Prices sit beside them at 800, 18px; special prices at 900, clamp 28 to 40px, tracking -0.02em, with tabular numerals.
- **Body** (400, 17px, line-height 1.55): default. Ledes and about paragraphs run 18px with measures of 30 to 40ch (hero promise 30ch, ledes 40ch, about 34em).
- **Label** (800, 13px, line-height 1.2, tracking 0.16em, uppercase): one shared role for the special's limited line, menu group headings, about fact names, form legends and field labels, and the footer tagline. Optional markers inside labels drop to 600, normal case, 0.04em tracking, ink-soft.
- **Wordmark** (700, 13px, tracking 0.22em, uppercase; 14px at desktop): "Abbyliv hair" beside the logo. The footer name is the same idea at 900, 15px, 0.2em.

### Named Rules
**The Two-Extremes Rule.** Headlines are 900-weight uppercase with negative tracking; labels are 13px uppercase at 0.16em. Do not add a middle tracked-caps size or a third weight style for headings.

**The One-Label Rule.** Every small uppercase label uses the shared 13px/800/0.16em role. New labels join that role rather than inventing a variant.

## Layout

Phone-first single column, full-bleed section grounds, content in a centered container (max 1180px) with a side gutter of 16px on phones, 28px from 600px, 40px from 1024px. Sections pad 56px top / 64px bottom on phones and 96px / 104px at desktop.

- **Breakpoints:** min-width 600px (hero buttons go side by side; work grid becomes three columns; Instagram pill shrinks to content width and centers) and min-width 1024px (two-column splits for the special, menu, about and booking sections at roughly 0.9fr/1.1fr or 1.3fr/1fr with 64 to 72px gaps; header grows; footer becomes a 2fr/1fr/1fr grid). A max-width 359px tweak tightens the wordmark.
- **Hero:** stacked on phones (header, headline, promise, buttons, then the lock at clamp 230 to 420px of small-viewport height). At desktop the lock grows to clamp 420 to 600px and pulls up under the copy with a negative top margin, so the hair sweeps into the empty right side of the headline; the copy layer passes pointer events through except on its links.
- **Work grid:** two columns with a 12px gap on phones, every second arch dropped 22px; three columns with an 18px gap from 600px, the middle column dropped 30px. The stagger is part of the system.
- **Rhythm:** form fields 26px apart; chips 8px apart; row minimum height 64px (76px in the special).

**The No-Sticky Rule.** Nothing is fixed or sticky. The header scrolls away with the hero; there is no floating call or book bar.

## Elevation & Depth

Mostly flat: depth comes from alternating section grounds and the hero's radial glow, not from stacked surfaces. Soft, downward ambient shadows appear only on objects that are physically "things": the round logo and the arched photos. Focus uses a copper ring, not elevation.

### Shadow Vocabulary
- **Logo lift** (`box-shadow: 0 2px 10px rgba(0,0,0,.25)`): the round logo in the header.
- **Arch drop** (`box-shadow: 0 14px 30px -12px rgba(0,0,0,.55)`): arched photo frames on cocoa.
- **Copper ring** (`box-shadow: 0 0 0 3px` accent-ring): focus on inputs, chips and the send button. Error state swaps it for a 3px error-tinted ring.

**The Flat-Section Rule.** Sections never become cards. A new section is a new full-bleed ground joined by a strand seam.

## Shapes

Everything a hand touches is a pill (999px): buttons, chips, the Instagram link, the circular row arrows. Text fields are softer rounded rectangles (14px); the sent-message panel is 16px. Photos are arched mirrors: a full round top over 18px bottom corners at a 3:4 aspect. Dividers are hairline 1px rules between rows. The seams are the only non-geometric edge: a wavy boundary where the next section's color fills under the middle strand.

**The Arch Rule.** Photos of her work are always in the arched mirror frame (round top, 18px foot, 3:4), never square tiles or rounded rectangles.

## Components

### Header
Logo and wordmark on the left (42px round logo, 52px at desktop), the phone number top-right: 800 weight, 15px (17px desktop), tabular numerals, a honey phone icon, hover to blonde, 44px tap target. It sits inside the hero on the same ground and is not sticky.

### Buttons
- **Shape:** pill (999px), 56px tall, 26px side padding, 2px blush border, 800 16px label with 0.02em tracking.
- **Filled (primary):** blush fill, ink text; hover lifts to blush-lift.
- **Outlined (secondary):** transparent, blush text and border; hover turns border and text honey.
- **Send:** full-width cocoa fill with blush text on the light booking ground; hover/focus adds a copper border and copper ring.
- **Press:** scale to 0.98. Transitions 0.2s on color, 0.15s on transform.
- The hero always pairs one filled and one outlined button, stacked on phones and side by side from 600px.

### Text-to-book rows
Each service is a full-width link (minimum 64px) on a hairline-divided list: name on the left (700), price right (800, tabular), and a 40px circular arrow at the end on a faint tint. On hover, focus or press, only the arrow changes: it fills copper with a white arrow. The row itself never gets a background, underline or outline; keyboard focus draws the copper outline around the arrow. Each row opens an `sms:` link with a prefilled message.

**The Arrow-Only Rule.** Row hover and focus feedback lives entirely in the arrow disc. Do not tint, underline or outline the row.

### Arched photo frames
3:4 arched frames (see Shapes) with the arch drop shadow and a cocoa-lift placeholder, images cover-cropped, not draggable, no caption. A single blush pill link to Instagram sits under the grid (60px tall, icon plus "Click to see more of my work." with the handle as a 13px ink-soft second line).

### Inputs / Fields
- **Style:** field fill, 2px field-line border, 14px radius, 54px minimum height (textarea 96px), 17px body text, ink text, warm brown placeholder.
- **Hover:** border turns copper. **Focus:** copper border plus the 3px copper ring; no default outline.
- **Error:** border turns error-red and dashed, a faint error ring, and a 15px/700 error message below.

### Chips
- **Style:** pill, 46px tall, 16px side padding, field fill, 2px field-line border, 600 16px text. Native radio or checkbox visually hidden underneath.
- **Hover:** copper border. **Focus-visible:** copper border plus copper ring.
- **Selected:** cocoa fill and border with blush text; hovering a selected chip still shows the copper border.
- **Error:** dashed error border, same as fields.

### Sent panel
After submit, a 16px-radius field-colored panel with a 2px line-light border fades up 6px (0.3s, cubic-bezier(.16,1,.3,1)) showing the composed message and two outlined 48px pills (open messages, copy).

### Footer
Cocoa-deep ground, on-dark-soft text at 16px. Wordmark (900, 15px, 0.2em), the label-role tagline, then call and text links and the Instagram link as 700-weight on-dark links with 44px tap targets, honey on hover. Bottom padding respects the safe-area inset.

### Hair lock (signature)
A full-width canvas in the hero: a lock of brunette hair whose ends warm to honey, drawn as three depth layers of strands (back strands darker, thicker and lightening least) over a solid gradient body, with tapered tips and a slow sheen band sliding along the length. Strands sway, ripple and drift across each other continuously.

- **Interaction:** dragging (or any pointer movement while touching) combs the strands apart with spring physics and paints highlights into only the strands touched; highlights grow strand by strand, cap below full bleach and slowly regrow back to the natural color. A small balayage brush (handle, metal band, flat bristle paddle with lightener on the edge) follows the pointer, offset up and right for a finger.
- **Self-painting:** after 5 seconds without touch, the brush paints by itself, stroking down the length of the hair and moving to a new section each pass.
- **Hint:** a 13px on-dark-soft line bottom-right ("Drag across the hair to paint highlights") becomes "That's balayage, by hand." on first touch, then fades out.
- **Phone vs desktop:** fewer strands and samples under 700px wide; at 1024px the lock stays low under the copy and sweeps up to the right, and the system cursor hides over it.
- **Tunables (top of the hair IIFE):** `STRANDS_PHONE` / `STRANDS_DESK` and `SAMPLES_PHONE` / `SAMPLES_DESK` (density), `SWELL`, `RIPPLE` (motion speeds), `BRUSH` (brush radius as a share of lock height), `LIFT`, `GHOST_LIFT`, `REGROW` (paint-in and fade-back rates), `PUSH`, `SPRING`, `DAMP` (combing physics), `IDLE_GHOST` (seconds before self-painting), `RAMP` (root-to-end natural color stops), `LIFTED` (highlight color), `LIFT_MAX` (strongest highlight), `LAYERS` (per-layer dim, width, alpha, lift), `TILT_PHONE` / `TILT_DESK` (how much the lock rises toward its ends), `GHOST_PUSH` (how hard the self-painting brush parts hair), `SHEEN`, `TIP` (sheen strength, taper length).

### Strand seams (signature)
Every boundary between two section grounds is a 56px band (80px at desktop) of seven SVG hair strands running chestnut to blonde, each with its own wave, speed and direction; the next section's color fills in under the middle (honey) strand, so the boundary itself is a strand. Strands part under the pointer with the same spring feel as the hero, and each seam is phase-shifted from the last.
- **Tunables (top of the seams IIFE):** `STEP` (point spacing), `VW`, `VH` (viewBox), `SPEED` (wave speed), `MID` (index of the strand the next color fills under), `REACH`, `PUSH`, `SPRING`, `DAMP` (pointer parting), `STRANDS` (per-strand color, height, amplitude, frequency, speed, width, opacity).

### Motion system
One shared requestAnimationFrame loop drives the lock and every seam. Each subscriber is watched by an IntersectionObserver (80px margin) and only runs while near the viewport; the loop stops entirely when nothing is visible, and a synchronous on-load visibility check covers in-app browsers that report the observer late. Frame delta is capped at 50ms. Under `prefers-reduced-motion: reduce`, the lock renders one still frame with highlights already painted on a third of the strands (redrawn on resize, hint hidden, no brush), seams render once and never animate, smooth scrolling, button and arrow transitions and the sent-panel entrance are disabled.

**The Shared-Loop Rule.** Any new animation subscribes to the shared loop and pauses off screen; no component starts its own rAF.

**The Still-Frame Rule.** Every animated element has a meaningful static state under reduced motion; never just remove it.

## Do's and Don'ts

### Do:
- **Do** keep cocoa as the ground and alternate light sections (blush, blonde) joined by strand seams.
- **Do** keep copper for hover, focus and press only, with the 3px copper outline or ring.
- **Do** put the phone number in the header top-right and nowhere else in the first screen.
- **Do** frame every work photo in the arch and place the single Instagram link directly under the photos.
- **Do** use text-to-book rows (sms links with a prefilled message) for any priced service, with arrow-only hover.
- **Do** keep tap targets at 44px or more and pair hero buttons as one filled, one outlined pill.
- **Do** run new motion through the shared loop and give it a reduced-motion still frame.

### Don't:
- **Don't** add a sticky or fixed header, call bar or book bar.
- **Don't** repeat the phone number elsewhere in the first viewport (hero copy, buttons).
- **Don't** add an email address or email link anywhere.
- **Don't** caption the work photos; the alt text carries the description.
- **Don't** use pure black, or colors outside the hair tones, blush and copper.
- **Don't** separate sections with rules, cards or straight edges; use a strand seam.
- **Don't** give rows a hover background or underline.
