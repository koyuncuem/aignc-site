# AIGNC Research Group — Website

Website of the AI-based Guidance, Navigation and Control Research Group (AIGNC-RG),
ITU Aerospace Research Center. Group leader: Prof. Dr. Emre Koyuncu.

Live site: served from `index.html` via GitHub Pages.

## How to edit

Everything is in the single `index.html`. Open it (pencil icon on GitHub) and
search for the marker you need:

| What to change            | Search for            | How |
|---------------------------|-----------------------|-----|
| Team members              | `TEAM ROSTER`         | One line per person in the `TEAM` array: `{name, degree, topics}` |
| Alumni                    | `alumni-row`          | Plain `<span>` entries |
| Research topics           | `Line 01` … `Line 04` | Add/remove `<span>` pills inside each `chips` div |
| Projects                  | `PROJECTS`            | Duplicate an `<article class="proj">` block; `status active` vs `status` toggles Active/Completed |
| Publications              | `PUBLICATIONS`        | Duplicate an `<article class="pub">` block |
| Leader bio & credentials  | `class="leader"`      | Text, pills, links |
| Colors                    | `:root`               | `--blue` and `--magenta` drive the palette |
| Contact info              | `CONTACT`             | Email, address, links |

Commit changes → the site republishes automatically in about a minute.
