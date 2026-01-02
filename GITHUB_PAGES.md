# GitHub Pages Setup

This repository is configured to automatically build and deploy a GitHub Pages site that displays lab exercises.

## How It Works

1. **Jekyll Configuration**: The site uses Jekyll with a custom theme (`MicrosoftLearning/Jekyll-Theme`) configured in `_config.yml`.

2. **GitHub Actions Workflow**: The `.github/workflows/pages.yml` file contains a workflow that:
   - Triggers on pushes to the `main` branch
   - Builds the Jekyll site
   - Deploys it to GitHub Pages

3. **Lab Listing**: The `index.md` file automatically lists all lab exercises found in the `Instructions/Labs/` directory.

## Enabling GitHub Pages

To enable GitHub Pages for this repository:

1. Go to **Settings** → **Pages** in the GitHub repository
2. Under **Source**, select **GitHub Actions** as the deployment source
3. The site will be automatically deployed when changes are pushed to the `main` branch

## Viewing the Site

Once GitHub Pages is enabled, the site will be available at:
```
https://microsoftlearning.github.io/AB-6002-Introduction-to-finance-in-Dynamics-365/
```

## Adding New Labs

To add a new lab exercise:

1. Create a markdown file in `Instructions/Labs/` directory
2. Add the following front matter at the top:
   ```yaml
   ---
   lab:
       title: 'Lab Title Here'
       module: 'Module Name Here'
   ---
   ```
3. The lab will automatically appear on the site after the next deployment

## Manual Deployment

You can manually trigger a deployment by going to **Actions** → **Deploy Jekyll site to Pages** → **Run workflow**.
