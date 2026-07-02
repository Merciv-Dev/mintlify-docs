# Documentation project instructions

## About this project

- This is the **Merciv product documentation** site — customer-facing docs for the Merciv platform, built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter (`title`, `description`, `icon`)
- Configuration and navigation live in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links
- `.archive/design-system/` holds the retired design-system docs (excluded from the site via `.mintignore`); `.archive/design-system/content/voice.mdx` remains the voice reference

## Audience & scope

- Readers are Merciv customers: brand managers, insights teams, analysts
- Source of truth for product behavior is the internal research in the EVA monorepo at `docs/product/` — do not invent UI, limits, or flows
- Never expose internal details: service names (datacore, chat-core, doc-process), infrastructure (queues, S3, databases), vendors (Auth0, PostHog, Stigg, SuprSend, LlamaParse), model names, feature-flag names, or staff-only tooling (Admin Panel, Reprocess)
- The product's internal codename is **EVA** — customer-facing name is always **Merciv**
- Plan-gated features get a `<Note>` ("available on select plans") rather than flag names

## Terminology

- Use **Merciv** (capital M) for the company and product name
- Core brand idea: **"Make sense of it all"**
- Product nouns (capitalize as the UI does): Chat, Knowledge, Trackers, Stories, Discover, Playbooks, Reports, Artifacts, Galleries, Projects, Portfolio
- "organization admin" (not "org admin") in customer-facing copy
- **Lucide** for icons — never emoji or unicode substitutes

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Run Now**
- Code formatting for file names, commands, and paths
- Match Merciv's content voice: conviction not salesmanship, specificity over abstraction
- Mintlify components (`<Steps>`, `<Note>`, `<Card>`, `<Accordion>`) only where they genuinely help; most content is prose and lists
- Internal links are root-relative (`/chat/overview`) and must point to pages listed in `docs.json`
