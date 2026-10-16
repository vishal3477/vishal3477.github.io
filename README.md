# Vishal Asnani's research website

Jekyll source for <https://vishal3477.github.io/>.

## Updating content

- `_pages/about.md`: biography, selected work, research interests, news, and contact
  information. Recent news comes first, followed by research areas and selected
  publications (four `selected_work` entries). Each entry and its `related` list reference
  publication permalinks; titles, dates, status, and reading links come from the
  corresponding publication files. Set `venue_label` for compact venue names,
  retaining workshop distinctions.
  Keep the problem, approach, and significance summaries grounded in public work.
  News shows the latest five date groups, with five more revealed per click.
  The historical timeline extends back to the CVPR 2022 proactive detection
  acceptance and includes publications, acceptance announcements, talks,
  internships, and career milestones. Preserve month/year and chronological order.
  Without JavaScript, every news item remains visible.
- `_publications/`: one file per publication, with authors, venue, and year.
  Set `authors` for the compact author line, `paperurl` for a verified reading
  link, and optionally `codeurl` for a public code repository. Publication cards
  are rendered by `_includes/publication-card.html`.
  Link published work to its official proceedings or publisher record, including
  supplementary material. Do not cache paper PDFs in `files/`; only the public
  resume downloads belong there. Preprints retain their arXiv links. If an
  accepted paper has no verified proceedings link yet, explicitly label the
  available copy with `paper_label: Public manuscript` rather than implying it is
  the published version.
  Use `status: preprint` for work that has not been peer-reviewed. The publication
  page groups all work by year, newest first, without separating preprints.
  Status labels remain visible on individual cards. Use `status: accepted` and the specific venue
  for accepted papers that have not yet appeared in proceedings.
  Dates used for sorting do not imply an exact
  publication day.
- `_talks/`: talks and tutorials.
  Set `summary` for the card description and `eventurl` / `event_label` for
  recordings or tutorial websites. Preserve existing permalinks when renaming
  titles. Use `date_precision: year` when the event's exact date is unverified.
- `_pages/cv.md`: web CV.
- `files/research-scientist-resume.html`: printable resume source.
- `files/Vishal_Resume.pdf` and `files/Vishal_CV.pdf`: identical current resume
  downloads, retaining both existing public URLs.
- `_config.yml`: sidebar profile, contact information, and site metadata.
- `_layouts/publication.html`: individual paper pages, with reading/code links,
  author highlighting, and optional research-area illustrations.
  For a figure from the paper itself, set `paper_figure` with `image`, `width`,
  `height`, `alt`, `caption`, `source`, and `credit`. This replaces the generic
  illustration on that page and supports enlargement. Credit the exact figure
  and source version; distinguish accepted proceedings, preprints, and authors'
  manuscripts. Keep only the extracted figure image, not a cached paper PDF.
  Numerical highlights must name the table, metric, dataset/setting, and relevant
  trade-offs. Do not substitute variant results or infer personal contributions.
  All 19 publication pages now include paper-derived visuals and grounded
  overviews. Surveys use research takeaways instead of invented aggregate scores;
  antenna pages distinguish simulated bands from measured responses. Figures are
  compact on the page and can be enlarged. Conference figures use proceedings
  copies; the IJCV survey and antenna figures use published articles. Signpost
  uses its explicitly labeled public manuscript, and the deceptions monograph
  figure uses the authors' full manuscript because the available publisher preview
  does not include it. The TPAMI reverse-engineering figure uses the authors'
  July 2023 manuscript. Preserve these version distinctions when updating sources.
- `images/research-*.svg`: original explanatory diagrams, not paper figures or
  experimental results. Set `research_image` and `research_area` on a paper to
  display a labeled illustration.
- `images/favicon.svg` and its raster variants: personal VA monogram icons.

Do not add private immigration documents, unpublished patent details, or internal
research material. Citation counts and h-index are intentionally omitted.

## Preview and publish

Install a Ruby version compatible with the repository's GitHub Pages dependencies,
then run:

```sh
bundle install
bundle exec jekyll serve
```

Open <http://127.0.0.1:4000/> and review the homepage, publications, talks, and CV.
Regenerate both resume PDFs from the printable HTML when changing resume content.
After editing navigation or contact-menu JavaScript, run `npm run build:js` to
regenerate `assets/js/main.min.js`. Install the existing npm dependencies first
if needed. Verify mobile menus, Escape-to-close, and mobile-to-desktop resizing.

To publish, copy the updated source files into your checkout of
`vishal3477/vishal3477.github.io`, inspect the changes, and commit and push using
the personal GitHub account that has write access. Keep the repository's existing
GitHub Pages deployment configuration. Do not upload `_site/`, local gem
directories, browser profiles, or local-only validation files.

If using the accompanying binary patch instead of copying files, apply it from
your clean website checkout:

```sh
git apply --check /path/to/Website_Update_2026-10-14.patch
git apply /path/to/Website_Update_2026-10-14.patch
git diff --check
```

The local content checks cover publication grouping, preserved publication URLs,
the main pages' internal links, contact details, and the two-page public resume.
Favicon references and the web manifest now point to the personal monogram assets.
The CSS explicitly declares UTF-8 so icon glyphs render correctly.