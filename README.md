# devops-lab1-portfolio

Lab 1 — DevOps Course: My First CI/CD Pipeline

## Project Structure

```
devops-lab1-portfolio/
├── .github/
│   └── workflows/
│       └── deploy.yml    ← CI/CD Pipeline definition
├── index.html            ← Static portfolio website
└── README.md
```

## How it Works

1. **Push code** to `main` branch
2. **GitHub Actions** automatically runs the pipeline
3. **Validates** HTML file exists
4. **Deploys** to GitHub Pages (branch `gh-pages`)
5. **Website live** at `https://<USERNAME>.github.io/devops-lab1-portfolio/`

## Setup GitHub Pages

1. Go to repo **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: `gh-pages` → `/ (root)` → **Save**
4. Wait 1-2 minutes for URL to appear

## Trigger Pipeline

```bash
git add .
git commit -m "feat: portfolio page + GitHub Actions CI/CD pipeline"
git push origin main
```

Then watch the **Actions** tab for pipeline execution.