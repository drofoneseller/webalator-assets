# Webalator — logo & icon handoff

New brand mark ("Ripple") for webalator.com, colored to the site's existing palette.
Nothing about the site's layout, type or colors needs to change. This is a logo swap plus icon files.

## The mark

A water drop above a shallow ripple line. Meaning: one drop lands and the effect keeps
widening — the site goes live, the listing gets fixed, the phone gets answered, and the
reach spreads past the thing the customer paid for. The drop is the work, the ring is the return.

Geometry (viewBox 0 0 100 100), do not redraw:

    drop:   M50 8 C 66 34 74 46 74 56 A 24 24 0 0 1 26 56 C 26 46 34 34 50 8 Z
    ripple: M18 86 A 34 12 0 0 0 82 86   (stroke-width 6, round cap)

## Colors (sampled from the live site)

    Forest      #234034   the drop, headings
    Cream       #F5EDE3   the ground
    Gold        #B08D4F   the ripple, eyebrow labels
    Terracotta  #C0492A   CTA buttons ONLY
    Stone       #8A7A62   descriptor line, muted text

Rule: the terracotta drop variant exists but must never appear on a screen next to a
terracotta CTA button. On cream, use the forest drop with the gold ripple.

## Site changes

1. Header — replace the current round green badge containing "w" with
   `assets/webalator-badge-forest.svg`. Same size, same position, same green circle.
   The wordmark text beside it stays exactly as it is (the site's existing serif).

2. Footer — same swap.

3. Favicons and app icons — replace the current files and use these tags in `<head>`:

```html
<link rel="icon" href="/favicon.svg" type="image/svg+xml">
<link rel="icon" href="/favicon-32.png" sizes="32x32">
<link rel="apple-touch-icon" href="/apple-touch-icon.png">
<link rel="manifest" href="/site.webmanifest">
<meta name="theme-color" content="#234034">
```

   `site.webmanifest` in this package is already set to theme #234034 / background #F5EDE3.
   Icon paths in it assume the files sit at the web root; adjust if they go in `/assets/`.

4. Social / OG image — use `webalator-badge-forest-512.png` or the cream mark on a
   forest ground. No new asset needed unless you want a wide 1200×630 card; ask and it can be made.

## Files

    webalator-mark-forest.svg          primary mark, for cream/light grounds
    webalator-mark-cream.svg           reverse mark, for forest/dark grounds
    webalator-mark-onecolor-forest.svg single color — vinyl, embroidery, stamps
    webalator-mark-terracotta.svg      alternate, restricted use (see rule above)
    webalator-badge-forest.svg         round green badge + cream drop — the header mark
    webalator-badge-terracotta.svg     round terracotta badge variant
    webalator-mark-forest-1024.png     transparent PNG
    webalator-mark-cream-1024.png      transparent PNG
    webalator-badge-forest-512.png     round badge PNG
    favicon.svg                        rounded forest tile + cream drop
    favicon-16/32/48/64.png            tab icons (16–48 omit the ripple for legibility)
    apple-touch-icon.png               180×180, opaque, square
    android-chrome-192/512.png         opaque, square
    maskable-512.png                   Android maskable, mark at 45% safe zone
    site.webmanifest

## Clear space and minimum size

- Clear space on all sides equals the full height of the drop.
- Mark: never below 24px on screen or 8mm in print.
- Lockup: never below 120px wide; below that drop the "WEB & GROWTH STUDIO" descriptor.
- Below 32px use the drop without the ripple — the favicon files already do this.

## Type

The wordmark is set in the site's existing display serif — do not substitute another face.
The descriptor line is the site's body sans, uppercase, 0.26em letter-spacing, in Stone #8A7A62.
No new fonts need to be loaded.

## Don'ts

- No gradient, bevel, glow or drop shadow on the drop.
- Do not rotate, flip, stretch, or recolor the ripple to forest on a cream ground.
- Do not curve, condense or re-set the wordmark.
- Do not place the mark on a photo without a cream or forest plate behind it.
