# Sterling Commercial Solutions — Astro Landing Site

Short static website built with Astro. Simple company landing page showcasing Sterling Commercial Solutions identity and industrial cleaning services.

## Features

-   Fast, accessible static site (Astro).
-   Single-page landing layout: hero, services, about, contact.
-   Image assets and SEO metadata.
-   Easy to customize and deploy to Vercel / Netlify / GitHub Pages.

## Prerequisites

-   Node.js 16.14+ (Node 18+ recommended)
-   npm, yarn, or pnpm
-   Git (for cloning and deployment)

## Quick start

1. Clone repository
    ```
    git clone <repo-url> .
    ```
2. Install dependencies
    ```
    npm install
    # or
    yarn
    # or
    pnpm install
    ```
3. Start dev server
    ```
    npm run dev
    ```
    Visit http://localhost:3000 (or port shown by Astro).

## Project structure

-   astro.config.mjs — Astro configuration
-   package.json — scripts and deps
-   public/ — static assets (images, favicon)
-   src/
    -   pages/ — routes and page templates (index.astro)
    -   components/ — UI components (Hero, Services, Footer)
    -   layouts/ — shared layouts
    -   styles/ — global CSS or Tailwind config

## Development commands

-   Dev server
    ```
    npm run dev
    ```
-   Build for production
    ```
    npm run build
    ```
-   Preview production build locally
    ```
    npm run preview
    ```

Example package.json scripts

```
"scripts": {
  "dev": "astro dev",
  "build": "astro build",
  "preview": "astro preview",
  "format": "prettier --write ."
}
```

## Building the production product (static site)

1. Ensure content and assets are finalized (src/pages, public images).
2. Optimize images (use compressed formats, generate responsive sizes).
3. Run build
    ```
    npm run build
    ```
    Output will be in the `dist/` folder (or the adapter-specific output).
4. Validate locally
    ```
    npm run preview
    ```
5. Deploy the `dist/` output or use platform integration (see below).

## Deployment

-   Vercel: connect repo, automatic build (Astro supported).
-   Netlify: set build command `npm run build`, publish directory `dist`.
-   GitHub Pages: push `dist` to gh-pages branch or use an action to deploy.
-   CI: ensure Node version matches local dev and run install → build → deploy.

## Content & customization

-   To edit the landing content, modify `src/pages/index.astro` and components in `src/components/`.
-   Replace images in `public/` and update metadata in page head for SEO.
-   Add services as data files (JSON/YAML) or as component props for easy updates.

## Accessibility & SEO notes

-   Use semantic HTML, alt attributes for images, and proper heading order.
-   Add meta description, OpenGraph tags, and structured data where appropriate.
-   Ensure color contrast and keyboard navigability for accessibility.

## Contributing

-   Create a branch per feature.
-   Run format and lint before committing.
-   Open a pull request with a brief description and screenshots if applicable.
