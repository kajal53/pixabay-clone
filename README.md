#  Pixabay Clone

A fully responsive image search app built with **React + Vite**, powered by the **Pixabay API**. Search millions of free stock images, browse by category, and save your favorites — all in a clean dark UI.

---

## ✨ Features

- 🔍 **Image Search** — Search any keyword and get results instantly
- 📂 **Category Filter** — Browse by Trending, Nature, Technology, People, Animals, Travel, Food and more
- ❤️ **Favorites** — Save and view your favourite images (stored in localStorage)
- ♾️ **Infinite Scroll** — Automatically loads more images as you scroll down
- 📱 **Responsive Design** — Works on mobile, tablet and desktop
- 🌑 **Dark Theme** — Clean dark UI built with Tailwind CSS

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| React 19 | UI Framework |
| Vite 7 | Build Tool |
| Tailwind CSS 4 | Styling |
| Lucide React | Icons |
| Pixabay API | Image Data |

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/kajal53/pixabay-clone
cd pixabay-clone
```

### 2. Install dependencies

```bash
npm install
```

Then add your Pixabay API key in the `.env` file:

```env
VITE_PIXABAY_API_KEY=your_api_key_here
VITE_PIXABAY_BASE_URL=https://pixabay.com/api/
VITE_PER_PAGE_INITIAL=20
VITE_PER_PAGE_LOAD_MORE=20
VITE_SCROLL_THRESHOLD=300
VITE_LOAD_MORE_DELAY=500
```

> 🔑 Get your free API key at: [https://pixabay.com/api/docs/](https://pixabay.com/api/docs/)

### 3. Run the app

```bash
npm run dev
```

App will open at: `http://localhost:5173`

---

## 📁 Project Structure

```
src/
├── components/
│   ├── layout/
│   │   ├── Navbar.jsx         # Search bar + Favorites button
│   │   └── Categories.jsx     # Category filter bar
│   ├── images/
│   │   ├── ImageGrid.jsx      # Image grid layout
│   │   └── ImageCard.jsx      # Single image card
│   └── ui/
│       ├── LoadingSpinner.jsx
│       ├── EmptyState.jsx
│       ├── ErrorMessage.jsx
│       └── FavoritesHeader.jsx
├── hooks/
│   ├── useImageFetch.js       # API fetch logic
│   ├── useFavorites.js        # Favorites state management
│   └── useInfiniteScroll.js   # Infinite scroll logic
├── services/
│   └── pixabay.service.js     # Pixabay API calls
├── config/
│   └── env.js                 # Environment variables config
└── App.jsx
```

---

## 📦 Build for Production

```bash
npm run build
```

---



## 📄 License

This project is open source and available under the [MIT License](LICENSE).
