# 📚 Mini Kindle

A one-file PDF book reader that remembers your page. No server, no database, free forever.

**One HTML file. No app store. No account. No database. No cloud storage. Free forever.**

Your PDF books are stored *inside your phone's browser* (IndexedDB). Nothing is ever uploaded anywhere.

## Features

- **Add your own PDFs** and read them like books
- **Remembers your page** — close it anytime, it reopens exactly where you left off (per book)
- **Reading modes** — Day, Sepia, and Night (dark) themes
- **Kindle-style controls** — swipe to turn pages, or tap the left/right edge of the page
- **Zoom** text size with A− / A+
- **Progress tracking** — shelf shows a bookmark ribbon, current page, and % complete
- Works on **iPhone, Android, and computers**

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

1. Open your app link in **Safari**.
2. Tap the **Share** button (square with an up arrow).
3. Scroll down → tap **Add to Home Screen** → **Add**.
4. Open it from the new home-screen icon. Tap **Add PDFs** and pick books from your Files app.

**Important:** always open it from that icon, and don't clear Safari website data in
Settings → Safari (that would erase your shelf and bookmarks).

## 🤖 Set it up on your Android phone

1. Open your app link in **Chrome**.
2. Tap the **⋮ menu** (top right).
3. Tap **Add to Home screen** (on some phones: "Install app") → **Add**.
4. Open it from the icon. Tap **Add PDFs** and pick books from your file manager.

**Important:** don't clear Chrome's site data / browsing data for this site — that's where
your books and bookmarks live.

## How to read

| Action | How |
|---|---|
| Open a book | Tap its title on the shelf |
| Next / previous page | Swipe left/right, tap right/left third of the page, or use ‹ › |
| Jump to a page | Type the page number in the box |
| Text size | A− / A+ buttons |
| Reading mode | Day / Sepia / Night buttons |
| Back to shelf | ‹ Shelf button |
| Remove a book | "remove" on the book card |

## 💻 Bonus: run it on a computer instead (Python version)

The `local-server/` folder contains a version that stores books as normal files on disk,
served by a zero-dependency Python server:

```bash
cd local-server
python3 app.py
# open http://localhost:8765
```

Books are saved to a `books/` folder next to `app.py`. To read from your phone on the
same Wi-Fi, change `127.0.0.1` to `0.0.0.0` in the last line of `app.py` and open
`http://YOUR-COMPUTER-IP:8765` on the phone.

## Good to know

- **Privacy:** only the empty app is hosted online. Your PDFs are saved in your own
  browser's storage and never leave your device.
- **Internet:** needed the first time you open the app (it loads the PDF renderer,
  PDF.js, from a CDN). After that your browser usually caches it.
- **Backups:** keep your original PDFs in your Files app / storage too. Bookmarks and
  books are tied to the exact web address you use, so if you ever change hosting, you'd
  re-add books there.
- **Big books:** very large PDFs (hundreds of MB) may hit browser storage limits — add
  them one at a time.

## License

MIT — do whatever you like with it. Happy reading! 📖
