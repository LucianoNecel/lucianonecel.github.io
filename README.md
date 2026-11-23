# lucianonecel.github.io

**Retired.** This repository used to serve the public product page for **Hiraeth**, a Discord bot
developed by Necel. The product page now lives in the `Hiraeth` repository itself, served by the
bot's own web surface:

- Spanish: <https://hiraeth-kb6c.onrender.com/es>
- English: <https://hiraeth-kb6c.onrender.com/>

`index.html` is a redirect shell: a `<meta http-equiv="refresh">` plus `rel="canonical"` pointing at
the Spanish home, so inbound links and search results from the old page land on the page that is kept
up to date. Nothing else is published from here.

## Why it was retired

The page carried its own copy of the prices, the quota table and the module list. Keeping a second
public copy of those numbers in sync with the bot's catalog was a manual step that had already drifted
(the yearly plan was advertised at a price the catalog no longer had), and a public page quoting a
price the checkout does not charge is worse than no page at all.

The legal documents are unaffected: the Privacy Policy and the Terms of Service live in the separate
`hiraeth-legal` repository and are served at <https://lucianonecel.github.io/hiraeth-legal/>, which
does not depend on this repository.

## Rules for editing

1. Do not restore the product page here. Product copy belongs to the `Hiraeth` repository, where the
   prices come from `listPlans()` and never from a literal.
2. Keep `index.html` to a redirect plus the plain links above; it must work with scripting disabled.
3. Point changes at `main` and push; Pages republishes within a minute.
