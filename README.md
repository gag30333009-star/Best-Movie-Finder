# 🎬 Cinema - Movie Finder

> A modern, responsive movie discovery app powered by TMDB API and a custom Django backend.

🌐 **Live Demo:** [gag30333009-star.github.io/Best-Movie-Finder](https://gag30333009-star.github.io/Best-Movie-Finder/)

---

## ✨ Features

- 🔥 **Trending Movies** - Discover what's hot this week
- ⭐ **Popular & Top Rated** - Browse curated collections
- 🎭 **14 Genre Filters** - Action, Comedy, Horror, Sci-Fi, and more
- 🔍 **Live Search** - Real-time suggestions as you type
- 🎬 **Movie Details** - Cast, director, budget, revenue, ratings
- ▶️ **YouTube Trailers** - Watch trailers directly in the app
- 💕 **Favorites System** - Save movies to your personal collection (Django backend)
- 🌐 **Watch Links** - Direct links to Netflix, Amazon, Disney+, Hulu, and more
- 📱 **Fully Responsive** - Works on phones, tablets, laptops, and 4K monitors

---

## 🛠️ Tech Stack

**Frontend:**
- HTML5 (semantic markup)
- CSS3 (Grid, Flexbox, custom properties, fluid typography with `clamp()`)
- Vanilla JavaScript (ES6+, Fetch API, Promises)

**APIs:**
- TMDB API (movie database)
- YouTube Embed API (trailers)

**Backend:** (separate repo)
- Django REST Framework
- Deployed on Render

**Hosting:**
- GitHub Pages (frontend)
- Render (backend)

---

## 🚀 Setup Instructions

### Prerequisites
- A TMDB API key (free at [themoviedb.org](https://www.themoviedb.org/settings/api))

### Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/gag30333009-star/Best-Movie-Finder.git
   cd Best-Movie-Finder
   ```

2. **Set up API key:**
   ```bash
   cp config.example.js config.js
   ```
   Edit `config.js` and add your TMDB API key.

3. **Open in browser:**
   Open `index.html` in any modern browser.

---

## 🎨 Design Philosophy

The app uses a **garnet + navy + orange** color palette inspired by classic cinema aesthetics. Key design principles:

- **Mobile-first responsive design**
- **Smooth animations** for engagement
- **Accessible UI** (keyboard navigation, ARIA labels, reduced-motion support)
- **Progressive enhancement** (works without JavaScript for SEO)

---

## 🔐 Security

- ✅ API keys managed via `.gitignore`
- ✅ Separate `config.example.js` template for setup
- ✅ HTTPS deployment

---

## 📐 Architecture

```
┌─────────────────────┐     ┌─────────────────────┐     ┌──────────────┐
│   Movie Finder UI   │ ──> │   TMDB API          │     │              │
│   (this repo)       │     │   (external)        │     │              │
└──────────┬──────────┘     └─────────────────────┘     │              │
           │                                              │              │
           │                                              │              │
           v                                              │              │
┌─────────────────────┐     ┌─────────────────────┐     │              │
│   Django Backend    │ ──> │   SQLite Database   │     │              │
│   (separate repo)   │     │   (cloud-hosted)    │     │              │
└─────────────────────┘     └─────────────────────┘     └──────────────┘
```

---

## 🐛 Known Issues & Solutions

| Issue | Solution |
|-------|----------|
| YouTube embed error on local file | Use deployed version on GitHub Pages |
| Trailer audio continues after modal close | Fixed by resetting iframe `src` |
| Backend not responding | Free Render instance spins down; first request takes 30-50 seconds |

---

## 🎯 What I Learned

Building this project taught me:
- Real-world API integration with error handling
- Secure API key management with `.gitignore`
- Responsive design with modern CSS (Grid, `clamp()`)
- DOM manipulation and event handling
- Asynchronous JavaScript with Fetch API and Promises
- Full-stack architecture (frontend ↔ backend ↔ database)
- Git workflow and deployment (GitHub Pages, Render)

---

## 🔗 Related Repositories

- **Backend (Django REST API):** [Movie-Backend](https://github.com/gag30333009-star/Movie-Backend)

---

## 📜 License

MIT License - feel free to use this for learning or your own projects.

---

## 👤 Author

**GAG**
- GitHub: [@gag30333009-star](https://github.com/gag30333009-star)
- Email: gag30333009@gmail.com
- Location: Yerevan, Armenia 🇦🇲

---

⭐ **If you found this useful, give it a star!** ⭐
