# lucianonecel.github.io

Public product page for **Hiraeth**, a Discord bot developed by Necel.

Published at <https://lucianonecel.github.io/> with GitHub Pages (branch `main`, root, legacy
build). This is the site URL used as the product page for the payment provider's integration
review: it shows what the bot is, what the optional paid plan costs, and how it is bought.

## Layout

- `index.html` — single self-contained page (inline CSS, no external assets, no build step).
- `.nojekyll` — serves files verbatim, without Jekyll processing.

## Rules for editing

1. Every claim on the page must match what the bot actually does. Prices, limits and included
   modules are read from the bot's catalog (`src/premium/utils/plans.js`) and quota table
   (`src/shared/utils/premiumQuotas.js`) in the `Hiraeth` repository — update this page in the same
   delivery that changes either of them.
2. The plan is bought from inside Discord with `/premium`; the page never promises a purchase path
   that does not exist in the bot.
3. Legal links point at the canonical documents in `hiraeth-legal`; those pages, not this one, are
   what governs a purchase.
4. Commit to `main` and push; Pages republishes within a minute.
