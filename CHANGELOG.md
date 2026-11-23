# Changelog

All notable changes to this project are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [v1.4.0] - 2026-11-23

### Changed
- Switched the GitHub Pages theme from **Cayman** to **[Just the Docs](https://just-the-docs.github.io/just-the-docs/)** (`just-the-docs/just-the-docs@v0.12.0`) for a more professional, documentation-style layout.
- Replaced the theme-specific stylesheet with a Just the Docs custom hook (`_sass/custom/custom.scss`), preserving the custom comparison-table styling (blue header, Kubernetes column highlight, sticky headers, zebra rows).

### Added
- **In-page Table of Contents**: enabled Just the Docs' built-in `toc` so readers can jump to any of the 14 section headings.
- **Table expand / fullscreen feature**: an "Expand table" button above every comparison table opens it in a full-width modal (close via button, backdrop, or `Esc`). Implemented with vanilla JS in `_includes/footer_custom.html`.

### Fixed
- Enabled the `jekyll-include-cache` plugin, required by Just the Docs (and Minimal Mistakes) on GitHub Pages.
- Resolved a build error by placing custom CSS in the correct Just the Docs hook (`_sass/custom/custom.scss`) instead of overriding `assets/css/just-the-docs.scss`.
- Removed `//` line comments from the inline expand-table script, which GitHub Pages/Just the Docs HTML minification was corrupting into a `SyntaxError`.

### Notes
- Revert points preserved as git tags:
  - `checkpoint-1` — original Cayman theme (v1.4.0 content).
  - `checkpoint-mm` — Minimal Mistakes theme state.

---

## [v1.4.0] - 2026-11-23

### Changed
- Updated the cloud service comparison for late-2026 developments: Amazon Nova 2 / Nova Forge & AWS assistant, AWS Graviton5 / Trainium3 and Google 8th-gen TPUs, KubeVirt & Kyverno CNCF graduations, Google's Wiz acquisition, and the Azure Stack → Azure Local rebranding.