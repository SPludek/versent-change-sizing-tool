[README (1).md](https://github.com/user-attachments/files/28865514/README.1.md)
# Versent Change Sizing Tool

**Business Strategy – OCM Practice**

A change complexity scoring tool built for Versent's OCM practice. Stop guessing the size of your change program. Answer 12 questions across four dimensions and get an instant complexity score, risk profile, recommended package, and indicative investment range — before scoping begins.

---

## What it does

The tool walks through 12 questions across four dimensions:

- **Scale & Reach** — how many people, locations, and roles are affected
- **Nature of Change** — what is changing, how significantly, and how fast
- **Organisational Readiness** — leadership sponsorship, change fatigue, and track record
- **Internal Capability** — in-house change skill, stakeholder complexity, and training load

From those inputs, it outputs:

- An overall complexity score (out of 48) with a Low / Medium / High band
- A dimension-by-dimension risk breakdown
- A recommended engagement level: Advisory, Packaged Delivery, or Design & Delivery
- An indicative investment range, typical duration, and FTE requirement
- Automatically triggered risk flags for high-stakes conditions (e.g. absent sponsorship, compressed timeline)

---

## How to use it

This is a single self-contained HTML file. No dependencies, no build step, no server required.

1. Download `versent-change-sizing-tool.html`
2. Open it in any modern web browser
3. That's it

To share it internally, host it on any static file server, SharePoint, Confluence, or GitHub Pages.

---

## GitHub Pages (quick hosting)

If you want a shareable URL:

1. Go to your repo **Settings → Pages**
2. Set source to **Deploy from a branch → main → / (root)**
3. Your tool will be live at `https://[your-username].github.io/[repo-name]/versent-change-sizing-tool.html`

---

## Customisation

All content is in a single HTML file. Common things you might want to update:

| What | Where in the file |
|---|---|
| Hero statistics | Search for `hero-stat` |
| Question text or options | Search for `question-block` |
| Score thresholds (Low/Medium/High bands) | Search for `total <= 18` in the script |
| Package names and deliverables | Search for `pkg =` in the script |
| Budget ranges | Search for `budgetLow` and `budgetHigh` |
| Brand colours | CSS variables at the top of the `<style>` block |
| Contact or footer link | Search for `versent.com.au` in the footer |

---

## Scoring model

Each of the 12 questions is scored 1–4. Maximum score is 48.

| Band | Score | Recommended Level |
|---|---|---|
| Low Complexity | 12–18 | CM Advisory Package |
| Medium Complexity | 19–30 | CM Packaged Delivery |
| High Complexity | 31–48 | CM Design & Delivery |

Risk flags fire automatically based on specific answer combinations regardless of overall score — for example, absent leadership sponsorship or a compressed timeline on a high-complexity program.

---

## Built with

Plain HTML, CSS, and vanilla JavaScript. No frameworks, no libraries, no external dependencies. Runs entirely in the browser.

---

## Versent

Versent is an Australian-born technology company, built in the cloud and engineered for outcomes. We architect, build, and operate cloud-native applications, data streams, platforms, and services for Australia's leading enterprises.

[versent.com.au](https://versent.com.au)
