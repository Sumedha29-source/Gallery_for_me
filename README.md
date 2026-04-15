# Gallery_for_me
A aesthetic gallery for fun purpose 
# Lavender & Burgundy Gallery

A curated online art gallery built with React and Vite, featuring a refined lavender and burgundy colour palette. Browse, filter, and explore contemporary artworks through an elegant, responsive interface with lightbox viewing.

---

## Features

- **Gallery grid** — responsive masonry-style layout with artwork cards
- **Lightbox viewer** — full-screen image view with keyboard navigation (arrow keys + Escape)
- **Category filtering** — filter artworks by type (Painting, Photography, Sculpture, etc.)
- **Multiple pages** — Home, Exhibitions, About, and Contact
- **Responsive design** — mobile-first layout with hamburger navigation
- **Lazy loading** — images load on demand for fast performance

---

## Tech Stack

- [React 18](https://react.dev/) — UI framework
- [Vite 5](https://vitejs.dev/) — build tool and dev server
- [React Router v6](https://reactrouter.com/) — client-side routing
- CSS custom properties — theming with lavender and burgundy variables
- Google Fonts — Playfair Display (headings) + Inter (body)

---

## Getting Started

### Prerequisites

- Node.js 18 or higher
- npm 9 or higher

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/lavender-burgundy-gallery.git
cd lavender-burgundy-gallery

# Install dependencies
npm install

# Start the development server
npm run dev
```

The app will be available at `http://localhost:5173`.

---

## Project Structure

```
lavender-burgundy-gallery/
├── public/
│   ├── favicon.ico
│   ├── index.html
│   └── images/
│       ├── hero-bg.jpg
│       └── gallery/          # Artwork image files
│
├── src/
│   ├── assets/               # Logo and fonts
│   ├── styles/
│   │   ├── variables.css     # Colour tokens and design system
│   │   ├── global.css        # Base/reset styles
│   │   ├── navbar.css
│   │   ├── hero.css
│   │   ├── gallery.css
│   │   └── lightbox.css
│   ├── components/
│   │   ├── Navbar.jsx
│   │   ├── Hero.jsx
│   │   ├── Gallery.jsx
│   │   ├── GalleryCard.jsx
│   │   ├── Lightbox.jsx
│   │   ├── FilterBar.jsx
│   │   └── Footer.jsx
│   ├── pages/
│   │   ├── Home.jsx
│   │   ├── About.jsx
│   │   ├── Exhibitions.jsx
│   │   └── Contact.jsx
│   ├── data/
│   │   ├── artworks.js       # Artwork metadata
│   │   └── exhibitions.js    # Exhibition data
│   ├── hooks/
│   │   ├── useGallery.js
│   │   └── useLightbox.js
│   ├── App.jsx
│   └── main.jsx
│
├── package.json
├── vite.config.js
└── README.md
```

---

## Adding Artworks

Add new artwork entries to `src/data/artworks.js`:

```js
{
  id: 4,
  title: 'Morning Haze',
  artist: 'Sofia Blanc',
  year: 2024,
  category: 'Painting',       // Used for filter bar
  medium: 'Watercolour on paper',
  image: '/images/gallery/artwork-4.jpg',
  price: '£1,200',            // Use 'On request' if unlisted
}
```

Place the corresponding image in `public/images/gallery/`.

---

## Colour Palette

| Token | Value | Usage |
|---|---|---|
| `--lavender` | `#9B8EC4` | Accents, tags, hover states |
| `--lavender-light` | `#C8B8E8` | Backgrounds, borders |
| `--lavender-pale` | `#F0EBF8` | Section backgrounds |
| `--burgundy` | `#6D1A2E` | Primary headings, CTA buttons |
| `--burgundy-dark` | `#4A0F1E` | Hover states, deep accents |
| `--burgundy-light` | `#A0304A` | Secondary text accents |
| `--cream` | `#FAF7F2` | Page background |

---

## Available Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start dev server at localhost:5173 |
| `npm run build` | Build for production into `dist/` |
| `npm run preview` | Preview the production build locally |

---

## Deployment

Build the project and deploy the `dist/` folder to any static host:

```bash
npm run build
```

Recommended hosts: **Vercel**, **Netlify**, or **GitHub Pages**.

For React Router to work on Netlify, add a `public/_redirects` file:

```
/*  /index.html  200
```

---

## License

MIT — feel free to use and adapt for your own gallery projects.