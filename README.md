# Ahmed Babundau Ngao – portfolio (Netlify + CMS)

A static site: no build step. All text and images live in `content/site.json` and `assets/`, and you edit them from `/admin`.

## Put it online (free)
1. Create a GitHub account and a new repository (for example `portfolio`). Upload everything inside this folder (drag and drop works) to the `main` branch.
2. On netlify.com choose **Add new project → Import from Git**, pick the repository, leave the build command empty and set the publish directory to `.`. Deploy.
3. In Netlify open **Project configuration → Identity**, enable it, set registration to **Invite only**, and enable **Git Gateway** (Services).
4. Invite your own email under Identity, accept the email, and set a password.
5. Open `https://YOUR-SITE.netlify.app/admin/`, sign in, and edit. Saving publishes by committing to GitHub, so the site updates in about a minute.
6. Contact form: in **Forms → Form notifications** add an email notification to your Gmail. Messages also show in the Forms tab.
7. Domain (optional): add a custom domain under **Domain management**, then replace `YOUR-DOMAIN.com` in `sitemap.xml`, `robots.txt` and `admin/config.yml`, and in `index.html` change the og:image to a full address, e.g. `https://yourdomain.com/assets/og-image.jpg`.
8. Submit `https://yourdomain.com/sitemap.xml` in Google Search Console.

Check Netlify's current Identity and Git Gateway steps if a menu name has changed.

## Notes
- Use a YouTube or Vimeo link for videos; large video files do not belong in Git.
- Test locally with `npx serve` (opening index.html directly will not load the content file).
- Files: `index.html`, `css/style.css`, `js/app.js`, `content/site.json`, `admin/` (CMS), `assets/` (images, CV), `netlify.toml`, `robots.txt`, `sitemap.xml`.
