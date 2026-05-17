# KAATAN Website — Claude Session Context

## Key facts
- Artist: KAATAN (primary identity) / INGA (live avatar). Based in Bangalore.
- Repo: sibyjohn0/kaatan | GitHub Pages: https://sibyjohn0.github.io/kaatan/
- Shortlink: https://tinyurl.com/kaatan
- Local file: /tmp/kaatan/index.html (re-download from GitHub if /tmp cleared)
- Push method: Python + GITHUB_TOKEN env var (see any previous push command)

## Palette
--bg #0C0808 | --gold #D4920E | --red #C93B1E | --teal #0F7050
--pink #E8907A | --cream #F5E6C8 | --indigo #1C1038
Bright accent for headings: #F7C520 (bright gold), #FFFFFF, #FF9944

## Typography
Headings: Bebas Neue | Body: Space Mono
Script fonts: Noto Sans Tamil (wght 700), Noto Sans Devanagari (wght 700)

## Architecture
Single HTML file — all CSS + JS embedded in index.html.
Key sections: Hero (YouTube bg video), About, Universe, Music (Spotify + YT), Collaborate, Footer
Assets in repo root: rose-medallion.png, rose-splash.jpg

## Active features
- Splash screen: rose-splash.jpg full-screen, gold flare burst → site
- Hero KAATAN title: bright gradient #F7C520→#FFF→#FF9944, cycles English→Tamil→Hindi via glitch transition
- Section headers ([data-letters]): letter cascade → gradient-active flowing text
- Rose medallion in section dividers
- Custom gold cursor, scroll reveal, marquee strip, rangoli dot bg on Universe section

## Known issues / rules
- Always hard-refresh (Cmd+Shift+R) or test incognito after pushing — GH Pages caches aggressively
- filter:drop-shadow conflicts with -webkit-background-clip:text legibility — use text-shadow instead
- pointer-events:none on .video-bg iframe prevents YouTube controls from appearing
- Splash shows every page load (sessionStorage guard removed intentionally)
