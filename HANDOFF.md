# Abbyliv hair — handoff at ~60%

**Live:** https://10elizabethbell.github.io/abbylivHair/ · **Repo:** https://github.com/10elizabethbell/abbylivHair · **Built:** 2026-10-18 from Muse brief of 2026-10-18 (Facebook group sweep, new-client-special ad)

## What's built
- One phone-first page (`index.html`, photos in `img/`): header (her Instagram logo + "ABBYLIV HAIR", 908-839-6941 top-right as `tel:`), hero "TREAT YOURSELF." with a promise line and two buttons (Book an appointment → form, New-client special → list), new-client special, the menu with her published prices, About Abby (15 years, hours, booking, South Manalapan), My work (6 arched photos + "Click to see more of my work." → Instagram), booking form, footer.
- **World:** her balayage. Cocoa-brown ground (not black), blush from her logo, hair tones chestnut → honey → blonde, copper only on hover/focus.
- **Signature:** a canvas lock of brunette-to-honey hair across the hero. Finger or mouse combs it (strands part and spring back) and paints highlights that fade back after a few seconds. Drags work up, down and sideways on phones. Until someone touches it, a flat balayage brush paints streaks along the mid-lengths by itself. The visitor's pointer becomes the brush (offset above the finger on touch). First stroke swaps the hint to "That's balayage, by hand."
- **Seams** between sections are seven hair strands in the same colors; they sway and part when a finger or mouse passes.
- **Booking (the free fix for her dead "Book Now" buttons):** every special and menu row is a pre-written text to her (`sms:` with the service named). The form (name, service, optional days/time/notes) composes one text and opens Messages; if Messages doesn't open, a fallback shows the message with Open messages / Copy buttons.
- Tunables at the top of each IIFE: `hair()` (strand counts, `SWELL`/`RIPPLE` speeds, `BRUSH`, `LIFT`, `GHOST_LIFT`, `REGROW`, `LIFT_MAX`, `TILT_*`, `SHEEN`, `TIP`, `IDLE_GHOST`), `seams()` (`SPEED`, `REACH`, `PUSH`, strand list).

## Assumptions I made
- **Voice is first person ("I")** — the old site signs off "by Abby" and only she is named. Hero promise "In my chair you get my full attention, from the first foil to the last curl." is my wording, not hers; the About copy is assembled from her own phrases (specialty list, "top-of-the-line products", "look—and feel—like a million dollars", "pamper yourself").
- **Colors:** blush from her Instagram logo; brown/honey from her hair work; copper accent chosen. Her site/logo give no other brand colors.
- **Logo:** only a 100px Instagram avatar exists. Used at 42–52px in the header and for favicon/home-screen icon (the 180px icon is upscaled, slightly soft).
- **"Color correction — Text me"**: her menu heading is "color / color correction" with no correction price, so it's a text-for-price row.
- **"Cutting" renamed "Haircut"** to match the special and the form.
- **Instagram stands in for Facebook** for "see more of my work": there's no business Facebook page (ad posted from her personal profile). IG @abbylivhair verified live 2026-10-18 (112 posts).
- **Audience:** general adult clientele, not 40+, so full motion is on.
- Photos: 6 of the 8 work photos on her Wix site (backs of heads, no faces). Copper photo re-cropped to remove a handbag chain.

## Placeholders and gaps
- No email (none exists) → footer has none.
- No street address published, per brief (South Manalapan only).
- No reviews anywhere → none on the page.
- No Google Maps listing, no Facebook business page.
- How long the new-client special runs ("Limited Time!") is unknown — the section says "limited time" with no end date.
- Her old site's "Book Now" buttons: the Wix pages render client-side and a plain fetch showed no booking flow; not verified in a real browser.

## Questions for the owner
- When does the new-client special end? Should it come down after?
- Prices for keratin, GK smoothing and color correction?
- A higher-res logo file, and a photo of you (a portrait is the strongest trust signal for a one-stylist salon)?
- Before/after pairs? (They'd unlock before/after sliders in the work section.)
- Any client reviews you're happy to quote word for word?
- Is the hero promise ("my full attention, from the first foil to the last curl") true to how you work? Anything you'd rather say?
- Do you want people texting, calling, or both? (The page leans on texting since the ad says "call or text".)

## Ideas not built (yours to pick)
- **Runner-up world:** a color bowl and tint brush — swirl lightener and glaze in a bowl you can stir; same palette.
- Canvas seams: rebuild each seam with the hero's hair renderer so they're thin combable locks (overdrive idea; skipped for phone frame budget).
- Before/after sliders once she sends pairs.
- A small "special ends <date>" line once she gives a date.
- A booking page (`book.html`) with the same lock divider, if she wants a separate link to post.
- Atkinson Hyperlegible or a script face echoing her logo for the wordmark only (house rule is system fonts; noted in case you want it).
- On desktop the upper right of the hero is still a bit empty; raising `TILT_DESK` (0.34 → ~0.42) fills it but needs a check that strands stay clear of "YOURSELF."

## Not verified
- Real-device touch on iPhone/Android inside Facebook's in-app browser (verified with simulated touch and mouse sweeps in headless Chrome only).
- Real SMS handoff on iOS and Android (`sms:+19088396941?&body=…` decoded correctly in the probe).
- Frame rate on older phones (260 strands × 64 samples on phones; not measured — headless timing probe never returned).
- WebKit/Safari rendering (Chrome only).
- Impeccable detector ran in its normal (non-degraded) mode; the critique ran single-context (one reviewer instead of two separate ones).
- No seed key: Impeccable's concept roll / decision page was skipped because the build is unattended.
