# Jules Tier Search — Android Home-Screen Web App

**[Open the live app](https://turtle328.github.io/bazaar-item-rankings/)**

**What it is:** An instant-search, mobile-first reference for all 120 Jules items from the Unduel Season 20 tier list (November 4, 2026). This is a fixed snapshot; it does not automatically sync future ratings.

## Test it right now (no hosting)
Open `index.html` in a web browser. Search works even without a network connection. For the best Android home-screen experience, use the hosted PWA instructions below.

## Put it on your Android home screen (free)
1. Create a public GitHub repository, such as `jules-tiers`.
2. Upload the **contents** of this ZIP (not the ZIP itself) into the root of the repository. Preserve the `icons` folder.
3. In the GitHub repo: **Settings → Pages → Build and deployment → Deploy from a branch → main → /(root) → Save**.
4. Open the GitHub Pages URL shown in Settings → Pages, usually `https://YOURUSERNAME.github.io/jules-tiers/`, in Chrome on your Android phone.
5. In Chrome's menu, choose **Install app** or **Add to Home screen** (wording may vary).
6. Open it once while online to cache the app; afterwards it works offline.

## Updating the data
Open `index.html`, find the `const DATA=` assignment, and replace its JSON array with new `{ "name": "...", "tier": "..." }` objects. Then bump the cache ID in `sw.js`, redeploy, and revise the snapshot date on the page.

Source: https://unduel.com/u/bazaardb/jules-items-the-bazaar-xk4xys8GR2Xky27m8C9ES/tier-list
