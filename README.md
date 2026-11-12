# APCV 2027 website

One-page save-the-date site for the Asia-Pacific Conference on Vision 2027, Bangkok.
Plain HTML, no build step. Everything is in `index.html`; `og-image.png` is the picture shown when the link is shared.

## Put it online (about 10 minutes, all in the browser)

1. **Create a GitHub organization** (free): github.com → your avatar → *Your organizations* → *New organization* → Free plan.
   Name it `apcv2027` (or whatever is available; the site address follows this name).
2. **Create a repository** in that organization named exactly `apcv2027.github.io` (match the org name). Public.
3. **Upload the files**: in the new repo, *Add file → Upload files*, drag in `index.html`, `og-image.png` and this `README.md`, then *Commit changes*.
4. **Check Pages is on**: repo *Settings → Pages*. Source should be *Deploy from a branch*, branch `main`, folder `/ (root)`.
5. After 1–2 minutes the site is live at **https://apcv2027.github.io**.

If you used a different org name, update the two link-preview URLs near the top of `index.html` (`og:url` and `og:image`).

## Adding a proper domain later

Repo *Settings → Pages → Custom domain*, enter e.g. `apcv2027.md.chula.ac.th` or `apcv2027.org`, then ask whoever manages that domain to add a **CNAME** record pointing to `apcv2027.github.io`. Tick *Enforce HTTPS* once it's available.
The old `apcv2027.github.io` address then redirects automatically, so links already sent out keep working. Update `og:url`/`og:image` to the new domain.

## Editing

Open `index.html` on GitHub, click the pencil icon, edit the text, commit. Changes go live in a minute or two.

- **Key dates**: the `<ul class="dates">` block.
- **Venue**: there's a `TODO` comment where the building/hall name goes.
- **Coming soon list**: the `<ul class="soon">` block; replace "coming soon" with links as things open.
- **Organizing committee**: a commented-out section is ready; uncomment it once everyone has agreed to be listed.
- **Calendar buttons**: dates live in the script at the bottom (search for `20270630`).
- Update the "Last updated" line in the footer when you change content.
