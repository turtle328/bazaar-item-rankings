# Jules Tier Search — Android Home-Screen Web App

**[Open the live app](https://turtle328.github.io/bazaar-item-rankings/)**

**What it is:** An instant-search, mobile-first reference for 122 Jules items: the original 120 from the Unduel Season 20 tier list (November 4, 2026), plus **Flaming Gelato (B tier, personal estimate)** and **Fire Fly Trap (B tier, personal estimate)**. Both estimates are labeled in the app and are **not** part of the community snapshot or its vote totals. Fire Fly Trap was added to the game in Patch 19.0 (October 7, 2026); it was adjusted in Patch 19.3. Rankings do not automatically sync.

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
Open `index.html`, find the `const DATA=` assignment, and replace its JSON array with new `{ "name": "...", "tier": "..." }` objects (or add `"estimated": true` for a personal estimate). Then bump the cache ID in `sw.js`, redeploy, and revise the snapshot date on the page.

Source: https://unduel.com/u/bazaardb/jules-items-the-bazaar-xk4xys8GR2Xky27m8C9ES/tier-list
