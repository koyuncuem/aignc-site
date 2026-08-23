# AIGNC Research Group — Website

Website of the AI-based Guidance, Navigation and Control Research Group (AIGNC-RG),
ITU Aerospace Research Center. Group leader: Prof. Dr. Emre Koyuncu.
Structure modeled on classic academic lab sites: Home · Team · Research · Publications · News.

## Pages

| File | Contains |
|------|----------|
| `index.html` | Hero, latest-news teaser, about, **videos**, full **news** list |
| `team.html` | Leader profile, **member photo grid**, alumni |
| `research.html` | Four research lines, projects, labs |
| `publications.html` | Publications grouped by year |
| `styles.css` | All styling, shared by every page |

## How to edit

Open the file on GitHub (pencil icon), edit, commit — the site republishes in ~1 minute.

**News** — `index.html`, search `NEWS = [`. One entry per item, newest first:
`{date:"Feb 2026", title:"…", blurb:"…", url:"…"}`. For LinkedIn items, open the post →
⋯ menu → **Copy link to post** and use that URL. The top 3 automatically become the
homepage teaser cards.

**Videos** — `index.html`, search `VIDEOS = [`. Paste the YouTube ID (the part after
`watch?v=` in the video URL) in place of `PASTE_YOUTUBE_ID` and edit the caption.
Slots without an ID show a neutral placeholder.

**Team & photos** — `team.html`, search `TEAM = [`. One line per member. Photos:
upload square-ish JPGs into a `photos/` folder in the repo with the filenames already
listed in the array (e.g. `photos/akin-catak.jpg`). Easiest way: on the repo page choose
*Add file → Upload files* and drag a folder named `photos` containing the images.
Members without a photo automatically show their initials. Leader photo:
`photos/emre-koyuncu.jpg`.

**Photo filenames expected**
`emre-koyuncu.jpg`, `ahmet-talha-cetin.jpg`, `akin-catak.jpg`, `omar-shadeed.jpg`,
`seyed-roghani.jpg`, `ege-can-altunkaya.jpg`, `eren-ertugrul.jpg`, `mustafa-demir.jpg`,
`omer-herekoglu.jpg`, `ipek-osken.jpg`, `zeynep-uygar-yengin.jpg`, `sezenoglu-cetin.jpg`

**Research topics** — `research.html`, search `Line 01`…`Line 04`; edit the `<span>` pills.

**Projects** — `research.html`, search `projects-grid`; duplicate an
`<article class="proj">` block. `class="status active"` vs `class="status"` toggles
Active/Completed.

**Publications** — `publications.html`; duplicate an `<article class="pub">` block under
the right year, or add a new `<p class="pubyear">` heading.

**Colors** — `styles.css`, `:root` block; `--blue` and `--magenta` drive the palette.
