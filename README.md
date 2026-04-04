# Zartan Restomods

A premium frontend for a vintage car restoration (restomod) business. Features a museum-inspired design with smooth GSAP scroll animations and a unique split-screen layout.

## Features

- **Split-Screen Layout**: Scrollable content on the left, sticky animated canvas on the right
- **Scroll-Driven Animation**: 98-frame car animation tied to scroll progress using GSAP ScrollTrigger
- **Vintage Museum Frame**: Custom CSS frame with elegant grey/ivory/violet accents
- **Smooth Animations**: Fade-up, stagger, and slide animations on scroll
- **Responsive Design**: Adapts to tablet and mobile viewports

## Sections

- **Hero**: Brand introduction with stats and CTAs
- **About**: Company story and philosophy cards
- **Gallery**: Portfolio grid with hover overlays
- **Contact**: Contact info and inquiry form
- **Register**: Project inquiry form with step-by-step process

## Tech Stack

**Frontend (Current)**

- HTML5 / CSS3
- GSAP 3.14 + ScrollTrigger

**Backend (Planned)**

- Next.js
- MongoDB

## Design System

### Colors

| Color      | Hex       | Usage                   |
| ---------- | --------- | ----------------------- |
| Violet     | `#6b4c9a` | Primary accent, buttons |
| Turquoise  | `#40b5ad` | Section labels, accents |
| Yellow     | `#f4d03f` | Highlights              |
| Ivory      | `#fffff0` | Background tints        |
| Grey Light | `#ebedef` | Page background         |
| Charcoal   | `#2d2d2d` | Text                    |

### Typography

- **Headings**: Playfair Display (serif)
- **Body**: Cormorant Garamond (serif)
- **Labels/Nav**: Montserrat (sans-serif)

## Project Structure

```
zartan/
├── index.html          # Main HTML file
├── style.css           # Stylesheet
├── README.md
└── static/
    ├── frames/
    │   └── eznew/      # 98 WebP frames for scroll animation
    ├── bg.png          # Gallery images
    ├── t1.webp
    ├── t2.webp
    ├── m1.webp
    └── m2.webp
```

## Getting Started

1. Clone the repository
2. Open `index.html` in a browser (or use a local server)

```bash
# Using Python
python -m http.server 8000

# Using Node
npx serve
```

3. Navigate to `http://localhost:8000`

## Scroll Animation

The canvas displays a 98-frame sequence that plays as you scroll. Frames are located in `static/frames/eznew/` and named `frame_001.webp` through `frame_098.webp`.

To use your own animation:

1. Export frames as WebP (recommended) or JPG
2. Name them sequentially with zero-padded numbers
3. Update `frameCount` and `currentFrame()` path in the script

## License

MIT
