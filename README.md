# AI CV Shortlisting & Ranking Tool

A general-purpose AI recruitment screening demo that lets a user upload **one job description** and **multiple CVs**, then ranks candidates using an evidence-based scoring rubric.

## Live Demo

After enabling GitHub Pages, your live URL will look like:

```text
[https://YOUR-USERNAME.github.io/YOUR-REPOSITORY-NAME/](https://pranaypoojari23.github.io/CV-Ranking-Assistant/)
```

## What It Does

- Upload a single JD in PDF, DOCX, or TXT format
- Upload multiple CVs in PDF, DOCX, or TXT format
- Extract text directly in the browser
- Analyse each CV against the JD using an AI model
- Score candidates across five dimensions:
  - Skills Match
  - Relevant Experience
  - Education & Certifications
  - Role Alignment
  - Ownership & Impact
- Rank candidates from highest to lowest score
- Categorise candidates into:
  - `SHORTLIST`
  - `MAYBE`
  - `REJECT`
- Export results as CSV or JSON

## Important Security Note

This is a **front-end GitHub Pages demo**. Do **not** hardcode your API key into the code.

The app provides a runtime field where you can paste your API key. For a real production tool, move the API call to a backend or serverless function so the key is never exposed in the browser.


## Demo Mode

The app includes a **Load Reward Analyst Demo** button. This loads sample results for a Reward Analyst / Global Compensation and Benefits Specialist role using one real sample profile and multiple dummy candidate profiles.

Use this mode when presenting the project on GitHub Pages so you can demonstrate the ranking, shortlisting, detailed scoring, CSV export and JSON export without repeatedly calling the AI API.

## How to Use

1. Open `index.html`.
2. Enter your OpenAI API key in the credentials field.
3. Add a role title.
4. Upload one job description.
5. Upload multiple CVs.
6. Click **Analyse & Rank Candidates**.
7. Review ranked results.
8. Export results as CSV or JSON if needed.

## Recommended GitHub Pages Setup

1. Create a new GitHub repository.
2. Upload `index.html` and `README.md`.
3. Go to **Settings** → **Pages**.
4. Under **Build and deployment**, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
5. Save and wait for GitHub to publish the site.

## Tech Stack

- HTML
- CSS
- JavaScript
- PDF.js for PDF text extraction
- Mammoth.js for DOCX text extraction
- OpenAI Responses API for AI scoring and structured JSON output

## Human-in-the-Loop Disclaimer

This tool is designed to support recruitment screening, not replace human judgement. Final decisions should always be reviewed by a recruiter or hiring manager.

## Data Privacy

CVs and JDs may contain personal information. Use sample CVs for public demonstrations. Do not process real candidate data unless you have permission and a clear privacy basis.
