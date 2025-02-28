<p align="center">
    <img src="assets/logo.png" width="35%" align="center" alt="logo">
</p>

# Pelican Bay Tennis Groups Website

This is the website for Pelican Bay Tennis Groups, built with Hugo and the Dot Org Hugo Theme.

## Structure

The website consists of two repositories:

1. **Main Website Repository** (this repo) - Contains the Hugo site configuration, layouts, and theme
2. **Content Repository** - Contains just the content (text and PDFs) that gets synchronized to this repo

## Development

### Prerequisites

- Hugo (extended version)
- Node.js and npm

### Running Locally

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

### Build

```bash
# Build for production
npm run build
```

## Content Updates

All content updates should be made in the separate content repository. That repository uses GitHub Actions to automatically sync changes to this repository.

## How It Works

1. The content repository contains:
   - Markdown files for website content
   - PDF files for tennis pairings
   - GitHub Actions workflow to sync with the main repo

2. When content is updated, GitHub Actions copies the files to the content directory in this repository

3. The website displays a list of tennis pairings using a custom shortcode that reads the PDF files

## Customization

- Edit `config/_default/hugo.yaml` to change site configuration
- Edit `config/_default/params.yaml` to change site parameters
- Edit layout files in `layouts/` to customize the site appearance
- Add custom CSS in `assets/scss/`

## Deployment

The site is deployed to GitHub Pages. Any push to the main branch triggers a deployment.
