
<p align="center">
  <img src="./public/logo.png" alt="Glacier" width="120" />
</p>

<h1 align="center">Glacier</h1>

<p align="center">
  A simple redirect page for the Glacier community.
  <br />
  <a href="https://discord.gg/Z6h2PQAZe8"><strong>Join our Discord</strong></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-A0B4C8?style=flat-square&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-647F9C?style=flat-square&logo=css&logoColor=white" alt="CSS3" />
  <a href="./LICENSE"><img src="https://img.shields.io/badge/License-MIT-25374D?style=flat-square" alt="MIT License" /></a>
</p>

---

## Getting started

Clone or download the repository and open `index.html` in your browser.

You can also run a local HTTP server using Python:

```bash
python -m http.server 8080
```

Open [localhost:8080](http://localhost:8080) to preview the page.

No dependencies or build process required.

## Configuration

All settings are located in `index.html`.

### Redirect URL

Replace the Discord invite in both the meta refresh tag and the fallback link.

```html
<meta http-equiv="refresh" content="2; url=https://discord.gg/YOUR_INVITE">
```

```html
<a href="https://discord.gg/YOUR_INVITE">
    Continue to Discord
</a>
```

### Redirect delay

Change the first value in the meta refresh `content` attribute.

| Value | Behavior |
| :--- | :--- |
| `0` | Instant redirect |
| `2` | Redirect after 2 seconds (default) |
| `5` | Redirect after 5 seconds |

### Appearance

The color palette is defined in the `:root` section of the stylesheet.

| Variable | Default |
| :--- | :--- |
| `--background` | `#0B111A` |
| `--surface` | `#151F2C` |
| `--primary` | `#A0B4C8` |
| `--secondary` | `#647F9C` |
| `--border` | `#25374D` |
| `--text` | `#E2E8F0` |
| `--muted` | `#94A3B8` |

The logo and browser icons can be replaced in the `public/` directory.

## Project structure

```text
.
├── public/
│   ├── logo.png
│   ├── favicon.ico
│   ├── favicon-16x16.png
│   ├── favicon-32x32.png
│   └── apple-touch-icon.png
├── index.html
├── README.md
└── LICENSE
```

## Deployment

Deploy the repository using any static hosting provider.

| Provider | Configuration |
| :--- | :--- |
| GitHub Pages | Deploy from the repository root |
| Vercel | Framework preset: Other |
| Cloudflare Pages | No build command |
| Nginx / Apache | Copy files to the web root |

No environment variables or build commands are required.

## License

Licensed under the [MIT License](./LICENSE).
