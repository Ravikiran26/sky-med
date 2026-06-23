# REACT Air Ambulance – Sky-Med Project

Single-page marketing website for **REACT (Rapid Emergency Aerocare Team)**, operating under **NL Curantis International Pvt Ltd**.

Domain: **reactairambulance.com**

## Project structure

```
sky-med/
└── index.html   # Self-contained: all CSS in <style>, all JS in <script>
```

## Brand

| Token | Value |
|-------|-------|
| Company | NL Curantis International Pvt Ltd |
| Brand | REACT (Rapid Emergency Aerocare Team) |
| Domain | reactairambulance.com |
| Emergency line | 1800-NIAMS-911 (to be updated) |
| WhatsApp | https://wa.me/918006426779 |
| Email | ops@nlcurantis.in |

## Design system

```css
--navy:  #04111f   /* page background */
--panel: #071628   /* card / panel background */
--red:   #e02828   /* primary accent, emergency */
--red2:  #ff4444   /* lighter red for glows */
--sky:   #1565c8   /* secondary blue */
--skylt: #4a9eff   /* light blue highlights */
--white: #eef3ff   /* body text */
--muted: #6a8aaa   /* secondary text */
--green: #3ddc84   /* success / WhatsApp / live status */
```

| Role | Font |
|------|------|
| Headings / numbers | Bebas Neue |
| Labels / tags / mono | Space Mono |
| Body copy | Barlow 300/400/500 |

## Dependencies (CDN, no npm)

- Google Fonts – Bebas Neue, Space Mono, Barlow
- Three.js r128 – particle background (disabled on mobile ≤920px)
- GSAP 3.12.2 + ScrollTrigger – hero stagger, scroll reveals, plane animation

## Sections

1. **Navbar** – fixed, backdrop-blur on scroll, hamburger ≤920px, pulsing EMERGENCY button
2. **Hero** – "WHEN LIVES DEPEND ON SPEED" word stagger, radar with sweep + plane animation, status bar
3. **Stats bar** – 1800+ missions, 18 min response, 32+ cities, 99.8% success (animated counters)
4. **Certifications ticker** – infinite CSS marquee
5. **Services** – 6-card 3×2 grid, red border slide-up on hover, GSAP stagger reveal
6. **How It Works** – alternating left/right timeline, 4 steps, ScrollTrigger slide-in
7. **Fleet** – 3 cards: Helicopter / Turbo Prop / ICU Jet, blue glow hover
8. **Coverage** – simplified India SVG map with animated route dashes and pin pulses
9. **Emergency CTA** – 4 sonar rings, glowing phone number, call + WhatsApp buttons
10. **Footer** – 4-column grid, DGCA Licensed badge, green status dot

## Mobile behaviour (≤920px)

- Hamburger nav replaces link bar
- Three.js particles disabled
- Radar hidden
- All grids collapse to single column
- Timeline switches to left-rail layout

## Floating buttons (always visible)

- Red pulsing **Emergency Call** (top)
- Green **WhatsApp** (below)
- Mobile ≤620px: icon-only (48×48px)
