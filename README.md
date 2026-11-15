# Fuel Plan

Low-FODMAP shopping list, Sunday prep, daily plan and recipes for half-marathon training.
A static, installable web app: no build step, no dependencies, works offline, ticks are saved on the device.

## Publish on GitHub Pages

1. Create a new repository (for example `fuel-plan`) on github.com.
2. Upload everything in this folder to the repository root (index.html, manifest.webmanifest, sw.js, icons/).
3. Repository Settings > Pages > Build and deployment > Source: "Deploy from a branch", Branch: `main`, folder `/ (root)`, Save.
4. After a minute the app is live at `https://<your-username>.github.io/fuel-plan/`.
5. On your phone, open that link and choose "Add to Home Screen".

## Edit the plan

All content (days, shopping list, prep steps, recipes, rules) is in the DATA block at the top of the script in `index.html`.
After changing content, bump `CACHE` in `sw.js` (for example `fuelplan-v2`) so installed copies update.
