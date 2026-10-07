# dental.bygenai.com

`index.html` is a single self-contained page. It's served free by GitHub Pages from this repo, and bygenai.com itself stays on Hostinger Website Builder.

## One-time setup
1. Hostinger hPanel → **Domains → bygenai.com → DNS / Nameservers → DNS records**. Add:
   - Type `CNAME` · Name `dental` · Target `sundar-1566.github.io` · TTL default
2. Wait for DNS (usually 5–30 min), then go to GitHub → repo **Settings → Pages** and tick **Enforce HTTPS** once it becomes available.
3. Website Builder → **Pages and navigation → Add link** → `Dental AI` → `https://dental.bygenai.com/` → **Publish**.

## Updating the page
Edit `index.html`, then commit and push to `main`. GitHub Pages republishes in about a minute.

Don't delete the `CNAME` file. GitHub Pages reads the custom domain from it.
