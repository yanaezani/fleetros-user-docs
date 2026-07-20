# Fleetros User Documentation

Fleetros user documentation site, built with [Hugo](https://gohugo.io/) and the [Docsy](https://www.docsy.dev/) theme.

**Live site:** https://yanaezani.github.io/fleetros-user-docs/

## Local Development

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) v0.110.0 or later
- [Go](https://go.dev/doc/install) 1.21 or later

### Run locally

```bash
git clone https://github.com/yanaezani/fleetros-user-docs.git
cd fleetros-user-docs
hugo server
```

Open http://localhost:1313/fleetros-user-docs/ in your browser.

### Build

```bash
hugo --minify
```

Output will be in the `public/` directory.

## Deployment

This site auto-deploys to GitHub Pages via GitHub Actions on every push to `main`.

To enable:
1. Go to **Settings > Pages** in your GitHub repo
2. Under **Build and deployment**, set Source to **GitHub Actions**
3. Push to `main` — the workflow will build and deploy automatically

## Project Structure

```
content/
└── docs/
    ├── _index.md                    ← Docs landing page
    ├── introduction.md              ← 1. Introduction
    ├── logging-in.md                ← 2. Logging In
    ├── dashboard.md                 ← 3. Dashboard
    ├── vehicle-management.md        ← 4. Vehicle Management
    ├── booking-management.md        ← 5. Booking Management
    ├── accident-management.md       ← 6. Accident Management
    ├── offerings-management.md      ← 7. Offerings Management
    ├── discount-management.md       ← 8. Discount Management
    ├── payment-management.md        ← 9. Payment Management
    ├── customer-management.md       ← 10. Customer Management
    ├── liability-reduction-options.md ← 11. Liability Reduction Options
    ├── settings.md                  ← 12. Settings
    ├── global-interface-elements.md ← 13. Global Interface Elements
    └── support-and-resources.md     ← 14. Support and Resources
```
