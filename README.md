# 📚 Mini Kindle

A one-file PDF book reader that remembers your page. No server, no database, free forever.

**One HTML file. No app store. No account. No database. No cloud storage. Free forever.**

Your PDF books are stored *inside your phone's browser* (IndexedDB). Nothing is ever uploaded anywhere.

## Features

- **Add your own PDFs** and read them like books
- **Kindle-style pages** — in Reflow layout the text is split into clean, screen-sized
  pages. Nothing ever runs off the edge or spills onto the next screen, and making the
  text bigger simply creates more pages — just like a real e-reader
- **Two layouts** — *Reflow* (resizable, reflowing text) or *Page* (the exact PDF, for
  scans, diagrams, and fixed layouts)
- **Highlight as you read** — select any text, pick a colour (yellow / green / pink /
  blue), and it's saved in your browser. A **Highlights** panel lists them all so you can
  jump straight back to any passage
- **Remembers your place** — close it anytime, it reopens on the exact page *and* screen
  you left off (per book)
- **Soft, book-like paper** — Day, Sepia, and Night themes tuned to be gentle on the eyes
- **Typography controls** — text size, line spacing, serif/sans typeface, and page margins
- **Kindle-style navigation** — swipe or tap the left/right edge to turn pages, tap the
  middle for a page scrubber with live thumbnails, or use the arrow keys on a computer
- **OCR for scanned books** — turn a picture-of-text page into real, resizable text
- **Progress tracking** — the shelf shows a bookmark ribbon, current page, and % complete
- **Responsive** — a comfortable single-column book page on phones, a centred book-like
  page on desktop. Works on **iPhone, Android, and computers**

## Quick start (easiest way — works for both iPhone & Android)

The app needs a web address to run, so host this single file for free. Two options:

### Option A: GitHub Pages (if you forked/cloned this repo)

1. Fork this repository (button at the top right).
2. In your fork, go to **Settings → Pages**.
3. Under "Build and deployment", set **Source: Deploy from a branch**, choose the **main** branch and **/ (root)** folder, then Save.
4. Wait a minute. Your app is now live at:
   `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

### Option B: Netlify Drop (no GitHub needed)

1. Download `index.html` from this repo.
2. Go to [app.netlify.com/drop](https://app.netlify.com/drop) and sign up (free).
3. Put `index.html` inside a folder and drag the folder onto the drop zone.
4. Netlify gives you a permanent free link like `https://some-randome-name.netlify.app`.
   ⚠️ Make sure you're logged in — unclaimed drops expire in 24 hours.

## 📱 Set it up on your iPhone

1. Open your github or netlify app link in **Safari**.
2. Tap the **Share** button (square with an up arrow).
3. Scroll down → tap **Add to Home Screen** → **Add**.
4. Open it from the new home-screen icon. Tap **Add PDFs** and pick books from your Files app.

**Important:** always open it from that icon, and don't clear Safari website data in
Settings → Safari (that would erase your shelf and bookmarks).

## 🤖 Set it up on your Android phone

1. Open your github or netlify app link in **Chrome**.
2. Tap the **⋮ menu** (top right).
3. Tap **Add to Home screen** (on some phones: "Install app") → **Add**.
4. Open it from the icon. Tap **Add PDFs** and pick books from your file manager.

**Important:** don't clear Chrome's site data / browsing data for this site — that's where
your books and bookmarks live.

## How to read

| Action | How |
|---|---|
| Open a book | Tap its title on the shelf |
| Next / previous page | Swipe left/right, tap the right/left edge, or arrow keys / spacebar |
| Jump to a page | Tap the middle of the page (or the progress bar) for the scrubber |
| Highlight text | Select text → pick a colour in the popup (Reflow layout) |
| Review / jump to highlights | Tap the **▤** button in the top bar |
| Text size | ☰ menu → Text size A− / A＋ (or `+` / `−` keys) |
| Layout, spacing, typeface, margins, theme | ☰ menu |
| Back to shelf | ‹ Shelf button (or Esc) |
| Remove a book | "remove" on the book card (highlights are kept) |

## Good to know

- **Privacy:** only the empty app is hosted online. Your PDFs are saved in your own
  browser's storage and never leave your device.
- **Internet:** needed the first time you open the app (it loads the PDF renderer,
  PDF.js, from a CDN). After that your browser usually caches it.
- **Backups:** keep your original PDFs in your Files app / storage too. Your books,
  reading position, and highlights are tied to the exact web address you use, so if you
  ever change hosting, you'd re-add books there.
- **Big books:** very large PDFs (hundreds of MB) may hit browser storage limits — add
  them one at a time.

## License

MIT — do whatever you like with it. Happy reading! 📖
