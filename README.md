# Developer Toolbox

A fast, private, offline-ready set of everyday developer tools in a single web page. No sign-up, no tracking, no server. Everything runs in your browser.

**[Live demo](https://YOUR-USERNAME.github.io/dev-toolbox/)**

![Developer Toolbox screenshot](screenshot.png)

## Tools

| Tool | What it does |
|---|---|
| JSON formatter | Format, minify and validate JSON |
| Base64 | Encode and decode text (Unicode-safe) |
| URL encoder | Escape and unescape URL components |
| Color picker | Convert between HEX, RGB and HSL |
| Regex tester | Live match highlighting for JavaScript regex |
| Hash generator | SHA-1, SHA-256 and SHA-512 via the Web Crypto API |
| Timestamp converter | Unix time to readable dates and back |
| UUID generator | Random v4 UUIDs, up to 50 at once |

## Features

- Works offline and can be installed as an app (PWA)
- Automatic light and dark mode
- Responsive layout for phones and desktops
- Keyboard accessible
- Deep links to each tool, for example `#regex`
- Zero dependencies and no build step

## Run it locally

```bash
git clone https://github.com/YOUR-USERNAME/dev-toolbox.git
cd dev-toolbox
python3 -m http.server 8000
```

Then open http://localhost:8000. A local server is needed for the service worker to register. Opening `index.html` directly also works, without offline support.

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. Open **Settings → Pages**.
3. Set the source to the `main` branch and the `/ (root)` folder.
4. Save. Your site will be live in about a minute.

## Project structure

```
dev-toolbox/
├── index.html      # the whole app
├── manifest.json   # PWA manifest
├── sw.js           # service worker for offline use
├── icon.svg        # app icon
├── LICENSE
└── README.md
```

## Contributing

Ideas and pull requests are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

Good first additions: JWT decoder, diff checker, Markdown preview, cron expression explainer, case converter.

## Privacy

Nothing you type leaves your device. There are no analytics, no cookies and no network requests after the page loads.

## License

[MIT](LICENSE)
