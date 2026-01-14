# Skill Forward — Escape With Velocity

Static single-page marketing site for the Skill Forward bootcamps. The page outlines the AI ramp, 2-week and 4-week bootcamps, program deliverables, and a contact form that opens the visitor's email client. It mirrors the content structure of the Squarespace export but keeps everything in a single HTML file with lightweight CSS and vanilla JS.

## Repository layout

- `index.html` — All markup, styling, and behavior (hero, gallery, ramp, bootcamps, structure, contact form, marquee duplication script, and mailto handler).
- `assets/` — Local images used in the gallery (`upskill1.jpeg`, `upskill2.jpeg`, `workshop1.jpeg`, `worksystems.jpeg`).

## Previewing locally

No build tooling is required; open `index.html` directly in a browser or serve it with any static file server, e.g.:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080` to view the page.

## Customization tips

- Update CTA links, copy, and cohort details directly in `index.html`. Search for the relevant section IDs (`#ramp`, `#bootcamps`, `#how`, etc.).
- Replace the hero image URL or swap the gallery photos inside the `assets/` directory to better reflect your cohort.
- The contact form currently uses a `mailto:` link that sends to `ssuresh.srinivas@gmail.com`. Change the `to` variable near the bottom of the file if you need a different inbox or embed a hosted form instead.
- All styling lives in the `<style>` block at the top of `index.html`. You can tweak the CSS variables under `:root` to adjust the color palette, typography, spacing, and shadows globally.

## Deployment

Because the site is static, it can be hosted on GitHub Pages, Netlify, Cloudflare Pages, Vercel, or any static web server. Just upload `index.html` and the `assets/` directory, and ensure any external assets (like the hero image hosted on Squarespace) remain accessible.
