# Makena Paint Co — Website SPEC v2

## Concept
A warm, trustworthy painting company website that converts homeowners. Not a design agency template — feels like a real, established, proud Gauteng painting contractor. Think Dulux editorial meets a premium local builder. Warm cream spaces, rich paint colours, portfolio you want to scroll through.

## Design Language

**Aesthetic:** Warm editorial paint house — cream backgrounds like a fresh coat of paint, terracotta and forest green accents that feel like paint on a colour card. Clean, spacious, confident. NOT dark, NOT corporate blue.

**Color Palette:**
- Background: `#FAF7F2` (warm cream — like fresh ceiling paint)
- Surface: `#F2EDE4` (slightly warmer, slightly darker cream)
- Surface 2: `#EBE3D7` (card backgrounds)
- Primary: `#B85C38` (terracotta/rust — main CTA colour)
- Secondary: `#2D5A47` (deep forest green — secondary accent)
- Gold: `#C9963C` (warm gold — highlights)
- Text: `#2C2416` (warm dark brown — body text)
- Text light: `#6B5D4D` (warm medium brown)
- Muted: `#9A8B7A` (warm grey-brown)
- Border: `#E0D8CC` (warm grey)
- White: `#FFFFFF`

**Typography:**
- Display: 'Cormorant Garamond' (700) — elegant serif headings, feels premium but warm
- Body: 'Plus Jakarta Sans' (400, 500, 600) — clean, friendly, modern, trustworthy
- Label: Plus Jakarta Sans 600, uppercase, tracked — section labels

**Motion:**
- CSS transitions throughout (no GSAP dependency for core)
- Scroll reveals: fade + slight upward translate (CSS animation class toggled by Intersection Observer)
- Hover effects: subtle lifts, colour shifts, smooth transitions
- No heavy Three.js — replace with CSS paint gradient backgrounds

**Visual Assets:**
- Hero: Full-bleed Unsplash warm painted interior photo
- Portfolio: Real painted room photos (Unsplash)
- Colour swatches: CSS gradients (no images needed)
- Icons: Custom inline SVG — simple, clean, 2px stroke
- Decorative: Subtle paint stroke SVG shapes, colour gradient backgrounds on alternating sections

## Layout & Structure

```
[NAV] — white bg, logo left, links centre, phone right
[HERO] — full-bleed painted room photo, left-aligned headline, CTA overlay
[TRUST BAR] — 4 stats on cream bg: Homes, Years, Satisfaction, Areas
[PORTFOLIO] — 3×2 grid, large images, hover reveals project name + category
[COLOUR STRIP] — full-width warm terracotta gradient with quote text
[SERVICES] — 3 cards with colour swatches and icons
[ABOUT] — split: stats left, story right
[TESTIMONIALS] — 3 cards on surface bg
[AREAS] — pill tags on cream bg
[FAQ] — accordion on surface bg
[CONTACT] — split: form left, info + colour swatch right
[FOOTER] — warm dark bg (--text colour), cream text
```

## Features

**Navigation:** Sticky white nav. Logo left (Makena Paint Co.), links centre, phone right. Subtle shadow when scrolled. Mobile: hamburger → slide-in overlay.

**Hero:** Full-width warm painted interior photo. Left-aligned text overlay with headline and CTA. Paint colour gradient at bottom.

**Portfolio:** 6-item grid, images are beautiful painted rooms/interiors. Hover: overlay with project name and type. Clean and inspiring.

**Trust Bar:** 4 numbers with labels. Cream background. Animates count-up on scroll.

**Services:** 3 cards — each with a colour swatch header, icon, title, description. Subtle shadow on hover.

**Contact Form:** Fields: Name, Phone, Email, Service dropdown, Message. Inline validation. Submit → loading → success state.

**WhatsApp Float:** Fixed bottom-right, terracotta-coloured, pulse.

## Content

### Hero
**Headline:** "Your Home Deserves to Look Its Best."
**Sub:** Professional house painting, Gamazine ceilings and paint supply in Pretoria North.

### Services
1. **Interior & Exterior Painting** — Walls, ceilings, doors, trims. Flawless prep, premium finish.
2. **Gamazine Textured Ceilings** — The classic spray-on ceiling finish. Smooth, clean, long-lasting.
3. **Hardware & Trade Supply** — Quality paints at trade prices for hardware stores and contractors.

### Portfolio (6)
1. Montañana Estate — Full home interior, warm terracotta feature wall
2. Annlin Family Home — Exterior repaint, storm grey with white trims
3. Sinoville Residence — Open-plan lounge, natural white throughout
4. Doornpoort Townhouse — Kitchen walls, Sage green cabinet accent
5. Wonderboom Home — Exterior + roof coating, cream with green shutters
6. Rosslyn Family House — Full Gamazine ceiling, 4 rooms

### About
We are Makena Paint Co — a Pretoria North painting contractor with 8+ years of experience. We started as part of Makena Building Group and have been transforming homes across Gauteng ever since. Every project is treated with the same care we'd give our own home.

### Testimonials
1. "The team was punctual, neat and the finish is impeccable. Our lounge looks like a different house." — Lerato M., Montañana
2. "Best Gamazine job we've had done. Smooth, even, no runs. And they cleaned up completely after." — Thabo K., Rosslyn
3. "Professional from start to finish. Fair price, honest advice, beautiful result. We'll use them again." — Karen van Z., Sinoville

### Areas
Pretoria North, Rosslyn, Soshanguve, Montañana, Annlin, Sinoville, Doornpoort, Wonderboom, Montana, Akasia, Mabopane, Centurion

### FAQ
1. How long does a house paint take?
2. Do you supply paint or do we buy it?
3. What surfaces do you paint?
4. How much does Gamazine cost per m²?
5. Do you offer a warranty?
6. Can you match any colour?

### Contact
Phone: +27 69 533 7778
WhatsApp: same
Email: info@makenapaint.co.za
Location: Rosslyn, Pretoria North
Hours: Mon–Fri 7:00–17:00, Sat 8:00–13:00

## Technical
- Single HTML file, all CSS/JS inline
- No heavy JS libraries — vanilla JS, CSS animations, Intersection Observer for reveals
- Google Fonts: Cormorant Garamond + Plus Jakarta Sans
- Unsplash for photography
- Mobile-first responsive
