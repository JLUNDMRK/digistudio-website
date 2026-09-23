# DigiStudio website

Static site for [digistudio.jlundmark.org](https://digistudio.jlundmark.org).
Deployed with **Cloudflare Pages** (no build step).

## Downloads

| File | Notes |
|------|--------|
| `downloads/DigiStudio-macOS.zip` | From `fld-player` `apple/package_macos.sh` |
| `downloads/DigiStudio-windows.zip` | Build on Windows with `build.bat`, zip the exe + assets |

## Deploy

```bash
npx wrangler pages project create digistudio-website --production-branch=main
npx wrangler pages deploy . --project-name=digistudio-website --branch=main
# Custom domain in dashboard or:
# npx wrangler pages domain add digistudio.jlundmark.org --project-name=digistudio-website
```
