# Snake Classic+ Site

This folder is ready to publish as a simple static site for GitHub Pages.

## Files

- `index.html` - landing page, support page, and privacy-policy page
- `.nojekyll` - prevents Jekyll processing on GitHub Pages

## Fast Publish Path

1. Create a new GitHub repo for the site, for example `snake-classic-plus-site`
2. Copy the contents of this folder into the root of that repo
3. Push the repo to GitHub
4. In GitHub, open `Settings -> Pages`
5. Set:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
6. Wait for GitHub Pages to publish
7. Use the published `https://...github.io/...` URL in App Store Connect, or connect a custom domain later

## Custom Domain

This site is preconfigured for:

- `apps.legendaryleo.com`

The `CNAME` file is already included. After the repo is pushed and GitHub Pages is enabled:

1. Open GitHub `Settings -> Pages`
2. Confirm the custom domain is `apps.legendaryleo.com`
3. In GoDaddy DNS, add:
   - Type: `CNAME`
   - Name: `apps`
   - Value: `<your-github-username>.github.io`
4. Wait for DNS propagation
5. Turn on `Enforce HTTPS` in GitHub Pages once the certificate is ready

## Before Publishing

The support email has already been set to:

- `support@legendaryleo.com`

You can update the footer date later if needed.
