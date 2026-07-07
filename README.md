# M9 Theme Editor

**A free, visual editor for ES-DE gamelist theme XML.**

No install. No server. No account. Open one HTML file in Chrome or Edge and start dragging elements around — it reads and writes your real theme files directly on disk.

**[→ Open the tool](https://m9sypher.github.io/m9-s_esde_themer/m9themer.html)**

---

## What it is

ES-DE themes are hand-written XML — positioning every image, text box, and rating widget by typing raw coordinates, then reloading the whole frontend just to see if you got it close. This tool replaces that loop with a real canvas: drag elements where you want them, see your actual game art and fonts while you work, and export XML checked against real, working ES-DE themes — not just documentation guesses.

Everything runs client-side in your browser. Your theme files never leave your machine.

---

## Features

**Canvas & elements**
- Drag, resize, rotate any element, with a custom rotation pivot
- Multi-select, then align or distribute evenly
- Right-click menu: duplicate, front/back, delete, copy/paste style, save as a reusable snippet
- Snap to canvas center, other elements' edges, or an adjustable grid
- Alt/Ctrl + hover as a fallback for opening the context menu
- Real image, video, and font previews — not placeholder boxes
- 17 real ES-DE element types: image, text, rating, datetime, video, rectangle, carousel, grid, textlist, helpsystem, badges, ninepatch, animation, gamelistinfo, gameselector, systemstatus, clock
- Smooth dragging/resizing even on large files — no full-canvas re-render on every frame

**Real data while you work**
- Point it at your ROMs/gamelists folder for a real game to preview against
- Text/datetime elements bound to metadata show real descriptions, developer, release date, and more
- Images/videos resolve through the real `imageType` priority list against your actual `downloaded_media` folder, the same way ES-DE does it
- Case-insensitive filename fallback

**Files & folders**
- Open your real ES-DE themes folder, browse and switch between installed themes
- Load, edit, and save real gamelist XML straight back to disk
- Diff preview before every save, autosave drafts with crash recovery
- Batch find & replace with an automatic backup `.zip` and a typed confirmation before anything destructive happens
- Full-theme validation catching real ES-DE gotchas (empty properties, wrong color format, invalid property/element combos)

**Theme-wide tools**
- Capabilities editor — variants, color schemes, aspect ratios, font sizes, languages, transitions (this file is mandatory; ES-DE won't load a theme without it)
- Variables editor — flat `variables.xml` or multiple named color schemes
- Navigation sounds panel, asset browser, ghost overlay for comparing layouts

**Compile — build a new theme from scratch**
- Creates a real folder, writes a correctly wired `theme.xml` + mandatory `capabilities.xml` + your current canvas work
- Optionally copies assets from your currently open theme into the new one
- Every written file is read back and verified before it reports success

**Interface**
- Floating, freely resizable panels that remember position and size
- 8 color themes: Terminal, Photoshop (default), Dracula, Synthwave, Ocean, Nord, Windows 95, Linux
- Help menu with Tips, Keyboard Shortcuts, the Getting Started guide, and 15 step-by-step Tutorials
- Support tab with socials, Live Chat tab forwarding to Twitch when hosted online

---

## Getting started

1. Open the tool: **[m9sypher.github.io/m9-s_esde_themer/m9themer.html](https://m9sypher.github.io/m9-s_esde_themer/m9themer.html)** — use **Chrome or Edge**, since real folder access needs the File System Access API. (Firefox/Safari can still use Paste XML + Export download instead.)
2. Click **Open ES-DE themes folder** to browse a real theme, or **Paste XML** to work on a snippet without touching disk.
3. For full previews with real game data: also open your **ROMs/gamelists folder** and your **downloaded_media** folder.

Want to keep a local copy for offline editing? Download [`m9themer.html`](m9themer.html) straight from this repo — no internet connection needed once you have it.

---

## Honest limitations

- This is a visual **approximation**, not a renderer — carousel/grid item transforms, exact text-wrap behavior, and some shader-level effects won't be pixel-perfect.
- Element types the tool doesn't recognize are preserved untouched in the raw XML, just not visually editable.
- Always double-check a themed screen in real ES-DE before considering it final.

---

## License

This project is free to use, modify, and share. In plain terms:

- **You're free to** use this tool, edit the code, and build on it.
- **If you redistribute it, re-host it, or release a modified version, please credit [@m9sypher](https://github.com/m9sypher)** — a visible mention is all that's asked.
- **No warranty.** This software is provided "as is," with no guarantee it's fit for any particular purpose. Use it at your own risk, and always double-check your theme in real ES-DE before relying on it.

## Using or re-releasing this project

**A safety note on copies from elsewhere:** this is a plain HTML/JavaScript file, which means anyone can technically download it, modify it, and re-upload it somewhere else under any name. If you find a copy of this tool outside of this official repository, its GitHub Pages link above, or the official Ko-fi listing — **be cautious**. There's no way to guarantee what a modified copy might do differently (including potentially unwanted or harmful additions), since neither GitHub nor I can vet third-party re-uploads. When in doubt, grab it from one of the official links, not a random site claiming to host it.

---

## Support

Built by **M9sypheR**. Free forever.

- Twitch: [twitch.tv/M9sypheR](https://www.twitch.tv/m9sypheR)
- YouTube: [youtube.com/@m9sypher](https://www.youtube.com/@m9sypher)
- Kick: [kick.com/m9sypher](https://kick.com/m9sypher)
- TikTok: [tiktok.com/@m9sypher](https://www.tiktok.com/@m9sypher)
- Ko-fi: [ko-fi.com/m9sypher/shop](https://ko-fi.com/m9sypher/shop) — completely optional, always appreciated
