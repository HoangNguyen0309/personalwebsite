## Personal Website Plan

### Objective
- Keep Hoang Nguyen’s single-page resume site crisp, up-to-date, and easy to maintain while preserving the current visual identity.
- Capture the outstanding work items so every change is deliberate rather than exploratory.

### Baseline
- `index.html` already houses the single-page layout, nav anchors, hero, experience, projects, skills, and a static resume download.
- Styling is inline, using `:root` variables for the dark theme and the Space Grotesk font.
- External assets include the downloadable PDFs in the root and a GitHub contribution heatmap image.

### Key deliverables
1. Update textual content where necessary to reflect the latest academic timeline and internships that appear on `resume.txt`.
2. Ensure the structure and styles remain responsive and accessible across breakpoints, especially the nav, hero, and card grids.
3. Keep the resume download flow healthy (PDF link + contact CTA) and confirm any referenced files (`HoangNguyen_Resume.pdf`, `resume.txt`, etc.) still exist.
4. Codify a simple testing/checklist routine so future tweaks do not regress layout or links.

### Work plan
1. **Content audit** – Compare `index.html` against `resume.txt` and any updated requirements (e.g., expected graduation, internships). Adjust copy, dates, and badges in the hero, experience, and education sections so they match the latest resume.
2. **CSS cleanup** – Keep the inline style tidy by grouping related rules (nav, hero, cards) and double-check responsive overrides under `@media (max-width: 640px)` to ensure spacing and button placement still feel natural after copy edits.
3. **Navigation & accessibility** – Confirm every nav anchor targets an existing section ID and that interactive elements (buttons/links) have meaningful labels/aria attributes. Add a visible focus style if the current scheme hides focus outlines.
4. **Project & skills clarity** – Validate that every project card has a short summary/pill/text and that technical skills reflect current focus areas (JavaScript/TypeScript + backend + ML tooling). Remove or reword outdated entries.
5. **Resume delivery** – Test the hero CTA buttons (email, GitHub, download PDF) to ensure they still target correct protocols/URLs. Verify the `HoangNguyen_Resume.pdf` file is present and referenced consistently.
6. **Testing & launch checklist** – Plan a quick manual QA (open in Chromium/Edge, mobile width) to verify layout, nav behavior, and downloadable assets work as expected before publishing the final version.

### Risks / Next steps
- Inline styling means future additions may feel crowded; consider migrating to a separate stylesheet once more sections are added.
- Keep `package.json` minimal until any tooling (e.g., build pipeline) is introduced.
- Once this plan is implemented, document any new decisions in `plan.md` so the next pass starts from a clear baseline.
