Efficiency Labs is an interactive organizational discovery and improvement app. Map processes, assess systems and AI readiness, test workflow scenarios, and track outcomes. 
Includes PMO and change management resources, implementation kit previews, and browser-based progress saving. Built for GitHub Pages.

# Efficiency Labs — GitHub Pages edition

A complete, build-free static site. Cream and olive identity with navy work surfaces, interactive assessment tools, local workspaces, progress missions and a governance simulator.

## Publish on GitHub Pages

1. Create or open the GitHub repository you want to use.
2. Upload the contents of this package to the repository root, preserving the `site` and `.github/workflows` folders. Commit to `main`.
3. Open **Settings → Pages → Build and deployment → Source → GitHub Actions**.
4. Open **Actions → Deploy Efficiency Labs to GitHub Pages**. If needed, select **Run workflow** on `main`.
5. Once deployment succeeds, open the address shown in **Settings → Pages**.

The workflow publishes only `site/`, not this README. No npm install, build command, API keys or Base44 account is required. Hash routes and relative asset paths work on both repository project URLs and custom domains.

If uploading through GitHub's browser interface, ensure `.github/workflows/deploy.yml` is included. Hidden folders may be omitted by file pickers. Alternatively use the site's four public files plus `.nojekyll` at your repository root and choose Pages → Deploy from a branch → main → /(root). Use one publishing method, not both.

Official documentation: https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages

## Preview locally

Open `site/index.html`, or run `python3 -m http.server 8000 --directory site` from this directory and visit http://localhost:8000. HTTP is recommended for reliable browser storage and clipboard behavior.

## Discovery journey update — 2026-10-05

The homepage now leads through process discovery → systems and source authority → readiness → workflow stress testing → contextual next steps and optional blueprints.

New capabilities:
- Interactive five-stage journey and progress rail, saved goal and resume cards.
- Current-state / improved-state reporting comparison (clearly illustrative).
- Source-of-truth register with owners, cadence and reconciliation rules.
- Workflow-discipline rating separate from tool readiness.
- Unknown assessment items retained as unrated discovery gaps, with optional observation and confidence notes. A complete score still requires all 24 ratings.
- Three educational portfolio scenarios with saved discoveries. These do not establish production readiness.
- Proposed portfolio-reporting prerequisites and contextual free next steps / product suggestions. Purchasing never affects scores or completion.
- PMO & Change COE pathway and first-30-days guide.
- Outcome baselines, observations, targets and subsequent updates.
- Existing backup format remains compatible; new discovery fields are included in exported backups.

Edit `site/journey.js` for these enhancements. Keep it after `app.js` in the page. The established six-dimension score and historical results remain unchanged.

## Included

- Homepage, four frameworks, prompt library with copying and filtering.
- 24-question readiness diagnostic, six dimension scores, history and local reports.
- Process mapping with editable/reorderable steps, touch/wait time, rework, visual flow and CSV export.
- Systems inventory with ownership, integration, quality, sensitivity, access and CSV export.
- Opportunity ranking using an explicit value/readiness/effort/risk heuristic.
- ROI calculator with implementation and recurring costs, net value, payback and JSON export.
- Improvement missions, earned milestones and 90-day checklist.
- Local organization/client workspaces, backup export and validated import as separate copies.
- Interactive governance simulation with approvals, rejection, critical escalation, agent toggles and log export.
- Report print / Save as PDF, text download and dynamic executive brief.
- Resources, roadmap, methodology, illustrative case studies, FAQ and privacy disclosures.
- Existing $97 / $149 / $297 Stripe links and package pages.

## Important feature differences from Base44

GitHub Pages is static hosting. This package intentionally does not pretend to implement account authentication, password reset, OAuth, server-side paid report computation, email delivery, payment verification, secure paid-file downloads, cloud storage or team access control. The approved local-browser workspace replaces account-based history. Existing Stripe links continue to send visitors to checkout; the pre-existing fulfillment service must remain operational. Verify its success/return URLs and delivery flow in Stripe before launching this replacement. This package does not modify Stripe settings or validate that fulfillment works.

The free local report is a browser-generated self-assessment. It is distinct from the paid personalized report advertised in the existing package. Paid blueprint assets were not included in the supplied source and are not redistributed in this public site. Existing marketing package descriptions/prices are preserved; confirm the actual product deliverables before release.

Original question/scoring dependencies and many original components were absent. The question bank has been newly authored around the same six dimensions. The original documented formula produced 20–100 for ratings 1–5; this edition explicitly normalizes to 0–100. Old scores are not imported or assumed comparable. Original customer claims were not independently evidenced; case studies are labeled illustrative rather than repeating unsupported quantified claims.

## Data and privacy

Data stays in localStorage under `elabs-workspace-v1` for this origin/browser. It is not encrypted, a database or a multi-user security boundary. Browser clearing/private sessions can remove it. Export backups regularly. Imports preserve existing workspaces and append copies; do not import untrusted files. Exported backups contain all workspaces. No analytics or AI API calls are included. Google Fonts are optional with local fallbacks. Stripe links open externally. No secrets should be placed in this repository or entered into the simulator.

## Editing

- `site/styles.css`: palette, layout, responsive behavior and print styling.
- `site/app.js`: content, questions, product links, tools and local persistence.
- `site/index.html`: shell, metadata and navigation.
- `site/favicon.svg`: brand mark.

No external JavaScript dependency. Reduced-motion preferences, keyboard focus, responsive layouts and print styling are included.

## Blueprint catalogue and drawer — 2026-10-05

A persistent Blueprint button opens a native modal drawer on desktop and mobile. The drawer is outside routed page content, so opening/closing it does not re-render forms or discard in-progress entries. It supports Escape, backdrop dismissal and native modal focus containment. Recommendations appear after eligible results, not inside assessment question flows.

New catalogue previews:
- Current-State Discovery Workshop Kit — proposed $97.
- Portfolio Reporting Standardization Kit — proposed $149.
- PMO & Change COE Launch Kit — proposed $297.

Each has a detailed preview and free downloadable text sample. Full commercial kits have NOT been produced by this site update. The prices are proposed, and the pages explicitly describe the kits as in development. No preorder, waitlist or payment is collected. The email enquiry link opens the visitor's mail application.

