# Merciv Product Docs

Customer-facing documentation for the Merciv platform — getting started, Chat, Knowledge, Trackers, Playbooks, Reports, Artifacts, account administration, and troubleshooting.

Built with [Mintlify](https://mintlify.com).

## Development

Install the Mintlify CLI:

```bash
npm i -g mint
```

Preview locally:

```bash
mint dev
```

Open `http://localhost:3000`.

Check links:

```bash
mint broken-links
```

## Source

Content is derived from the internal product research in the EVA monorepo (`docs/product/`), rewritten for customers. When product behavior changes, update the internal research first, then this site. `.archive/design-system/` contains the retired design-system docs; the brand styling (colors, logos, favicon) lives on in `docs.json` and `/logo`.

## Publishing

Install the Mintlify GitHub app from your [dashboard](https://dashboard.mintlify.com/settings/organization/github-app) to deploy changes automatically on push to the default branch.
