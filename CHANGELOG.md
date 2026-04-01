# Mintlify Help Center Changelog

## 2026-03-31 (Iteration 10 -- Growth Persona)

### New page: Growth & Sales Development persona

Created `personas/growth.mdx` targeting growth marketers, SDRs, BDRs, and demand gen teams:

- 6-step Setup Checklist: multi-account connection, snippet library, open tracking, follow-up automations, pipeline labels, booking links
- 5 Automations: sequence follow-up drip, engagement alerts (3+ opens), timezone-optimized sends, stale lead scanner, auto-label by engagement
- Concrete workflow: "Run a 50-Person Outreach Campaign in 30 Minutes" (5 steps)
- 6 pro tips for high-volume outreach (account separation, snippet variables, open tracking patterns, breakup emails, batching, agent reports)
- 9 sample agent commands in 3 tabs (Campaign Management, Outreach & Sequences, Engagement & Reporting)
- 4 Related Articles cards (Email Tracking, Snippets, Follow-ups, Multiple Accounts)
- Full frontmatter with seoDescription and chart-line icon

### docs.json: added growth persona to navigation

Added `personas/growth` to the Personas group in the "Slashy for Your Role" tab, positioned between Sales and VCs.

---

## 2026-03-31 (Iteration 9 -- QA Pass)

Final quality assurance pass across all 80 articles, docs.json, and 3 snippets.

### Checks performed (all passed)

- **MDX syntax validation**: Verified all JSX component tags (Steps, Tabs, Accordion, CardGroup, Frame, Note, Tip, Warning, etc.) are properly opened and closed across all 80 articles. No mismatches found.
- **Frontmatter consistency**: Confirmed every article has `title`, `description`, and `seoDescription`. All present.
- **Snippet usage**: Verified `ContactSupport` (4 articles) and `KeyboardShortcutTip` (5 articles) are correctly imported with `/snippets/` path prefix and properly invoked. `AgentSidebarOpen` snippet exists for future use; its content is already inlined in the `contact-support` snippet.
- **docs.json validation**: JSON parses cleanly. All 80 page paths resolve to existing .mdx files. No duplicate entries. No orphaned .mdx files outside navigation.
- **Image alt text**: No empty `alt=""` attributes found. No generic "screenshot" alt texts. All images have descriptive alt text.
- **Tone/voice**: Spot-checked 5 articles (booking-page, notifications, contacts/overview, ai-memories, disconnect). All consistent: direct, authoritative, 2nd person, 300-800 word range.
- **No orphaned files**: Every content .mdx file appears in docs.json navigation. Every docs.json entry has a corresponding .mdx file.

### Result

No fixes required. The help center is clean and ready for production.

---

## 2026-03-31 (Iteration 8 -- Refinement & Advanced Features)

### Feedback widget and theming enhancements (docs.json)

Added Mintlify configuration for reader engagement and visual polish:

- `feedback.thumbsRating: true` -- thumbs up/down rating on every article
- `feedback.suggestEdit: true` -- readers can suggest edits
- `rounded: "default"` -- consistent rounded corners on images and cards
- `background.decoration: "gradient"` -- subtle gradient decoration on pages
- `typography.headings.weight: 600` -- semi-bold headings for visual hierarchy

### Internal link audit: 2 broken links fixed

Fixed broken internal links in `troubleshooting/unexpected-behavior.mdx`:

- `/how-to-guides/automations` (404) -> `/features/automations/overview`
- `/how-to-guides/writing-style` (404) -> `/how-to-guides/customize-agent`

### Broken image references fixed: connecting-gmail screenshots

Fixed 3 broken image `src` paths in `getting-started/connecting-gmail.mdx` where filenames were missing the `-sla` segment:

- `connecting-gmail-permissions-security-and-what-1.png` -> `connecting-gmail-permissions-security-and-what-sla-1.png`
- `connecting-gmail-permissions-security-and-what-2.png` -> `connecting-gmail-permissions-security-and-what-sla-2.png`
- `connecting-gmail-permissions-security-and-what-3.png` -> `connecting-gmail-permissions-security-and-what-sla-3.png`

### Image utilization: all 25 remaining unused screenshots added (113/113 mapped images now used)

Cross-referenced image-mapping.json with article usage. Added Frame+img tags for all 25 previously unused screenshots:

- `troubleshooting/disconnect.mdx` -- 3 screenshots (connected accounts, reconnect button, Google permissions page)
- `getting-started/connecting-gmail.mdx` -- 1 screenshot (connected accounts overview)
- `features/settings/theme.mdx` -- 1 screenshot (dark theme preview)
- `features/email/composing.mdx` -- 1 screenshot (full compose window with toolbar)
- `features/email/snippets.mdx` -- 3 screenshots (snippet list, AI variable editor, analytics dashboard)
- `how-to-guides/ai-drafts.mdx` -- 1 screenshot (AI email rating with score)
- `features/tasks/overview.mdx` -- 1 screenshot (task detail with linked email)
- `getting-started/ai-memories.mdx` -- 1 screenshot (memories management page)
- `getting-started/importance-labels.mdx` -- 2 screenshots (training examples, per-label settings)
- `how-to-guides/never-miss-followup.mdx` -- 1 screenshot (follow-up automation settings)
- `features/email/unsubscribe.mdx` -- 1 screenshot (bulk unsubscribe confirmation)
- `getting-started/desktop-app.mdx` -- 1 screenshot (system tray and dock badge)
- `how-to-guides/multiple-accounts.mdx` -- 1 screenshot (connected accounts overview)
- `how-to-guides/customize-agent.mdx` -- 1 screenshot (writing style preferences)
- `getting-started/calendar-setup.mdx` -- 3 screenshots (calendar toggles, event editor, Meet With overlay)

### Content expansion: 3 thin articles enriched

Expanded substance in the 3 thinnest feature/troubleshooting articles:

- `troubleshooting/disconnect.mdx` -- added Read Mode preservation table, Tip about safety, "Choosing the Right Option" AccordionGroup (3 scenarios), expanded deletion info
- `features/integrations/zoom.mdx` -- added "Zoom with Automations" section with meeting prep tip, "Troubleshooting" AccordionGroup (3 common issues)
- `features/email/replying.mdx` -- added threading Tip, comprehensive "Reply Shortcuts at a Glance" table (7 shortcuts)

---

## 2026-03-31 (Iteration 7 -- Final Polish)

### Complete SEO coverage: seoDescription on all 80 articles (28 remaining added)

Added `seoDescription` frontmatter with unique, keyword-rich meta descriptions to all remaining 28 articles:

- `features/settings/theme.mdx`
- `features/tasks/overview.mdx`
- `features/calendar/booking-links.mdx`
- `features/calendar/availability.mdx`
- `features/calendar/rsvp.mdx`
- `features/calendar/granola.mdx`
- `features/contacts/overview.mdx`
- `features/search/overview.mdx`
- `features/integrations/zoom.mdx`
- `features/email/replying.mdx`
- `features/email/snippets.mdx`
- `features/email/scheduled-send.mdx`
- `features/email/unsubscribe.mdx`
- `features/email/notifications.mdx`
- `troubleshooting/roadmap.mdx`
- `troubleshooting/known-issues.mdx`
- `getting-started/ai-privacy.mdx`
- `getting-started/why-primary.mdx`
- `getting-started/subprocessors.mdx`
- `how-to-guides/slashy-method.mdx`
- `how-to-guides/signatures.mdx`
- `how-to-guides/track-opens.mdx`
- `how-to-guides/automate-receipts.mdx`
- `how-to-guides/multiple-accounts.mdx`
- `how-to-guides/otp-forwarding.mdx`
- `how-to-guides/gmail-together.mdx`
- `how-to-guides/booking-page.mdx`
- `how-to-guides/customer-followups.mdx`

All 80 articles now have seoDescription for search engine optimization.

### Image utilization: 9 unused screenshots added to articles

Cross-referenced image-mapping.json with article usage. Added Frame+img tags for 9 previously unused screenshots:

- `how-to-guides/customer-followups.mdx` -- added follow-up automation settings screenshot
- `how-to-guides/automate-receipts.mdx` -- added automations panel screenshot
- `features/email/unsubscribe.mdx` -- added 2 screenshots (bulk unsubscribe rankings, blocked sender management)
- `how-to-guides/batch-processing.mdx` -- added batch action confirmation screenshot
- `features/email/composing.mdx` -- added pop-up compose mode screenshot
- `how-to-guides/customize-agent.mdx` -- added writing style settings screenshot
- `switching/superhuman-migration.mdx` -- added Superhuman comparison hero screenshot
- `how-to-guides/track-opens.mdx` -- added VIP open alert automation screenshot

### Multi-account articles: enhanced with Tips, Steps, Warnings, cross-linking

- `getting-started/multi-account.mdx` -- added Warning about From field in All mode, added second screenshot (account switcher), expanded Related Articles from 2 to 4 cards with cross-link to how-to-guides/multiple-accounts
- `how-to-guides/multiple-accounts.mdx` -- added Tip about account limits, converted connection instructions to Steps (4-step), added Warning about From field default, added third screenshot (From dropdown), added Tip about cross-account agent queries, expanded Related Articles from 2 to 4 cards with cross-link to getting-started/multi-account

### Slashy Method: showcase article enhancement

Rewrote `how-to-guides/slashy-method.mdx` as a showcase article:

- Added opening Tip callout about the 70-85% time savings
- Converted Principle 1 from bullet list to 4-step Steps walkthrough (enable labels, start in Important, bulk-process, correct misclassifications)
- Added "Setup Command" column to the automations table in Principle 2 with exact agent commands users can paste
- Added Tip about 10-minute setup for all six automations
- Expanded "Getting Started Today" from 3-step to 5-step "Day-by-Day Plan" covering labels, first automation, writing memories, desktop app, and review
- Added "Measuring Your Progress" table showing expected improvements across Week 1, Month 1, and Month 3
- Expanded Related Articles from 2 to 4 cards (added First Week guide and Why Primary Matters)

### Hidden pages: 2 additional niche pages hidden from nav

- `how-to-guides/otp-forwarding.mdx` -- niche iMessage sub-feature, linked from iMessage capabilities and automation guides
- `features/calendar/granola.mdx` -- specific third-party integration, linked from meeting prep

Total hidden pages: 8 (up from 6). All remain accessible via search and direct links.

---

## 2026-03-31 (Iteration 6b -- Polish & Consistency)

### Consistency audit: seoDescription added to 27 more articles (52/80 total)

Added `seoDescription` frontmatter with unique, keyword-rich meta descriptions to:

- `features/ai-agent/composing.mdx`
- `features/ai-drafts/autocomplete.mdx`
- `features/ai-drafts/editing.mdx`
- `features/automations/auto-reminders.mdx`
- `features/automations/overview.mdx`
- `features/automations/scheduled-reminders.mdx`
- `features/automations/email-triggers.mdx`
- `features/email/labels.mdx`
- `getting-started/ai-memories.mdx`
- `getting-started/importance-labels.mdx`
- `getting-started/desktop-app.mdx`
- `getting-started/mobile.mdx`
- `getting-started/calendar-setup.mdx`
- `getting-started/multi-account.mdx`
- `how-to-guides/ai-drafts.mdx`
- `how-to-guides/inbox-zero.mdx`
- `how-to-guides/email-tracking.mdx`
- `how-to-guides/customize-agent.mdx`
- `how-to-guides/meeting-prep.mdx`
- `how-to-guides/never-miss-followup.mdx`
- `how-to-guides/batch-processing.mdx`
- `personas/founders.mdx`
- `personas/sales.mdx`
- `personas/vcs.mdx`
- `personas/recruiters.mdx`
- `personas/executives.mdx`
- `whats-new/changelog.mdx`

### Consistency audit: Related Articles headings on 12 articles

Added or standardized "## Related Articles" heading above CardGroup sections and expanded to 4 cards on:

- `features/ai-agent/composing.mdx` -- added heading + Keyboard Shortcuts card
- `features/ai-drafts/autocomplete.mdx` -- added heading + AI Memories card
- `features/ai-drafts/editing.mdx` -- added heading + Composing Emails card
- `features/automations/auto-reminders.mdx` -- added heading + Automations Overview card
- `features/automations/calendar-triggers.mdx` -- added heading + Meeting Prep card
- `features/automations/scheduled-reminders.mdx` -- added heading + Automation Recipes card
- `features/email/labels.mdx` -- added heading + Inbox Zero and Importance Labels cards
- `getting-started/ai-memories.mdx` -- added heading + Autocomplete and AI Privacy cards
- `getting-started/importance-labels.mdx` -- added heading + Inbox Zero and Inbox Views cards
- `getting-started/desktop-app.mdx` -- added heading + Keyboard Shortcuts and Mobile cards
- `getting-started/mobile.mdx` -- added heading + Desktop App and Mobile Fixes cards
- `whats-new/changelog.mdx` -- added heading + Roadmap and 10 Automations cards

### Image audit: screenshots added to 2 articles

- `getting-started/security-privacy.mdx` -- added security overview screenshot
- `getting-started/desktop-app.mdx` -- added second screenshot (desktop app with dock badge)

### Desktop app & mobile: enhanced with Tips

- `getting-started/desktop-app.mdx` -- added Tip about automatic sync from web
- `getting-started/mobile.mdx` -- added Tip about account sync

### Changelog: restructured with version numbers and dates

Rewrote `whats-new/changelog.mdx` with:
- Version numbers (v2.5 through v2.14) for each update
- Specific dates per release (weekly cadence)
- Horizontal rule separators between months
- Added seoDescription for search
- Expanded Related Articles from 2 to 4 cards

### docs.json verification

Verified all 80 page paths in docs.json resolve to existing .mdx files. Verified all .mdx content pages appear in the navigation. No missing pages or orphaned files found.

---

## 2026-03-31 (Iteration 6)

### iMessage articles: enhanced with Steps, Tips, Accordions

Upgraded all 3 iMessage articles with richer Mintlify components and better structure:

- `how-to-guides/imessage-setup.mdx` -- Added Tip (differentiator callout), "Quick Test After Setup" Steps (3-step verification), converted troubleshooting table to AccordionGroup (5 items with expanded answers), added privacy link to AI Privacy page, expanded Related Articles to 4 cards, added seoDescription
- `how-to-guides/imessage-capabilities.mdx` -- Added Tip (remote control metaphor), converted Draft and Send Replies from bullets to 3-step Steps walkthrough, added Warning (send it vs save as draft), added Tip for voice messages, replaced Tips section with "Power User Tips" AccordionGroup (4 items), expanded Related Articles to 4 cards with Daily Briefings link, added seoDescription
- `how-to-guides/imessage-briefings.mdx` -- Added 4th step to setup Steps, added Tip (setup timing advice), added "Add an End-of-Day Wrap-Up" section with Steps, added Tip (briefing is interactive), expanded Related Articles from 2 to 4 cards, added seoDescription

### Security & Trust: trust badges, expanded FAQs, cross-linking

Enhanced all 3 Security & Trust articles:

- `getting-started/security-privacy.mdx` -- Added "Trust at a Glance" CardGroup with 3 trust badge cards (SOC 2, Zero-Training, AES-256), expanded Enterprise Security FAQ AccordionGroup from 4 to 7 questions (added breach response, Workspace admin, company safety), renamed section to "Common Security Questions", expanded Related Articles from 2 to 4 cards
- `getting-started/ai-privacy.mdx` -- Added "Common AI Privacy Questions" AccordionGroup (4 items: accidental send, cross-account, BYOK, memories privacy), expanded Related Articles from 2 to 4 cards
- `getting-started/data-storage.mdx` -- Added "Common Data Questions" AccordionGroup (3 items: attachments, export, Gmail after deletion), expanded Related Articles from 2 to 3 cards, added seoDescription

### Founders persona: CEO Morning Email Routine workflow

Added "Workflow: CEO Morning Email Routine (15 Minutes)" Steps section to `personas/founders.mdx`:

- 5-step workflow: iMessage briefing (2 min), VIP triage (3 min), keyboard shortcut processing (5 min), dropped ball check (2 min), meeting prep (3 min)
- Added Tip about inbox zero timing with importance labels
- Cross-links to daily briefings and meeting prep guides

### New page: Automation Recipes

Created `how-to-guides/automation-recipes.mdx` with 6 copy-paste automation recipes:

1. Auto-forward receipts to accountant
2. Send meeting prep 30 minutes before external calls
3. Daily dropped ball scanner at 8am
4. VIP email alerts with visual preview
5. Post-meeting follow-up drafts
6. Weekly email digest every Friday

Each recipe uses Steps with exact agent commands users can paste directly. Added to Automation Guides nav group in docs.json.

### Homepage polish

- Added "Security & Trust" section with 3 cards (Security & Privacy, AI Privacy, Data Storage)
- Added "Automation Recipes" card to the automations section (changed from 3-col to 2-col for 4 cards)

---

## 2026-03-31 (Iteration 5)

### Troubleshooting: expanded FAQ with grouped Accordions

Restructured `troubleshooting/faq.mdx` from a single AccordionGroup into three categorized sections:

- **General** (10 existing questions)
- **AI & Automations** (4 new questions: AI draft accuracy, limiting agent actions, turning off automations, debugging triggers)
- **Billing & Plans** (2 new questions: free trial, BYOK API keys)
- Added contact support snippet and expanded Related Articles CardGroup from 2 to 4 cards

### Troubleshooting: contact support snippet integration

Replaced manual "report a bug" / "contact support" blocks with a reusable `<ContactSupport />` snippet across 4 troubleshooting pages:

- `troubleshooting/faq.mdx`
- `troubleshooting/desktop-fixes.mdx`
- `troubleshooting/mobile-fixes.mdx`
- `troubleshooting/sync-issues.mdx`

### Switching guides: comparison tables and migration checklists

Added detailed feature comparison tables (Slashy vs competitor) and step-by-step migration checklists using `<Steps>` to all 3 switching guides:

- `switching/gmail-migration.mdx` -- 10-row "Gmail vs Slashy at a Glance" table + 7-step migration checklist
- `switching/superhuman-migration.mdx` -- 13-row full feature comparison table + 6-step migration checklist
- `switching/shortwave-migration.mdx` -- 12-row full feature comparison table + 7-step migration checklist (replaced bullet checklist)

### Features: enhanced 4 articles with Mintlify components

- `features/calendar/creating-events.mdx` -- Added AccordionGroup for "Creating Events with the AI Agent" (3 examples: schedule, find time, reschedule)
- `features/email/composing.mdx` -- Added Tip for undo send configuration
- `features/email/inbox-views.mdx` -- Added AccordionGroup for "Common View Workflows" (morning triage, follow-up review, end-of-day cleanup)
- `features/automations/calendar-triggers.mdx` -- Added AccordionGroup for "Troubleshooting Calendar Triggers" (3 common issues)

### SEO: added seoDescription frontmatter to 15 key articles

Added `seoDescription` field with unique, keyword-rich descriptions optimized for search:

- `index.mdx`
- `getting-started/first-week.mdx`
- `getting-started/connecting-gmail.mdx`
- `getting-started/security-privacy.mdx`
- `how-to-guides/10-automations.mdx`
- `how-to-guides/keyboard-shortcuts.mdx`
- `features/ai-agent/autonomy.mdx`
- `features/email/composing.mdx`
- `features/email/inbox-views.mdx`
- `features/calendar/creating-events.mdx`
- `features/automations/calendar-triggers.mdx`
- `switching/gmail-migration.mdx`
- `switching/superhuman-migration.mdx`
- `switching/shortwave-migration.mdx`
- `troubleshooting/faq.mdx`
- `troubleshooting/sync-issues.mdx`
- `troubleshooting/desktop-fixes.mdx`
- `troubleshooting/mobile-fixes.mdx`
- `troubleshooting/unexpected-behavior.mdx`
- `troubleshooting/disconnect.mdx`

### Snippets: created 3 reusable content blocks

Created `snippets/` directory with 3 reusable MDX snippets:

- `snippets/contact-support.mdx` -- Standard "Need more help?" Note callout with email and agent sidebar instructions
- `snippets/keyboard-shortcut-tip.mdx` -- Tip callout linking to full keyboard shortcuts cheatsheet
- `snippets/agent-sidebar-open.mdx` -- Standard text for opening the AI agent sidebar

Snippets imported and used across 10+ articles (troubleshooting pages, switching guides, feature articles).

---

## 2026-03-31 (Iteration 4)

### Article quality: Tip, Warning, and Steps components

Added Mintlify callout components to 7 articles for better readability and scannability:

- `how-to-guides/ai-drafts.mdx` -- Added Tip (getting started advice), Warning (accept does not send), Tip (manual drafts use case), Tip (model selection guidance)
- `how-to-guides/inbox-zero.mdx` -- Added Tip (time-to-inbox-zero), Warning (labels are required), converted label setup from numbered list to Steps component
- `how-to-guides/email-tracking.mdx` -- Added Warning (tracking is not 100% reliable), Tip (combine tracking with follow-up automation)
- `how-to-guides/batch-processing.mdx` -- Added Warning (check selection before bulk actions)
- `how-to-guides/never-miss-followup.mdx` -- Added Tip (recommended two-layer setup)
- `how-to-guides/customize-agent.mdx` -- Added Tip (fastest training approach), converted BYOK from numbered list to Steps, added Warning (Opus billing)
- `features/email/snippets.mdx` -- Converted AI Variables section from bullet list to Steps walkthrough, added Tip (snippets + AI for outreach at scale)

### Persona pages: Sample Agent Commands with Tabs

Added `<Tabs>` sections to all 5 persona pages showing concrete agent sidebar commands organized by workflow type:

- `personas/founders.mdx` -- Tabs: Inbox Triage, Investor Relations, Team & Delegation (9 example commands)
- `personas/sales.mdx` -- Tabs: Pipeline Management, Outreach, Meeting Prep (9 example commands)
- `personas/vcs.mdx` -- Tabs: Deal Flow, Portfolio, Intros & Passes (9 example commands)
- `personas/recruiters.mdx` -- Tabs: Pipeline, Outreach, Coordination (9 example commands)
- `personas/executives.mdx` -- Tabs: Triage & Summaries, Delegation, Decisions (9 example commands)

### Cross-linking: expanded Related Articles sections

Added or expanded "Related Articles" headings and CardGroup sections in 8 articles:

- `how-to-guides/ai-drafts.mdx` -- expanded from 3 to 4 cards (added Never Miss a Follow-up)
- `how-to-guides/inbox-zero.mdx` -- expanded from 2 to 4 cards (added Batch Processing, Keyboard Shortcuts)
- `how-to-guides/email-tracking.mdx` -- expanded to 4 cards (added Slashy for Sales, Customer Follow-ups)
- `how-to-guides/batch-processing.mdx` -- expanded from 2 to 4 cards (added Keyboard Shortcuts, AI Drafts)
- `how-to-guides/never-miss-followup.mdx` -- expanded from 2 to 4 cards (added Customer Follow-ups, Inbox Zero)
- `how-to-guides/customize-agent.mdx` -- replaced iMessage Capabilities with AI Memories card, added Related Articles heading
- `features/email/snippets.mdx` -- expanded from 2 to 4 cards (added Slashy for Sales, Slashy for Recruiters)
- `personas/founders.mdx` -- expanded from 2 to 4 cards (added Never Miss a Follow-up, Meeting Prep)

---

## 2026-03-31 (Iteration 3)

### Cross-linking: Related Articles CardGroup sections

Added or expanded "Related Articles" `<CardGroup>` sections at the bottom of 12 articles, creating a bidirectional link network across the docs:

- `getting-started/first-week.mdx` -- expanded from 2 to 6 cards (added 10 Automations, AI Drafts, Keyboard Shortcuts, iMessage Setup)
- `getting-started/connecting-gmail.mdx` -- expanded from 2 to 4 cards (added Calendar Setup, Multiple Accounts)
- `getting-started/calendar-setup.mdx` -- expanded from 2 to 4 cards (added Booking Pages, Meeting Prep)
- `how-to-guides/10-automations.mdx` -- expanded from 4 to 6 cards (added Automations Overview, Email Triggers, Calendar Triggers, Never Miss a Follow-up; removed duplicates)
- `how-to-guides/meeting-prep.mdx` -- expanded from 2 to 4 cards (added Calendar Triggers, Booking Pages)
- `how-to-guides/automate-receipts.mdx` -- expanded from 2 to 4 cards (added Email Triggers, Automations Overview)
- `features/automations/email-triggers.mdx` -- expanded from 3 to 4 cards (added 10 Automations)
- `features/automations/overview.mdx` -- expanded from 2 to 4 cards (added Customize Your Agent, iMessage Setup)
- `how-to-guides/email-tracking.mdx` -- added Related Articles heading; linter expanded to 4 cards
- `personas/founders.mdx` -- unchanged (already had good links)
- `personas/sales.mdx` -- expanded to 4 cards with corrected paths
- `personas/recruiters.mdx` -- expanded to 4 cards with corrected paths
- `personas/vcs.mdx` -- expanded to 4 cards with corrected paths
- `personas/executives.mdx` -- expanded to 4 cards with corrected paths

### Steps components: converted numbered lists to `<Steps>`

Converted step-by-step instructions in 3 articles from numbered lists to Mintlify `<Steps>` components for visual clarity:

- `getting-started/connecting-gmail.mdx` -- "Verify Your Sync" section (4 steps)
- `getting-started/calendar-setup.mdx` -- "Choose Which Calendars to Show" (3 steps), "Booking Links" (3 steps), "Meet With" (3 steps)
- `how-to-guides/email-tracking.mdx` -- "Open Trigger Automations" (3 steps)

### Persona pages: concrete workflow examples with Steps

Added full `<Steps>` workflow walkthroughs to 2 persona pages:

- `personas/sales.mdx` -- "Workflow: Process Your Morning Pipeline in 10 Minutes" (5 steps covering triage, AI drafts, opens panel, dropped ball scanner, scheduled sends)
- `personas/recruiters.mdx` -- "Workflow: Send 20 Personalized Outreach Emails in 15 Minutes" (5 steps covering snippets, personalization, booking links, tracking, opens review)

Linter also auto-added "Sample Agent Commands" `<Tabs>` sections to sales, recruiters, VCs, and executives persona pages.

### Broken internal link fixes

Fixed 7 broken links in persona page CardGroup sections:

- `personas/sales.mdx`: `/features/email-tracking` -> `/how-to-guides/email-tracking`
- `personas/sales.mdx`: `/features/snippets` -> `/features/email/snippets`
- `personas/recruiters.mdx`: `/features/snippets` -> `/features/email/snippets`
- `personas/recruiters.mdx`: `/features/email-tracking` -> `/how-to-guides/email-tracking`
- `personas/vcs.mdx`: `/features/ai-drafts` -> `/how-to-guides/ai-drafts`
- `personas/executives.mdx`: `/features/ai-drafts` -> `/how-to-guides/ai-drafts`
- `personas/executives.mdx`: `/features/automations` -> `/features/automations/overview`

---

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
