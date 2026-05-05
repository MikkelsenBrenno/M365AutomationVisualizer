# M365 Automation Architecture Explorer

Live site: https://mikkelsenbrenno.github.io/M365AutomationVisualizer/

Interactive playbooks for IT architects and Power Platform consultants — explore
best-practice architectures, licensing, and technologies for the most common
Microsoft 365 automation scenarios.

This branch contains the production build of the static site. The source is
maintained on Replit; rebuilding regenerates the `assets/`, `index.html`,
`404.html`, `.nojekyll`, `favicon.svg`, and `opengraph.jpg` files in this
directory.

To rebuild from source (Vite + React + Tailwind):

```bash
PORT=5000 BASE_PATH=/M365AutomationVisualizer/ NODE_ENV=production \
  pnpm --filter @workspace/m365-explorer run build
```

Then publish the contents of `dist/public/` to the `main` branch of this repo.
