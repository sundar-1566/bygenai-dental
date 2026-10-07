# Putting the dental demo on bygenai.com

bygenai.com runs on Hostinger Website Builder, which can't serve your own HTML files at a path like `/dental`. `index.html` is a single self-contained file, so either option works.

## Option A: subdomain (recommended), dental.bygenai.com

Use this if your Hostinger plan includes web hosting (hPanel shows **Websites → Add website** or **File Manager**).

1. hPanel → **Domains → Subdomains** → create `dental` under bygenai.com.
2. hPanel → **Files → File Manager** → open the new subdomain's folder (e.g. `public_html/dental` or `domains/dental.bygenai.com/public_html`).
3. Upload `index.html`.
4. Wait for SSL: hPanel → **Security → SSL** → install/enable for `dental.bygenai.com` (usually automatic within ~15 min).
5. Open https://dental.bygenai.com and check that it loads.
6. Add it to the main site's menu: Website Builder → **Pages and navigation → Add link** → name `Dental AI`, URL `https://dental.bygenai.com/` → Publish.

If you use a different URL, update `canonical`, `og:url` and the "Dental AI" nav link in `index.html` (search for `dental.bygenai.com`).

## Option B: page inside the Website Builder (builder-only plans)

1. Website Builder → **Pages and navigation → Add page → Blank page**, name it `Dental AI` (URL `/dental-ai`).
2. Add element → **Embed code**, then paste the full contents of `index.html`.
3. Stretch the embed block to full width and drag its height until nothing is cut off (about 5200 px on desktop). Check mobile view in the builder (about 7600 px) and adjust there too.
4. The builder adds its own header and footer, so you'll see two navs. Delete the `<header class="site">…</header>` block from the pasted code to avoid that.
5. Publish.

The embed runs inside a fixed-height frame. That's why Option A looks and behaves better, especially on phones.

## After it's live
- Test "Book a 20-minute call" (Google Calendar link) and the email link.
- Share https://dental.bygenai.com in LinkedIn/Slack to check the preview card.
