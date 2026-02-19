# Website Progress & TODO

## Completed

### Profile & Identity
- [x] Replaced Einstein placeholder photo with real headshot (`Headshot_1_2022.jpeg`)
- [x] Added ORCID ID (`0000-0003-1640-9620`)
- [x] Updated site keywords with quantum computing / tensor networks
- [x] Fixed `socials.yml`: correct email, scholar ID, removed Einstein custom social & inspirehep
- [x] Removed RSS icon (not useful for academic site)

### About Page (Bio)
- [x] Rewrote bio from personal research exploration perspective
- [x] Removed over-emphasis on UMN/SAFL/advisor
- [x] Profile photo moved to left side
- [x] Removed "Minneapolis, MN, USA" from sidebar

### CV
- [x] Extracted LaTeX CV package from `CV___Han_Liu.zip` into `assets/cv/`
- [x] Compiled CV with tectonic (switched biblatex backend from biber to bibtex)
- [x] Output PDF placed at `assets/pdf/Han_Liu_CV.pdf`
- [x] CV page now links to real PDF (was `example_pdf.pdf`)
- [x] Enriched `_data/cv.yml` with: IBM Qiskit certificate, thesis titles, 15 presentations (was 6), peer review journals (PRL, JFM, GRL, etc.), APS/AGU memberships, session chair service, Guardian media coverage, detailed skills, richer job descriptions

### Publications
- [x] Added Weems et al. (2022) conference paper to `papers.bib`
- [x] Updated `_data/venues.yml` with real journals (JFM, JCP, PoF, PRE, PRF, IJMF, RE, AAMM)

### News
- [x] Added APS DFD 2024 presentation (quantum-inspired solver)
- [x] Added APS Global Summit 2025 presentation (quantum tensor networks)

### Research Figures
- [x] Downloaded/copied 10 figures from Dropbox to `assets/img/research/`:
  - `ventilated_cavity.jpg` — graphical abstract
  - `ventilated_cavity_vortex.png` — vorticity field
  - `covid_restaurant.png` — restaurant setup diagram
  - `covid_concentration.png` — 3D particle concentration
  - `oil_spill.png` — simulation configuration
  - `canopy.png` — canopy flow snapshot
  - `richtmyer_meshkov.jpg` — SGS energy flux
  - `compressible_turbulence.jpg` — dilatation field
  - `shock_turbulence.jpeg` — shock-turbulence interaction
  - `quantum_tensor.png` — DNS flow field from tensor network solver

### Template Cleanup
- [x] Removed 31 template blog posts (kept only real CFD post)
- [x] Removed template pages: `about_einstein.md`, `dropdown.md`
- [x] Fixed `profiles.md` (removed reference to deleted Einstein file)
- [x] Removed template images: `brownian-motion.gif`, `wave-mechanics.gif`
- [x] Replaced `_data/repositories.yml` with `hanliu-cfd`
- [x] Replaced `_data/coauthors.yml` with real collaborators (Shen, Xiao, He, Gao, Hong, etc.)
- [x] Updated `resume.json` with quantum-inspired computing

### Navigation
- [x] Clean nav order: Research (1) > Publications (2) > CV (3) > Blog (4) > Repositories (5)
- [x] Hidden unused pages: projects (duplicate), profiles, teaching, bookshelf

---

## TODO

### High Priority

- [ ] **Upload research videos to YouTube** (unlisted), then embed on project pages:
  | Video | Source (Dropbox) | Size |
  |-------|-----------------|------|
  | Ventilated cavity | `Supercavitation.../Movie 1.mp4` | 26 MB |
  | COVID-19 | `COVID19_2020/Movie_COVID_high_resolution.mp4` | 245 MB |
  | Oil spill | `Oil spill.../oil_high_top view.mp4` | 75 MB |
  | Canopy flow | `Canopy.../Movie_JFM.mp4` | 40 MB |
  | Wave breaking | `Wave breaking/bw3d.mp4` | 12 MB |

- [ ] **Update project pages** (`_projects/*.md`) to use the new figures in `assets/img/research/` and embed YouTube videos once uploaded

- [ ] **Add a real profile photo** to the LaTeX CV (current `assets/cv/profile.png` is a stylized icon)

### Medium Priority

- [ ] **Add publication preview images** to `assets/img/publication_preview/` for selected papers (currently empty after removing templates)
- [ ] **Write more blog posts** — only one CFD post exists
- [ ] **Add teaching content** if applicable (page is hidden with placeholder)
- [ ] **Update `prof_pic_color.png`** — still the old Einstein image (14MB), either replace or delete

### Low Priority

- [ ] **Set up Google Analytics** if you want visitor tracking
- [ ] **Add project images for remaining projects** (particle-laden flow, turbine — no dedicated figures found)
- [ ] **Configure git user** to avoid the "configured automatically" warning:
  ```bash
  git config --global user.name "Han Liu"
  git config --global user.email "liux3790@umn.edu"
  ```
- [ ] **Run prettier** before deploying (per AGENTS.md pre-commit checklist):
  ```bash
  npm install --save-dev prettier @shopify/prettier-plugin-liquid
  npx prettier . --write
  ```
