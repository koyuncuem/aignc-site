# AIGNC Research Group — Website

Website of the AI-based Guidance, Navigation and Control Research Group (AIGNC-RG),
ITU Aerospace Research Center. Group leader: Prof. Dr. Emre Koyuncu.

Live site: GitHub Pages. **Content is edited through Pages CMS — no code editing needed.**

## Editing content (the normal way)

1. Go to **https://app.pagescms.org** and sign in with GitHub.
2. Open this repository's project.
3. Edit in the sidebar sections:
   - **News** — add/edit/reorder news items (top 3 appear on the homepage teaser).
   - **Team** — members (name, role, topics, photo picker) and alumni.
   - **Videos** — paste a YouTube video ID (the part after `watch?v=`) and a caption.
   - **Publications** — year, title, authors, venue, optional link. Grouped by year automatically.
   - **Page text** — the About paragraphs and Prof. Koyuncu's biography
     (separate paragraphs with a blank line).
4. **Media** tab — drag-and-drop team photos (they live in the `photos/` folder).
5. Save. The site republishes automatically in about a minute.

## How it works

The pages read their content at load time from flat data files, which Pages CMS edits:

| Data file | Feeds |
|---|---|
| `data-news.json` | Homepage news teaser + full news list |
| `data-team.json` | Team members grid + alumni |
| `data-videos.json` | Homepage video embeds |
| `data-publications.json` | Publications page |
| `data-general.json` | About + biography text on the homepage |

`.pages.yml` defines the editing forms shown in Pages CMS.

## Code-side (rarely needed)

- `index.html`, `team.html`, `research.html`, `publications.html` — page structure & design
- `styles.css` — all styling (`--blue` and `--magenta` in `:root` drive the palette)
- Research lines, projects, and labs on `research.html` are managed in code — ask Claude
  (or edit the HTML) to change them.
