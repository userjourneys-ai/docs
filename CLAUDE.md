# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the technical documentation site for userjourneys.ai, built with Mintlify. The site provides integration guides for streaming session replays from PostHog and Sentry to the userjourneys.ai platform.

## Commands

```bash
# Install dependencies
npm install

# Start local development server
npx mint dev

# Build for production
npx mint build
```

## Architecture

- **Framework**: Mintlify (v4.2.108)
- **Content format**: MDX files (Markdown with JSX components)
- **Configuration**: `docs.json` defines navigation, theme, and site settings

### Directory Structure

- `/` - Main documentation pages (index.mdx, how-it-works.mdx)
- `/setup/` - Integration guides (posthog.mdx, sentry.mdx)
- `/images/` - Screenshots for setup guides
- `/logo/` - Light and dark theme logos

## Writing Guidelines

See `AGENTS.md` for comprehensive Mintlify technical writing standards. Key points:

- Every MDX page must start with YAML frontmatter containing `title` and `description`
- Use Mintlify components: `<Steps>`, `<Note>`, `<Tip>`, `<Warning>`, `<Check>`, `<Tabs>`, `<CodeGroup>`, `<AccordionGroup>`, `<Card>`, `<Frame>`
- Write in second person ("you"), use active voice and present tense
- Lead with most important information, use progressive disclosure
- Include verification steps to confirm success
