# AI Talent Partner Landing Pages

Static, responsive landing pages for AI Talent Partner / AI Sourcing.

## Pages

- `/` - Intent Router
- `/employers/` - AI Talent Partner for Employers
- `/recruiting-firms/` - AI Sourcing for Recruiting Firms
- `/ats-integration/` - AI Sourcing for ATS
- `/hr-tech/` - AI Sourcing for HR Tech

## Positioning

AI Sourcing is the method. Candidate outcomes are the solution. The site uses progressive disclosure so the first view is concise while technical and process details remain available through expandable sections.

## Local preview

From the repository root:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Deployment

The repository is compatible with GitHub Pages or any static hosting platform.

## GitHub Pages deployment

A GitHub Actions workflow is included at `.github/workflows/pages.yml`.

The workflow is intentionally manual (`workflow_dispatch`) for the initial setup. This avoids failing deployments before GitHub Pages has been enabled for the repository.

One-time setup in GitHub:
1. Open **Settings -> Pages**.
2. Under **Build and deployment**, set **Source** to **GitHub Actions**.
3. Open **Actions**, choose **Deploy static site to GitHub Pages**, and click **Run workflow**.
4. After the first successful run, GitHub will show the published Pages URL.

Once Pages is confirmed working, the workflow can be changed to deploy automatically on every push to `main`.
