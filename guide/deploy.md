---
outline: deep
---

# Deploy Your VitePress Site

## Build and Test Locally

1. Run this command to build the docs:

   ```sh
   npm run docs:build
   ```

2. Once built, preview it locally by running:

   ```sh
   npm run docs:preview
   ```

   The `preview` command will boot up a local static web server that will serve the output directory `.vitepress/dist` at `http://localhost:4173`. You can use this to make sure everything looks good before pushing to production.

## Platform Guides

### Netlify

Set up a new project and change these settings using your dashboard:

- **Build Command:** `npm run docs:build`
- **Output Directory:** `.vitepress/dist`
- **Node Version:** `16`

::: tip
Cool.
:::

### Other

VitePress also supports:

- Netlify
- Github Pages
- Vercel
- AWS Amplify
- Render
- GitLab Pages
- Cloudflare Pages
- Firebase Hosting
- Heroku
- Edgio

Look at the docs: <https://vitepress.dev/guide/deploy>
