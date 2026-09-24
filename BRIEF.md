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
- **Main contact:** drleiabelt@gmail.com (public-facing; confirmed by client)
- **Current institution:** Postdoctoral Scholar, Nicotine &amp; Cannabis Policy
  Center, University of California, Merced (2025–present) — confirmed via CV
  (`CV_Belt_Fall2026_website`, provided 2026-09-23)

This is **not** a Golden Valley Web local-business site. It does not use the
`_template/` SaaS-style scaffold or the studio's three-service positioning —
those apply to GVW's own local-business clients only. This is a fully custom
editorial/academic personal site, built once from the detailed design brief
the client (via Richie) provided in full.

## Content status — read before editing

The client's initial design brief supplied extensive **positioning, tone, and
section-by-section copy direction**, but almost no concrete biographical/CV
data. On 2026-09-23 the client supplied Dr. Belt's actual CV
(`CV_Belt_Fall2026_website.docx`/`.pdf`), which now backs most of the site's
factual content — see the decision log below for exactly what changed. Per
the client's own explicit content rule, still-unverified content keeps the
placeholder convention:
- `[ADD ACTUAL INFORMATION]` — missing facts.
- `[VERIFY BEFORE PUBLISHING]` — facts entered but not yet confirmed.

**Before launch, replace every remaining bracketed placeholder** — search the
file for `[ADD ACTUAL` and `[VERIFY BEFORE`. What's still placeholder after
the CV pass: LinkedIn URL, Google Scholar profile URL, University faculty
profile URL, DOI/full-text links for most publications (only the Dryad
dataset has a confirmed link), teaching philosophy statement, sample syllabi,
findings detail on the maternal-health project card, stewardship model for
the community-data project, quote/target-launch date/domain/DNS registrar.

Copy that **is** real: the client's original headline/subhead/expertise line/
research-philosophy statement/core-research-area descriptions/methods
clusters (from the design brief), plus — from the CV — her degrees and
dissertation, appointment history, publications, grants/fellowships,
presentations, guest lectures, professional societies, software
competencies, and her ORCID (0009-0005-4371-1819) and public contact email
(drleiabelt@gmail.com, confirmed by the client directly, distinct from her
institutional lbelt@ucmerced.edu). Treat all of that as approved, not draft.

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
- 2026-09-23 — Client supplied Dr. Belt's CV (docx, then a cleaner PDF —
  `assets/Belt-CV.pdf` is now the Download-CV target on the page). Used it to
  replace placeholders with real content across: About (fact card + full-story
  training/fellowships/postdoc paragraphs), Professional Experience (full
  5-entry timeline: current postdoc → HERE Lab postdoc → PhD → MA → BS),
  Publications (10 real entries: 2 peer-reviewed, 1 Dryad dataset with a live
  DOI link, 2 commentary, 2 AcademyHealth policy-response reports, 1
  under-review, 2 conference presentations — dropped the "Book Chapters"
  filter since she has none), Selected Projects (all 3 cards now have real
  collaborators/methods/outputs; the maternal-health card's "Findings" field
  is still placeholder — the CV doesn't give published findings text, only
  the conceptual framework), Methods (added her real software competencies:
  STATA/SPSS/R/Gephi, NVivo/Dedoose, Qualtrics, ArcGIS/QGIS/ArcMap), Speaking
  (added a "Selected engagements" list, including her confirmed 2024 keynote
  — safe to call her a keynote speaker now), Teaching (real guest-lecture
  list + real mentorship-program line), Ideas & Perspectives (3 real
  short-form pieces, replacing the empty state), Contact/footer/JSON-LD (real
  ORCID link everywhere, real public email). Still placeholder: LinkedIn,
  Google Scholar, university profile URLs, and DOI/full-text links for most
  publications (the CV lists citations, not URLs, for most of them).
- 2026-09-23 — Client supplied three more real research artifacts, now on
  the page: (1) `assets/POST_sundown.pdf`, a 2-page conference poster,
  "Sundown Towns Sightings by State" (conception &amp; research: Leia Belt;
  visual engineering: Anthony Starks; source: Loewen 2005) — both panels
  rendered to web images (`assets/poster-sundown-map.webp`,
  `assets/poster-sundown-bystate.webp`) and placed in the Featured Research
  media strip, linking out to the full PDF; (2)/(3) two real IRB-style
  recruitment flyers for her ongoing qualitative studies —
  `assets/flyer-photovoice-study.webp` (PhotoVoice study, birth workers) and
  `assets/flyer-key-informant-interviews.webp` (key informant interviews,
  birth-work business owners) — placed in the Participatory & Qualitative
  Research mosaic. These are recruitment materials, not participant data, so
  no consent/privacy concern. Note: the poster's pull-quote is a direct
  historical citation of actual sundown-town warning-sign language (sourced
  to Loewen's book) — displayed as-is since it's Dr. Belt's own real academic
  work, presented the same way standard scholarship in this field presents
  that evidence. Remaining media-strip/mosaic slots are still honest
  placeholders.
