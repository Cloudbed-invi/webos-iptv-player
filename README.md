# WebOS IPTV Player PWA

A modern, fast, and lightweight IPTV player designed for Smart TVs (specifically LG WebOS) and modern browsers. Built as a Progressive Web App (PWA) with a focus on performance and remote control navigation.

## Features

-   **TV-First UI**: Fully navigable using a D-pad remote (Up, Down, Left, Right, Enter, Back).
-   **M3U Playlist Support**: Load custom playlists via URL.
-   **Smart Search**: Filter channels instantly with an optimized on-screen keyboard flow.
-   **Modern Design**: Dark theme, glassmorphism UI, and smooth animations inspired by premium streaming apps.
-   **Performance**:
    -   Optimized HLS.js config for low-latency streaming.
    -   Virtual scrolling / Dynamic grid columns.
    -   Lazy loading for images with smart fallback (Proxy -> Direct -> Text).
-   **Device Support**:
    -   LG WebOS (via hosted web app).
    -   Android TV / Fire TV (via browser).
    -   Desktop (Chrome/Edge/Firefox).

## How to use

1.  **Open the App**: Host the `index.html` on any static file server (GitHub Pages, Netlify, Vercel).
2.  **Add Playlist**:
    -   On first load, select "Add Profile".
    -   Enter a Name and the URL of your M3U playlist.
    -   Click Save.
3.  **Navigation**:
    -   **Arrow Keys**: Navigate the grid and sidebar.
    -   **Enter**: Select channel or confirm action.
    -   **Back / Esc**: Go back or close the player.
4.  **Search**:
    -   Navigate UP to the Search icon.
    -   Press **Enter** to open the keyboard.
    -   Type query and filter results.

## Deployment

Simply upload `index.html` to GitHub Pages.

1.  Create a new repository named `webos-iptv-player`.
2.  Run the commands below to push the code.
3.  Go to Settings -> Pages -> Source: `main` branch.
4.  Open `https://cloudbed-invi.github.io/webos-iptv-player/` on your TV's browser.

## Technical Details

-   **Core**: Vanilla HTML5, CSS3, JavaScript (ES6+).
-   **Video**: [hls.js](https://github.com/video-dev/hls.js) v1.5.2 for HLS streaming.
-   **Persistence**: `localStorage` for saving profiles and playlists.
-   **Images**: Uses `images.weserv.nl` proxy to handle mixed-content and CORS issues for channel logos.

## License

MIT License. Free to use and modify.
