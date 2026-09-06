# RecompileX Portfolio Implementation Plan

**Goal:** Build and publish Hamza Kamal's approved portfolio and prepare the domain fork without submitting a PR.

**Architecture:** A static HTML/CSS site with no build step. GitHub Pages serves the root of the main branch. The registration fork contains only the domain configuration change.

**Tech Stack:** HTML, CSS, GitHub Pages.

**Spec:** ../specs/2026-09-05-portfolio-design.md

## Global constraints

- Exact name: Hamza Kamal.
- Exact description: Building systems from the ground up.
- Include only the four verified public projects.
- No upstream pull request.

## Steps

- [ ] Create `index.html`, `styles.css`, `favicon.svg`, `.nojekyll`, and `README.md`. Include project links and the public wildfire screenshot.
- [ ] Check relative resources, anchor targets, viewport behavior, keyboard accessibility, and screenshots using Edge headless if available. This is a static presentation change; no unit-test suite is needed.
- [ ] Initialize a separate repository, commit the portfolio, create `RecompileX/RecompileX.github.io`, push main, and enable Pages.
- [ ] Update the existing fork's domain file to `records.CNAME = recompilex.github.io`, preserving the exact name and description.
- [ ] Verify the published site, remote file, and absence of upstream PRs.
