# 🍫 ChocoTV – Simple Web M3U Player

**ChocoTV** is a web-based IPTV player that allows you to watch TV channels from an M3U playlist file. It features a clean, responsive interface built with modern web technologies.

![screenshot](https://files.catbox.moe/p2k6ia.png)

## ✨ Features

- **M3U Playlist Parsing** – Loads and parses standard `.m3u` playlist files.
- **Channel Grouping** – Organizes channels based on `group-title` (usually by country).
- **HLS Playback** – Uses [HLS.js](https://github.com/video-dev/hls.js) to play `.m3u8` video streams. Native fallback for Safari.
- **Responsive Design**
  - Desktop: Three-column layout (Countries → Player → Channels)
  - Mobile: Player-first layout with slide-up panels
- **Channel Logos** – Shows logos from `tvg-logo` in the playlist.
- **Flags & Icons** – Displays country flags (via [flag-icons](https://github.com/lipis/flag-icons)) and category icons (via Font Awesome).
- **Manual Video Quality Selection** – Select stream resolution if supported.
- **Search Function** – Real-time filter for channels in current country.
- **Auto Retry** – Reconnects automatically on stream failure.
- **Multi-language UI** – Available in 🇮🇹 🇬🇧 🇷🇴 🇷🇺 🇨🇳 🇪🇸. Auto-detects browser language or manual selection (saved in `localStorage`).
- **Welcome Modal** – Friendly intro for first-time visitors.
- **Modern UI** – Clean dark theme styled with Tailwind CSS.

## 🚀 How to Use / Deploy without Network Error

### 🧾 Setup

1. Place your `index.html` in the root directory.
2. Place your playlist named **`index.m3u`** in the same root.
3. *(Optional)* Add `manifest.json` and `service-worker.js` for PWA features (if desired).

### 🧪 Local Testing

If you want to test locally, use Python in the same folder you put "index.html,index.m3u,favicon.png and apple-touch.icon.png to open the website local:

```bash
python -m http.server
```

Then visit: `http://localhost:8000/`

You shouldn't have anymore network errors

> Opening `index.html` directly will block loading `index.m3u` due to browser security (CORS).

### ☁️ Deploy to GitHub Pages

1. Push your files to GitHub.
2. Go to **Settings > Pages**.
3. Select the root folder (`/`) of your `main` or `master` branch.
4. Your app will be live at:

```
https://YOUR_USERNAME.github.io/YOUR_REPOSITORY/
```

## 🛠️ Built With

- HTML5
- Tailwind CSS
- JavaScript (Vanilla)
- [HLS.js](https://github.com/video-dev/hls.js)
- [Font Awesome](https://fontawesome.com/)
- [flag-icons](https://github.com/lipis/flag-icons)

## 👤 Author

Created by **KakaoXI**  
GitHub Repository: [https://github.com/KakaoXI/ChocoTV](https://github.com/KakaoXI/ChocoTV)

## 📄 License

This project is licensed under the **MIT License**.  
See [LICENSE](LICENSE) for details.

🔗 [MIT License – Full Text](https://opensource.org/licenses/MIT)
