# lanternwp

## What this is
The foundational theme for the Tearmann product system — the base that the free pattern library, paid template packs, and client builds all extend from. Built by Tearmann Designs.

## Who it's for
- **DIY builders** — non-technical or lightly technical users who need to launch and customize a site without writing code. They work primarily in the block editor and Site Editor patterns.
- **WP developers** — freelancers and small agencies who want a clean, well-documented PHP foundation they can extend, override, or build client work on top of without fighting the theme.

The theme has to genuinely serve both without compromising either — DIY-friendly customization on top of a developer-sane codebase underneath.

## Architecture
- **Standalone theme** (not a child theme of Kadence or anything else)
- **Hybrid approach:** classic PHP templates for markup and structure, with `theme.json` registered to define the design system and enable block pattern/style support
- Block-locking and limited Global Styles access configured in `theme.json` so DIY builders can customize safely without breaking contrast or typography

## Minimum supported versions
- **WordPress:** 6.8 (second-to-latest major release)
- **PHP:** 8.4 (second-to-latest branch)

## What this theme must never compromise on

**Accessibility (WCAG 2.1 AA)**
Every release must pass the Tearmann Verified accessibility checklist in full — semantic landmarks, keyboard navigation, contrast ratios, visible focus states, and properly labeled forms are non-negotiable, not optional polish.

**Performance (Core Web Vitals)**
Every release must meet LCP < 2.5s, INP < 200ms, and CLS < 0.1 on mobile. Features that compromise these thresholds get redesigned or cut, not shipped with a caveat.

When accessibility and performance work pull in different directions, the resolution is to solve for both — not trade one for the other. A feature that isn't accessible or isn't fast doesn't ship.

## What success looks like
A DIY builder can launch a fully accessible, fast site without touching code. A developer can extend the theme without fighting undocumented behavior. Both walk away trusting the Tearmann name means "accessible and fast," verifiably.
