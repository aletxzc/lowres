# Web first, iOS later, in one monorepo

Lowres ships first as a PWA hosted on GitHub Pages, and a native Swift iOS app comes later. Both live in this one repository (`web/` now, `ios/` later). Web goes first because it runs on any phone (including iPhone, via Add to Home Screen), can be developed from Windows, and gives every pull request a testable HTTPS preview; tuning the Effects there once makes the later port to Metal straightforward. A single repository keeps one issue tracker and lets both apps share the same Model recipes (see ADR-0001).

## Considered Options

- **Native iOS first**: rejected because development happens on Windows and iOS distribution has recurring costs, while the PWA already installs on an iPhone.
- **One repository per app**: rejected because the Model recipes, issues and roadmap would be split across two places.
