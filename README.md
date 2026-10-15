# Yahtzee

A tiny two-friends Yahtzee for iPhone. One file (`index.html`), no build, no dependencies.

- **Solo**: chase your best score (saved per name on that phone).
- **Together**: two players pass one phone back and forth.
- Names are remembered, and an unfinished game resumes if you close the page.

## Put it online with your domain

1. Create a new GitHub repo and upload `index.html`, `icon.png` and `README.md` to the `main` branch.
2. Repo **Settings → Pages**: Source = *Deploy from a branch*, Branch = `main`, folder = `/ (root)`.
3. Still in Pages, enter your domain (for example `yahtzee.yourdomain.com`) under **Custom domain**. GitHub creates the `CNAME` file for you.
4. At your DNS provider, add a `CNAME` record: name `yahtzee` (or `www`), value `<your-github-username>.github.io`.
   (For a bare domain like `yourdomain.com`, use GitHub's four `A` records instead; see GitHub's Pages docs.)
5. When the check passes, tick **Enforce HTTPS**.

## On the iPhone

Open the site in Safari, tap Share, then **Add to Home Screen**. It opens full screen like an app.

## Rules implemented

Standard scoring, 35-point bonus at 63+ in the upper section, +100 for each extra Yahtzee (when the Yahtzee box holds 50), with Joker rules for forced placement.
