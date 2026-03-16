# Nutri Valley — Astro Website

Pixel-perfect implementation από το XD design (1920px desktop).

## Setup

```bash
cd nutri-valley
npm install
npm run dev      # http://localhost:4321
npm run build    # production build
```

## Project Structure

```
src/
├── components/
│   ├── Header.astro          # Navbar + mega menu
│   ├── Hero.astro            # Hero slider
│   ├── ProductsAdults.astro  # Oval cards carousel
│   ├── ProductsKids.astro    # Peppa Pig / PJ Masks / Minions cards
│   ├── About.astro           # Dark section με checklist
│   ├── Recipes.astro         # 4 recipe photos grid
│   ├── Events.astro          # Beige texture section
│   ├── Blog.astro            # 2 blog post cards
│   └── Footer.astro          # Footer + bottom bar
├── layouts/
│   └── Layout.astro          # HTML shell + global CSS + design tokens
└── pages/
    └── index.astro           # Homepage
```

## Assets που χρειάζονται (κατέβασε από XD)

Βάλε όλα τα αρχεία στο φάκελο `public/assets/`:

### Fonts
```
public/assets/fonts/
  TikTokSans-Bold.woff2
  TikTokSans-Regular.woff2
```
→ Download: https://www.tiktok.com/brand/font  (ή χρησιμοποίησε Nunito/Inter ως fallback)

### Logo
```
public/assets/images/
  logo.svg           ← NUTRI VALLEY logo (από XD Download)
  favicon.svg
```

### Hero
```
public/assets/images/hero/
  hero-slide-1.png   ← Granola + Αφράτες product shot
  hero-bg-1.jpg      ← Beige background texture
```

### Products - Adults
```
public/assets/images/products/
  konserves.png      ← Κοτόπουλο κονσέρβα
  mpares.png         ← Μπάρες πρωτεΐνης
  gkofretes.png      ← Αφράτες γκοφρέτες
  taxini.png         ← Ταχίνι jar
  dhmitrh.png        ← Δημητριακά (αν υπάρχει)
```

### Kids
```
public/assets/images/kids/
  peppa-pig-logo.png
  peppa-pig-products.png
  pj-masks-logo.png
  pj-masks-products.png
  minions-logo.png
  minions-products.png
```

### Menu (mega menu thumbnails)
```
public/assets/images/menu/
  konserves-thumb.jpg
  mpares-thumb.jpg
  gkofretes-thumb.jpg
  taxini-thumb.jpg
```

### About
```
public/assets/images/about/
  oats-bg.jpg        ← Dark oats falling background
```

### Recipes
```
public/assets/images/recipes/
  recipe-1.jpg       ← Τηγανητό ρύζι
  recipe-2.jpg       ← Granola
  recipe-3.jpg       ← Ρυζογκοφρέτες
  recipe-4.jpg       ← Ζυμαρικά
```

### Events
```
public/assets/images/events/
  events-texture-bg.jpg   ← Beige paper texture
  event-photo-1.jpg       ← Άτομα σε event
  event-photo-2.jpg       ← Stand/products στο event
```

### Blog
```
public/assets/images/blog/
  blog-1.jpg         ← Φιλέτο κοτόπουλο
  blog-2.jpg         ← Βιωσιμότητα
```

## Design Tokens (CSS Variables)

| Token | Value | Χρήση |
|-------|-------|-------|
| `--green` | `#859E66` | Primary button, accents |
| `--dark` | `#474444` | Text, dark buttons |
| `--beige` | `#C4B2A3` | Hero bg, Events bg |
| `--light` | `#E8E8E8` | Borders, dividers |
| `--yellow` | `#F9F3AF` | Accent |
| `--white` | `#FFFFFF` | Backgrounds |

## Typography

Font: **TikTok Sans** (Bold 700 + Regular 400)

| Element | Size | Weight | Letter-spacing |
|---------|------|--------|----------------|
| Hero heading | 42px | 700 | 2.1px |
| Nav links | 17px | 700 | 1.7px |
| Section titles | 32px | 700 | 1.5px |
| Body | 16px | 400 | normal |

## Screens υλοποιημένα

- ✅ Homepage - Desktop (1920×7600px)
- ✅ Menu - Desktop - 1 (dropdown)
- ✅ Menu - Desktop - 2 (kids dropdown)
- ⬜ Homepage - Desktop Hovers (hover states — add CSS :hover rules)
