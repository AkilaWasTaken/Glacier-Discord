

<p align="center">

&#x20; <img src="public/logo.png" alt="Glacier" width="140" />

</p>



<h1 align="center">Glacier</h1>



<p align="center">

&#x20; A simple redirect page for the Glacier community.<br />

&#x20; <a href="https://discord.gg/Z6h2PQAZe8"><strong>Join our Discord</strong></a>

</p>



<p align="center">

&#x20; <img src="https://img.shields.io/badge/HTML5-A0B4C8?logo=html5\&logoColor=white" alt="HTML5" />

&#x20; <img src="https://img.shields.io/badge/CSS3-647F9C?logo=css\&logoColor=white" alt="CSS3" />

&#x20; <img src="https://img.shields.io/badge/License-MIT-25374D" alt="MIT License" />

</p>



\---



\## Getting started



Clone or download the repository and open `index.html` in your browser.



Alternatively, run a local HTTP server using Python:



```bash

python -m http.server 8080

```



The page will be available at `http://localhost:8080`.



No dependencies or build process required.



\## Configuration



All configuration is handled directly in `index.html`.



\### Redirect URL



Update the Discord invite in both the meta refresh tag and the fallback link.



```html

<meta http-equiv="refresh" content="2; url=https://discord.gg/YOUR\_INVITE">

```



```html

<a href="https://discord.gg/YOUR\_INVITE">

&#x20;   Continue to Discord

</a>

```



\### Redirect delay



The first value in the `content` attribute defines how long the page waits before redirecting.



| Value | Behavior |

| ----- | -------- |

| `0` | Instant redirect |

| `2` | Redirect after 2 seconds (default) |

| `5` | Redirect after 5 seconds |



\### Appearance



Colors are defined as CSS variables in the `:root` section of the stylesheet.



```css

:root {

&#x20;   --background: #0B111A;

&#x20;   --surface: #151F2C;

&#x20;   --primary: #A0B4C8;

&#x20;   --secondary: #647F9C;

&#x20;   --border: #25374D;

&#x20;   --text: #E2E8F0;

&#x20;   --muted: #94A3B8;

}

```



Edit these values to customize the page without changing the layout.



\## Project structure



```

Glacier/

├── public/

│   └── logo.png

├── index.html

├── README.md

└── LICENSE

```



\## Deployment



The page can be hosted on any static hosting service, including GitHub Pages, Vercel, Cloudflare Pages, or a regular web server.



Deploy the repository as a static website with `index.html` in the root directory. No build commands or environment variables are required.



\## License



Licensed under the \[MIT License](LICENSE).



