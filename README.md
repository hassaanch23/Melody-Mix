# 🎵 Melody Mix — Music Web App

Melody Mix is a client-side music player web application built with plain HTML, CSS and JavaScript. It was developed as a UI/UX-focused project and demonstrates a complete front-end experience for browsing, playing and organizing music without a backend.

**Quick summary:** a lightweight, educational music UI that uses `songsdata.json` and browser `localStorage` to manage songs, playlists and favourites.

**Table of contents**
- Project
- How it works
- Features
- File structure (high level)
- Run / Usage
- How to contribute
- Contributors
- License & notes

## Project

Melody Mix provides a multi-page interface (HTML files) where users can sign up, sign in, search songs, create playlists, like/favourite songs and play tracks. The app's logic and state live entirely on the client — no server required.

## How it works

- The static song catalogue is stored in `songsdata.json` (and some .txt song files used as content examples).  
- Pages such as `mainpage.html`, `playlistpage.html`, `favouritespage.html`, `searchpage.html`, and `songplaying.html` present views and interact via JavaScript files (`*.js`).  
- User accounts and saved data (playlists, likes, last played) are persisted using the browser's `localStorage`.  
- Playing a song opens the song player UI which reads song metadata and audio source from the project files.

## Features

- Sign up / Log in (client-side, `localStorage`)  
- Browse songs and open the player  
- Search songs with live results  
- Create and manage playlists  
- Mark songs as favourites (heart)  
- Simple responsive UI for desktop and mobile widths

## File structure (high level)

- `mainpage.html` / `mainpage.js` / `mainpage.css`: main landing view  
- `homepage.html` / `homepage.js` / `homepage.css`: top-level navigation UI  
- `login.html`, `signup.html`: auth pages (client-only)  
- `playlistpage.*`, `favouritespage.*`, `searchpage.*`, `songplaying.*`: feature pages  
- `songsdata.json`: static song list used by the app  
- various `.txt` files: song lyrics / sample content  
- `1.html`, `1.js`, `1.css`: (extra/demo files — safe to inspect)  
- `README.md`: this file

## Run / Usage

1. Clone or download the repository.  
2. Open `mainpage.html` (or `homepage.html`) in a modern browser (Chrome, Edge, Firefox).  
3. Use the UI to sign up, add playlists, like songs and open the player.  

Developer tip: you can host the folder with a simple static server if you want to test audio loading or CORS behavior, for example:

```powershell
# in repo root (PowerShell)
# serve with Python 3 built-in server
python -m http.server 5500; Start-Process "http://localhost:5500/mainpage.html"
```

## How to contribute

- Bug reports & suggestions: open an Issue.  
- Small fixes: fork, edit, and submit a Pull Request with a short description.  
- Adding songs: update `songsdata.json` with new entries and add audio/metadata files to the repo.  

Please keep changes small and focused so they are easy to review.

## Contributors

- **hassaanch23** — original author and repository owner

Want to be listed? Add your name and GitHub handle in a PR and it will be included here.

## License & notes

- This project contains static demo assets and is intended for educational / portfolio use.  
- No license file is included — add a `LICENSE` if you want to apply one (e.g., MIT).

---

If you'd like, I can also:
- add a small contribution guide (`CONTRIBUTING.md`), or
- generate a starter `LICENSE` (MIT) and add contributor credits.

Enjoy exploring `Melody Mix`!

