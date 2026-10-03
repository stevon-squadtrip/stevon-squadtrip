# Hi, I'm Stevon 👋

I put AI into production and keep it honest.

Most of my work is the part people skip: the agent tooling, and then the verification and guardrails that decide what it's allowed to do on its own. I build with Claude Code and MCP daily, and I ship small, complete products end to end with Next.js, TypeScript, and Postgres.

🌐 [stevonjudd.com](https://stevonjudd.com)

## What I've built at work

Co-founder and former CTO of [SquadTrip](https://squadtrip.com), a group travel and payments platform running roughly $12M a year in booking volume on Stripe Connect. The codebase is closed, but the work looked like this:

**Agent tooling.** An agent workflow layer on Claude Code: 16 orchestration commands and 10 MCP integrations across the support platform, production SQL, Stripe, Jira, Honeybadger, PostHog, and Azure. One command dispatches nine agents in parallel against a single support ticket and returns a diagnosis with its evidence attached.

**The guardrails around it.** Evidence required before an agent asserts anything. Human approval on every customer-facing send and every production write. Pre-tool hooks that block secret-file creation and gate edits to payment code. An audit log of every run. That verification layer caught the agent contradicting its own earlier conclusion before it reached a customer.

**Knowledge grounding.** Verified 176 help articles against source code, production data, and the payment processor directly. Staged 340+ corrections behind human sign-off. Found 10 answers already reaching customers that were materially wrong. Froze a 68.1% resolution baseline across 552 conversations first, so impact would be a number rather than a feeling.

**Test and release infrastructure.** Built the automated test layer from nothing: 1,087 Playwright and unit tests where no end-to-end coverage existed. Cut regression runtime from 110 minutes to 24 through partitioned parallelization. CI/CD with environment swapping, deploy-verification health endpoints, a system health API, Honeybadger and PostHog instrumentation, and a Slack ops center running health checks and daily digests.

**Payments integrity.** Daily reconciliation across 2,000+ connected Stripe accounts catching charges the processor had and the database didn't. Structured decline capture that made $45K of previously invisible installment failures queryable.

Before that: Senior Technical Program Manager at MongoDB, where I led the relaunch and sunset of Ops Manager across 8 organizations, migrating 200 enterprise customers with zero disruption.

## Things I've built on my own

| Project | What it is | Stack |
| --- | --- | --- |
| [Rplyflow](https://rplyflow.ai) | AI reply assistant for Instagram. Learns your voice from past replies and drafts comment and DM responses you approve before sending | AI SaaS |
| **Ezra Tracker** | Family health tracker used daily. Feed and med schedules, appointments, AI document processing, Google Calendar sync, Telegram bot *(code private)* | Next.js, Prisma, Postgres, Claude API |
| [1,000 Whys](https://1000-whys.vercel.app) | Interactive science discovery app for curious kids. 1,000 "why" questions across animals, space, weather, the human body, and everyday science. [code](https://github.com/stevon-squadtrip/1000-whys) | Next.js 14 |
| [28 Days of Amazing People](https://black-history-book.vercel.app) | Interactive Black History Month storybook for kids ages 4+. [code](https://github.com/stevon-squadtrip/black-history-book) | Next.js 14 |
| [Squad Pool](https://github.com/stevon-squadtrip/squad-pool) | World Cup 2026 bracket pool. Shareable picks, zero auth | Next.js 14, Postgres |
| [Spades Tracker](https://spades-tracker.vercel.app) | Self-contained spades scorekeeper in a single static HTML file. [code](https://github.com/stevon-squadtrip/spades-tracker) | Vanilla JS |
| [Phila Sheriff Sales](https://github.com/stevon-squadtrip/phila-sheriff-sales) | Philadelphia sheriff-sale auction tracker. Scrapes final bids, generates an HTML report | Python |

Every one of these is deployed and in real use. None of them were assigned to me.

## How I work

- Find where a team is losing time, then build the thing that removes it
- Ship small and complete rather than large and theoretical
- Freeze the baseline before changing anything, so improvement is measurable
- Constrain what runs unsupervised. The mistakes that matter are the irreversible ones

**Working with:** Claude Code, MCP, agent orchestration, RAG and knowledge grounding, LLM evaluation, n8n, Zapier, Stripe Connect, Azure, Playwright, C#/.NET, React, SQL, Python

📫 Reach me through [stevonjudd.com](https://stevonjudd.com)
