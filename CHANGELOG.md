# Mintlify Help Center Changelog

## 2026-03-31

### Navigation restructure (docs.json)

- **Added icons to all tabs:** Help Center (house), Features (sparkles), Slashy for Your Role (user-tie)
- **Added icons to all sidebar groups:** rocket, robot, message, gauge-high, shield-check, wrench, bolt, calendar, envelope, magnifying-glass, gear, etc.
- **Split "How-To Guides" into 3 focused groups:** "Automation Guides" (8 pages), "iMessage Agent" (3 pages), "Productivity & Workflow" (10 pages) -- reduces overwhelm from a single 21-page group
- **Moved What's New + Roadmap to global anchors:** Always visible from any page via sidebar anchors, no longer buried in a nav group
- **Added hidden group for changelog/roadmap pages:** Keeps pages accessible via global anchors without duplicating in sidebar nav
- **Added `seo.indexHiddenPages: false`** to prevent search engines from indexing hidden deep pages

### Hidden pages (reduce nav overwhelm)

6 pages marked `hidden: true` in frontmatter -- still accessible via search and direct links, but hidden from sidebar to keep navigation clean:

- `getting-started/subprocessors.mdx` -- compliance detail page, linked from Security & Trust
- `getting-started/why-primary.mdx` -- philosophical piece, linked from Slashy Method
- `getting-started/data-storage.mdx` -- GDPR/data detail page, linked from Security & Trust
- `troubleshooting/known-issues.mdx` -- changes frequently, better accessed via search
- `how-to-guides/gmail-together.mdx` -- niche use case for dual-client users
- `how-to-guides/track-opens.mdx` -- deep tracking article, covered in email-tracking parent

### New page: Automations Overview

- Created `features/automations/overview.mdx` as a landing page for the Automations section in the Features tab
- Explains how automations work (3-step process), links to all 4 automation types (email triggers, calendar triggers, auto-reminders, scheduled reminders), and includes a table of 7 popular automation examples
- Added to Features tab nav ahead of the individual automation pages

### Homepage improvements (index.mdx)

- **Fixed broken link:** "AI Drafts" card pointed to non-existent `/features/ai-drafts/how-drafts-work`, now correctly links to `/how-to-guides/ai-drafts`
- **Added "Top automations to set up" section:** Prominent horizontal card for 10-automations article plus 3 cards for receipt forwarding, meeting prep, and follow-up tracker
- **Added all 5 personas** (was 3): Added Recruiters and Executive Assistants cards
- **Added "Switching from another email client?" section:** Cards for Gmail, Superhuman, and Shortwave migration guides (was a single Gmail card)
- **Added Desktop App card** to Getting Started section (was missing)
- **Renamed "Explore features" to "What can Slashy do?"** for clarity
- **Split "Need help?" into FAQ + Troubleshooting cards** (was a single card)

### Accessibility: Image alt text

Fixed all 18 images across the docs that had empty `alt=""` attributes. Added descriptive alt text to:

- `how-to-guides/ai-drafts.mdx` (2 images)
- `personas/founders.mdx` (1 image)
- `personas/vcs.mdx` (1 image)
- `personas/sales.mdx` (1 image)
- `personas/executives.mdx` (2 images)
- `how-to-guides/keyboard-shortcuts.mdx` (1 image)
- `whats-new/changelog.mdx` (1 image)
- `switching/gmail-migration.mdx` (1 image)
- `how-to-guides/email-tracking.mdx` (2 images)
- `how-to-guides/never-miss-followup.mdx` (2 images)
- `how-to-guides/customize-agent.mdx` (2 images)
- `getting-started/calendar-setup.mdx` (3 images)

### Broken link fixes

- `personas/founders.mdx`: Fixed card link from `/features/automations` (404) to `/features/automations/overview`
- `index.mdx`: Fixed AI Drafts card from `/features/ai-drafts/how-drafts-work` (404) to `/how-to-guides/ai-drafts`
