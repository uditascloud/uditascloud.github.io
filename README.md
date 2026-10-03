# Udita Sen: portfolio site

A single-page portfolio. Plain HTML and CSS, no build step, hosted free on GitHub Pages.

## Files

- `index.html`: the whole site
- `resume.pdf`: linked from the site (replace it with the latest resume, same file name)
- `.nojekyll`: tells GitHub Pages to serve the files as they are

## Publish it free on GitHub Pages (about 10 minutes)

1. Sign in to GitHub as `uditascloud`. The username becomes the web address.
2. Create a new **public** repository named exactly `uditascloud.github.io`.
3. Click **Add file → Upload files**, drag in `index.html`, `resume.pdf` and `.nojekyll`, then click **Commit changes**.
   (If `.nojekyll` is hidden on your computer, skip it. The site still works.)
4. Go to **Settings → Pages**. Under "Build and deployment", set Source to **Deploy from a branch**, branch **main**, folder **/ (root)**, and save.
5. After a minute or two the site is live at `https://uditascloud.github.io`.

## Before sharing it

Open `index.html` in any text editor and fill in the links near the bottom:

```js
const LINKS = {
  "LinkedIn": "https://www.linkedin.com/in/...",
  "GitHub": "https://github.com/uditascloud",
  "LeetCode": "https://leetcode.com/u/user4137q/",
  "Resume": "resume.pdf"
};
```

Any link left as `""` is hidden automatically.

Also consider:

- **Phone number**: the site leaves it out, but `resume.pdf` includes it. Upload a copy without the phone number if you'd rather not publish it.
- **Visa line**: if you need sponsorship, add it to the status pill at the top ("Open to relocation · UK & Australia").

## Company logos

Oracle and PayPal logos are built into the page. HashedIn and MAKAUT show a letter badge; to show their logos, create a `logos` folder in the repo and upload square PNGs named `logos/hashedin.png` and `logos/makaut.png`. The page picks them up automatically.

## Updating later

Edit `index.html` on GitHub (pencil icon) and commit. Changes go live within a minute or two.

## Adding a custom domain later

Buy the domain (for example `uditasen.com`), then in **Settings → Pages → Custom domain** enter it, and at the registrar add four A records for `@` pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`, plus a CNAME for `www` pointing to `<username>.github.io`. Tick **Enforce HTTPS** once it works.
