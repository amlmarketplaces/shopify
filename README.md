# amlmarketplaces/shopify

Claude Code marketplace federating all `@amlplugins/shopify-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-shopify": {
      "source": { "source": "github", "repo": "amlmarketplaces/shopify" }
    }
  },
  "enabledPlugins": {
      "shopify-admin-api@aml-shopify": true,
      "shopify-app-bridge@aml-shopify": true,
      "shopify-billing@aml-shopify": true,
      "shopify-functions@aml-shopify": true,
      "shopify-storefront-api@aml-shopify": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/shopify`, cached under `~/.claude/plugins/cache/aml-shopify/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (6 total)

- `shopify-admin-api` — [@amlplugins/shopify-admin-api](https://github.com/amlplugins/shopify-admin-api)
- `shopify-app-bridge` — [@amlplugins/shopify-app-bridge](https://github.com/amlplugins/shopify-app-bridge)
- `shopify-billing` — [@amlplugins/shopify-billing](https://github.com/amlplugins/shopify-billing)
- `shopify-functions` — [@amlplugins/shopify-functions](https://github.com/amlplugins/shopify-functions)
- `shopify-storefront-api` — [@amlplugins/shopify-storefront-api](https://github.com/amlplugins/shopify-storefront-api)
- `shopify-webhooks` — [@amlplugins/shopify-webhooks](https://github.com/amlplugins/shopify-webhooks)

## Related

- npm packages: `@amlplugins/shopify-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
