# Privacy Policy

**Myshcat's Services (Discord bot)** — last updated 2026-09-26

This bot provides a middleman escrow service, a build/farm-order service, and a support
ticket system for a DonutSMP Discord community. This page explains what data it collects,
why, and how to control or remove yours.

## What we collect

- **Discord identity:** your user ID, username, display name and avatar — used to show who's
  who in trades, orders, tickets and the staff dashboard.
- **Trade and order records:** the value of a trade, who was involved, what was ordered,
  prices, refunds and payout history. Kept indefinitely for accounting and dispute
  resolution, the same as any transaction record a business keeps.
- **Ticket message content:** only inside tickets the bot itself opens (middleman trades,
  build orders, support requests) and the staff vouch channel — never general server chat.
  Kept for 30 days, encrypted at rest, then automatically deleted. You can opt out of future
  capture, or have your existing messages scrubbed, at any time — see below.
- **Vouch records:** who vouched for whom, a star rating and an optional written reason, used
  for the public staff leaderboard.
- **Staff actions:** an audit log of moderation/staff actions taken through the bot or
  dashboard (who did what, when), for accountability.

## Who else sees it

- **The staff dashboard** — a private, self-hosted site. Only Discord accounts explicitly
  granted access (`/panelaccess add`) can sign in, via Discord's own OAuth login. We never
  see or store your Discord password.
- **The DonutSMP game API** — used only to verify in-game payment balances for the build
  service. No Discord data is sent to it, only a Minecraft account name.
- **A third-party vouch-tracking service** — used to keep vouch counts consistent with the
  server's existing helper bot. Receives your Discord user ID, the vouch giver's ID, and any
  reason text you write when giving a vouch.

We do not sell data, run ads, or use any of this to train AI/ML models.

## Your controls

- `/privacy optout` — stop future ticket messages from being captured (metadata like
  timestamps is kept for context, but content is withheld).
- `/privacy optin` — resume normal capture.
- `/privacy status` — check your current setting.
- `/privacy delete-my-data` — immediately scrub your message content from every ticket
  transcript already stored. This does not remove structured trade/order/payment records
  tied to your account, which are kept for financial record-keeping as described above.

## Security

Ticket message content is encrypted at rest (AES-256-GCM). The dashboard requires Discord
sign-in and an explicit access grant; nothing is publicly browsable.

## Contact

For questions or a data request beyond what the commands above cover, contact server staff
directly in Discord.
