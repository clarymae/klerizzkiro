# Design — Personal Portfolio

## Document structure
A single `index.html`:

```
<!doctype html>
<html lang="en">
  <head>
    <meta charset>, <meta viewport>, <title>
    <style> ... all CSS ...</style>
  </head>
  <body>
    <header>   name + role
    <main>     three project <article> cards in a grid
    <footer>   email + GitHub + LinkedIn links
  </body>
</html>
```

No `<script>` anywhere. No external links to CSS/JS.

## Design Tokens
Declared once in `:root` so the whole page is rethemable from four values.

| Token | Value | Role |
|---|---|---|
| `--bg` | `#0f1115` | page background |
| `--ink` | `#eef2f6` | primary text |
| `--muted` | `#8a9bad` | secondary text |
| `--accent` | `#f59e0b` | links, heading accents |

Supporting (not themable, structural): `--card:#1a1f28`, `--line:#2b3340`.

## Layout
- Centered column, `max-width: 820px`, auto margins, generous padding.
- `header`: centered, large `<h1>` name with accent span, muted role line.
- `main > .projects`: `display:grid` with three equal columns on desktop.
- Each project is an `<article>` with `<h2>` title, one-sentence `<p>`, one `<a>`.
- `footer`: centered row of three links (email, GitHub, LinkedIn).

## Responsive behaviour
- `@media (max-width:760px)`: `.projects` becomes a single column; heading sizes reduce.
- `<meta name="viewport" content="width=device-width, initial-scale=1">` ensures correct phone scaling.

## Style
- Dark background (`--bg`), light ink text, single warm accent (`--accent`).
- Cards: subtle surface (`--card`) with a thin border (`--line`), rounded corners.
- Spacing: 56px top header padding, 18–24px card padding, 40–48px gaps between sections.

## Content (made up except name & email)
- Name: Clary Mae F. Llaguno
- Role: "Front-end developer who builds fast, accessible web experiences."
- Projects:
  1. **TaraBiyahePH** — A trip planner that maps budget itineraries across the Philippines. Link: https://example.com/tarabiyahe
  2. **PlateMate** — A recipe app that turns whatever is in your fridge into a dinner plan. Link: https://example.com/platemate
  3. **StudySprint** — A focus timer that gamifies study sessions with streaks and stats. Link: https://example.com/studysprint
- Contacts:
  - Email: clarymaellaguno21@gmail.com
  - GitHub: https://github.com/clarymaellaguno
  - LinkedIn: https://www.linkedin.com/in/clarymaellaguno
