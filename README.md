# Week 6: HTML and CSS, the academic website

A personal academic website with four pages (Bio, Research, Publications, Teaching), built live in class in six checkpoints. The same site continues in the JavaScript session and in the server-side session.

## How to use the checkpoints

Every folder is a complete, working copy of the site at one point in the session. Open `index.html` in any folder and it works on its own.

1. Everyone starts in `00-start`, which contains only the text and the portrait.
2. At the end of each stage, the class moves to the next checkpoint together.
3. If your own copy is broken or behind, open the next checkpoint folder and continue from there. You lose nothing you need.
4. If you finish early, try the challenges in `STRETCH.md`.

## What each checkpoint adds

| Folder | What is new | Key ideas |
|---|---|---|
| `00-start` | Plain text content for four pages and a portrait | Content comes before code |
| `01-semantic` | Four HTML pages, no CSS | Document structure, `header`, `nav`, `main`, `article`, `section`, `footer`, heading order, `alt` text, `aria-current`, relative links |
| `02-tokens` | `css/style.css` with colours, fonts and spacing | Linking a stylesheet, custom properties (`--color-accent`), `var()`, selectors, the box model |
| `03-layout` | Header, navigation, cards, footer laid out | Flexbox for rows, Grid for cards, centring with `max-width` and `margin-inline: auto` |
| `04-responsive` | Works on phones and desktops | Mobile first, `flex-wrap`, `repeat(auto-fit, minmax())`, `clamp()`, one media query |
| `05-final` | Dark mode and accessibility polish | `prefers-color-scheme`, changing tokens only, `:focus-visible`, skip link, `prefers-reduced-motion` |
| `stretch-solutions` | Optional extras, in a separate `css/stretch.css` | `:has()`, nesting, container queries, view transitions, print styles |

The stylesheet in each checkpoint marks new and changed rules with comments (`NEW in 04`, `CHANGED in 04`), so students can see exactly what moved on.

Checkpoint 03 deliberately uses a fixed three-column grid and a one-row header. Ask students to narrow the browser window: the layout breaks, and checkpoint 04 fixes it.

## What this site leaves for the next sessions

These are deliberate. They are the problems the following sessions solve.

| Week 6 limitation | JavaScript session | Server-side session |
|---|---|---|
| Header, navigation and footer are copied into all four pages | A JavaScript include, shown to be fragile | Templates and includes (DRY) |
| Publications are typed by hand in HTML | Rendered from an array or JSON | Read from a database |
| On phones, the navigation takes up space and cannot be hidden | A menu button that opens and closes | No change needed |
| Dark mode follows the system setting only | A toggle that remembers the choice | The preference could be stored per user |
| The CSS-only publication filter (stretch) | The same filter in JavaScript, compared | Filtering with a database query |

## Before using in class

- **Publications:** check author order, titles and status for each entry, and add earlier published work with full references and links.
- **Portrait:** `images/portrait.svg` is a placeholder. Replace it with a real photo (for example `portrait.jpg`) and update the `src` in each checkpoint from 01 onwards.
- **Contact:** the Bio page points students to the OPIT learning platform. Add an email address if wanted.
