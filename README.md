# Linkr Docs

The documentation site for [Linkr](https://linkrmap.com), built with
[Mintlify](https://mintlify.com).

Linkr is a community-powered connectivity network. This repository contains the public
docs: how Linkr works, the mobile-app guide, the sharing guide, the map guide, and the
public API reference.

> Ground truth: the public map and API cover **New York City only** (78 hotspots) and are
> a curated beta. The mobile app is in **invitation-only beta**. See
> `docs/introduction/status.mdx` — it is the single source of truth for what is available.
> Keep every other page consistent with it.

## Structure

- `docs.json` — navigation, theme, and API reference configuration
- `docs/` — all documentation pages (`.mdx`)
- `docs/api-reference/` — API pages and `openapi.json` (the read-only public API)
- `images/`, `logo/`, `favicon.svg` — brand assets

## Local development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint):

```
npm i -g mint
```

Run a local beta from the repo root (where `docs.json` lives):

```
mint dev
```

The beta runs at `http://localhost:3000`.

## Publishing

Changes are deployed by Mintlify's GitHub app when they are pushed to the default branch
of the connected repository. Install/configure it from the
[Mintlify dashboard](https://dashboard.mintlify.com).

## Editing guidelines

- Match the calm, precise voice already in the pages; avoid hype words.
- Use the canonical terms: **hotspot**, **the Linkr network**, **contributor**.
- Keep headings in sentence case.
- Do not describe features that are not in the current build. If in doubt, check
  `docs/introduction/status.mdx` and mark roadmap items as roadmap.
