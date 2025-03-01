<p align="center">
    <img src="assets/logo.png" width="35%" align="center" alt="logo">
</p>

# Pelican Bay Tennis Groups Website

This is the website for Pelican Bay Tennis Groups, built with Hugo and the Dot Org Hugo Theme.

## Development

### Dependencies

This repo uses the following hugo projects, directly commited to the repo as we've modified them:

- <https://github.com/nodejh/hugo-theme-mini>
- <https://github.com/anvithks/hugo-embed-pdf-shortcode>

### Running Locally

```bash
# Start development server
hugo serve
```

### Build

```bash
HUGO_ENV=production hugo build
```

## Content Updates

All content updates should be made in the separate content repository. That repository uses GitHub Actions to automatically sync changes to this repository.

## Deployment

The site is deployed to GitHub Pages. Any push to the main branch triggers a deployment.
