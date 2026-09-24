# Client brief — Dr. Leia D. Belt, PhD

_Status:_ in build
_Started:_ 2026-09-21   _Target launch:_ [ADD ACTUAL INFORMATION]
_Services sold:_ Website (personal/professional scholar site)
_Quote:_ [ADD ACTUAL INFORMATION]

---

## The person

- **Name:** Dr. Leia D. Belt, PhD
- **What she does, in one sentence:** Interdisciplinary sociologist and population
  health researcher studying how history, place, and structural racism shape
  contemporary health and inequality.
- **Main contact:** [ADD ACTUAL INFORMATION — email, best way to reach]
- **Current institution:** University of California, Merced (postdoctoral
  research) — [VERIFY BEFORE PUBLISHING: exact title, department, dates]

This is **not** a Golden Valley Web local-business site. It does not use the
`_template/` SaaS-style scaffold or the studio's three-service positioning —
those apply to GVW's own local-business clients only. This is a fully custom
editorial/academic personal site, built once from the detailed design brief
the client (via Richie) provided in full.

## Content status — read before editing

The client supplied extensive **positioning, tone, and section-by-section
copy direction**, but very little concrete biographical/CV data (exact
degrees, dates, publications, grants, collaborators, courses, speaking
engagements, links). Per the client's own explicit content rule:

> Do not fabricate biographical information, academic credentials, employment,
> research findings, publications, awards, grants, clients, collaborators,
> statistics, participant quotations, media appearances, speaking engagements,
> teaching experience, book contracts, or institutional partnerships.

So `index.html` uses the client's own placeholder convention throughout:
- `[ADD ACTUAL INFORMATION]` — missing facts.
- `[VERIFY BEFORE PUBLISHING]` — facts entered but not yet confirmed (e.g. the
  UC Merced postdoc details, mentioned once in the brief without dates).

**Before launch, replace every bracketed placeholder** — search the file for
`[ADD ACTUAL` and `[VERIFY BEFORE`. Sections still fully placeholder pending
real content: Professional Experience (dates/titles), Publications (every
entry), Speaking engagements (every entry), Teaching (courses), Ideas &
Perspectives (all articles — currently an honest empty state), Selected
Projects (collaborators/methods/outputs), Contact (all external profile
links), CV file.

Copy that **is** real (used near-verbatim from the client's brief, not
invented): the headline, subhead, expertise line, research-philosophy
statement (History/Place/Health/Community), the seven core-research-area
descriptions, the methods clusters, and the sundown-towns project framing.
Treat all of that as approved editorial copy, not draft.

## Brand direction (from client brief, not GVW defaults)

- **Feel:** intelligent, historically grounded, warm, sophisticated, Black
  scholarly, culturally aware, research-driven, editorial, archival, premium.
  Explicitly *not* generic-university blue/white, not SaaS/tech, not
  nonprofit-cheerful.
- **Palette:** warm archival — cream/parchment ground, rust/terracotta as the
  primary accent, deep aubergine/plum for occasional dark panels, ochre/olive/
  forest as secondary accents. See brand tokens at the top of `index.html`.
- **Type:** Source Serif 4 (editorial serif, headlines + pull quotes) + IBM
  Plex Sans (body/UI) + IBM Plex Mono (eyebrows/labels/archival tags). All
  Google Fonts (free), standing in for the brief's paid suggestions
  (Freight/Tiempos, Neue Haas).
- **Imagery:** no AI-generated portrait. Hero shows a real client-supplied
  photo (`assets/portrait-leia-belt.webp`) against the editorial/archival
  contour-line + grid motif, background removed with `rembg` (alpha matting +
  a connected-component cleanup pass to drop stray background specks — see
  the note below). Not a corporate headshot card.

## Structure delivered

Single-page site (`index.html`), sticky nav (About / Research / Publications
/ Teaching / Speaking / Contact + "Collaborate With Me" CTA), mobile slide-out
drawer. Sections, in order: Hero → Expertise strip → About (with expandable
"full story") → Research philosophy (History/Place/Health/Community) → Core
research areas (7 cards) → Featured project (sundown towns) → Digital
scholarship / born-digital book → Community-engaged public health data
(San Joaquin Valley & Sierra Foothills) → Participatory & qualitative research
→ Selected projects → Methods → Professional experience timeline →
Publications (filterable/searchable) → Books & major projects → Speaking &
Conversations → Teaching & Mentorship → Ideas & Perspectives → Collaboration
→ Contact → Footer.

Accessibility: skip link, semantic landmarks, visible focus rings, keyboard
nav + drawer, `prefers-reduced-motion` respected, alt-text placeholders on
the portrait/figures, publications filter is a real `<form>`/buttons (not
mouse-only). SEO: title/meta description/canonical/OG tags, `Person` JSON-LD
with `knowsAbout`, `ScholarlyArticle` stubs on publication entries.

## Hosting & deploy

- **Repo:** github.com/RichieGitMoney/leia-belt-phd — [VERIFY BEFORE
  PUBLISHING: confirm slug/repo name and GitHub owner with the client]
- **Domain live at:** [ADD ACTUAL INFORMATION]
- **DNS registrar:** [ADD ACTUAL INFORMATION — Namecheap per studio default?]

Deploy steps are the studio standard — see root `CLAUDE.md` → "Deploying a
site (GitHub Pages, same every time)".

## Open questions / decisions log

- 2026-09-21 — Built full first draft from the client's design brief with
  placeholders for all unverified facts. Needs: real bio/CV, real
  publications list, real contact links, confirmed working title for the
  sundown-towns project (used "Mapping the Afterlife of Sundown Towns" as a
  placeholder working title), confirmed domain/repo name.
- 2026-09-23 — Added the client's real portrait photo to the hero
  (`assets/portrait-leia-belt.webp`), background removed. The automated
  cutout has some residual color fringing in the hair from the original
  busy painted backdrop (a hard case for any background-removal tool without
  a plain backdrop) — usable now, but worth a professional retouch or a
  reshoot against a plain background before public launch. See the
  `[VERIFY BEFORE PUBLISHING]` caption under the portrait.
