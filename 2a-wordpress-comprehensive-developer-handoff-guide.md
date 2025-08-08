# WordPress Developer Handoff Guide (Comprehensive)

A complete, practical guide for transferring a WordPress project from one team to another. It merges strategic, legal, operational, and technical handover material into one definitive reference, with checklists and templates you can use immediately.

Use this as a living document during the handover. Bring it to the handover meeting, check off items as you verify them, and keep the inventories up to date.

---

## How to use this guide

- Start with the Quickstart and Final Handover Checklist to frame the transfer.
- Work top-to-bottom. Each section ends with concrete actions and data to collect.
- Log every credential, license, and account in the Master Inventory table.
- Change passwords and enable 2FA as soon as access is confirmed.
- Remove the outgoing developer’s access everywhere before you sign off.

---

## Table of contents

1. [Quickstart & Success criteria](#quickstart--success-criteria)
2. [Strategic overview](#strategic-overview)
3. [Stakeholders & roles](#stakeholders--roles)
4. [Ownership & legal](#ownership--legal)
5. [Domain & DNS](#domain--dns)
6. [Hosting & server infrastructure](#hosting--server-infrastructure)
7. [Database access & structure](#database-access--structure)
8. [WordPress access & user management](#wordpress-access--user-management)
9. [Server access (FTP/SFTP/SSH)](#server-access-ftpsftpssh)
10. [Email configuration](#email-configuration)
11. [Themes, plugins, and custom code](#themes-plugins-and-custom-code)
12. [Third‑party services & integrations](#third-party-services--integrations)
13. [Backups & disaster recovery](#backups--disaster-recovery)
14. [Security posture](#security-posture)
15. [Performance & caching](#performance--caching)
16. [Analytics & SEO](#analytics--seo)
17. [Environments, version control & deployment](#environments-version-control--deployment)
18. [Documentation & training](#documentation--training)
19. [Maintenance & monitoring](#maintenance--monitoring)
20. [Final handover checklist](#final-handover-checklist)
21. [Exit interview questions](#exit-interview-questions)
22. [Appendix: Inventories & templates](#appendix-inventories--templates)

---

## Quickstart & Success criteria

Minimum bar for a successful handoff:

- Ownership: You have full administrative control of domain, DNS, hosting, WordPress, and all integrated services. Billing and renewal responsibility are in your accounts.
- Access: All credentials are in your password manager. Every admin login tested successfully.
- Security: Passwords rotated, 2FA enabled, previous access fully revoked, and keys regenerated where applicable.
- Backups: Verified working backups and a tested restore procedure.
- Operations: Clear, documented deployment process, update cadence, and monitoring in place.
- Knowledge: Architecture, customizations, and “quirks” are documented; training delivered.

---

## Strategic overview

Understand the purpose and history before changing anything.

- What problem does the site solve? Primary objectives (e.g., e‑commerce, lead gen, publishing).
- Who is the audience, and how has it evolved?
- Key milestones, major feature additions, pivots, or redesigns.
- KPIs for success (conversions, revenue, engagement) and how they’re measured.
- Any unique business rules, compliance constraints, or seasonal patterns.

Actions

- Capture the answers above in the project notes.
- Identify any misalignments between current architecture and business goals.

---

## Stakeholders & roles

- Decision makers and points of contact (product, content, marketing, tech).
- Approval workflow for content and technical changes; escalation path for incidents.
- Who managed discovery/planning; who will own the site post-handover.

Actions

- Record stakeholder list with roles and contact info.
- Agree on post-handover support window and communication channels.

---

## Ownership & legal

- Written confirmation of 100% ownership of website, content, custom code, and data upon final payment.
- List of premium themes/plugins and other licenses; transfer or repurchase details.
- Contracts and SLAs (hosting, maintenance, support); renewal dates and costs.
- Privacy compliance (GDPR/CCPA): data collection points, storage, retention, and policies.

Actions

- File copies of agreements; update billing to new owner.
- Populate license inventory with keys, renewal dates, and accounts.

---

## Domain & DNS

- Registrar, account owner, renewal date, and auto‑renew status.
- DNS provider (registrar, Cloudflare, etc.) and complete record set (A, AAAA, CNAME, MX, TXT, SPF, DKIM, DMARC, verification records).
- Subdomains, redirects, staging domains, and special rules.

Actions

- Gain registrar and DNS admin access; transfer account ownership where needed.
- Export current DNS zone file and attach to this document.

---

## Hosting & server infrastructure

- Hosting provider, plan name, cost, renewal date, and geographic region.
- Environment type (shared, VPS, dedicated, managed WordPress) and resource limits (CPU, RAM, storage, bandwidth, PHP memory/time limits).
- Server stack and versions (OS, Web server, PHP + extensions, MySQL/MariaDB), control panel (cPanel/Plesk/custom).
- Server‑level security (WAF/ModSecurity), firewall rules, and any allowlists.

Actions

- Verify access to hosting dashboard and server console (as applicable).
- Document any non‑standard server configs and required PHP extensions.

---

## Database access & structure

- DB host, port, engine/version, database name(s), users and privileges.
- Access method (phpMyAdmin, Adminer, CLI) and credentials.
- Custom tables or stored procedures beyond standard WordPress schema.
- Backup schedule, retention, and restore process.

Actions

- Perform a read‑only smoke check of DB access; export schema for reference.

---

## WordPress access & user management

- Provide NEW administrator account for the new owner/team. Do not re‑use existing logins.
- Inventory of all users and roles; identify accounts to remove or demote.
- Security features: 2FA, login restrictions, password policies.

Actions

- Create and test new admin(s). Rotate passwords for all service accounts.
- Remove previous developer/admin access after confirmation.

---

## Server access (FTP/SFTP/SSH)

- SFTP/SSH host, port, users/keys, and required security protocols.
- Document root path, logs, backup directories, symlinks, and special file permissions.
- Sudo privileges and any restrictions.

Actions

- Exchange SSH public keys via a secure channel; validate login and permissions.
- Store keys and connection profiles in your password manager.

---

## Email configuration

- Where domain email is hosted (e.g., Google Workspace/365/hosted).
- Account list, mailbox/alias/forward rules, and admin access.
- Transactional email path (WordPress mail, SMTP plugin, or service like SendGrid/Postmark) and credentials/API keys.

Actions

- Verify SPF, DKIM, DMARC; document SMTP settings and rate limits.

---

## Themes, plugins, and custom code

Theme

- Active theme, parent/child usage, and customization locations.
- For commercial themes: license/account info and documentation source.

Plugins

- Complete list (active/inactive) with version, purpose, premium/free status, and license details.
- Known conflicts or performance issues.

Custom development

- Custom plugins and their repositories; code locations for PHP, CSS, and JS.
- Custom post types, taxonomies, fields (e.g., ACF) and how they’re configured/exported.
- Coding standards followed; commenting level; lint/build tooling if any.

Actions

- Populate the Plugin & Theme Audit table in the Appendix.
- Ensure child theme is used for all theme customizations; no edits in parent theme.

---

## Third-party services & integrations

- Payments (Stripe/PayPal), CDN/WAF (Cloudflare), email marketing (Mailchimp/ConvertKit), CRM, analytics (GA/GTM), search, maps, forms, shipping/tax, etc.
- For each service: admin access, API keys/tokens, billing ownership, renewal dates, transfer steps.

Actions

- Regenerate API keys after ownership transfer. Update webhooks and callback URLs as needed.

---

## Backups & disaster recovery

- Backup solutions (host level, plugin, third‑party) and what’s included (files, DB, both).
- Frequency and retention policy; storage locations (on‑server, off‑site/cloud, multiple regions).
- Full restoration procedure and last successful restore test date.

Actions

- Perform a test restore on staging to validate backup integrity.

---

## Security posture

- Security plugins/tools (Wordfence, Sucuri, iThemes Security) and key configurations.
- SSL/TLS provider, renewal, and certificate monitoring.
- Role‑based access controls and Principle of Least Privilege.
- Security incident history and remediations.

Actions

- Rotate all secrets; enable 2FA for all admin‑level services.
- Review and harden file permissions; confirm WAF/CDN firewall rules.

---

## Performance & caching

- Caching layers: plugin (WP Rocket/W3TC), server (Redis/Memcached/Varnish), CDN caching, and browser caching settings.
- Cache purge procedures and automation hooks.
- Image optimization, asset minification/concatenation, DB optimization.

Actions

- Document clear “clear-all-caches” steps across every layer.

---

## Analytics & SEO

- Admin access to Google Analytics/GA4, Google Tag Manager, and Google Search Console.
- SEO plugin in use (Yoast/RankMath), sitemap location, meta templates, schema.
- Current rankings and any penalties/manual actions.

Actions

- Verify property ownerships and data streams. Capture baseline metrics before changes.

---

## Environments, version control & deployment

Environments

- Development and staging sites with access details and sync procedures.

Version control

- Git repository location and access, branching model, and protected branches.
- Confirm complete commit history and mapping to environments.

Deployment

- Exact process from commit to production, including DB change handling.
- Rollback steps; pre‑deploy checklist.

Actions

- Document an end‑to‑end deployment runbook; avoid making changes via FTP to production.

---

## Documentation & training

- Technical specs, architecture diagrams, admin guides, and brand/style guides.
- Video walkthroughs for common tasks and custom workflows.

Actions

- Store docs with the repo or knowledge base; schedule a live training/Q&A.

---

## Maintenance & monitoring

- Update cadence for core, themes, and plugins; change window policy.
- Uptime and performance monitoring; error logging and alert recipients.
- Support scope/duration and rates after the formal handover.

Actions

- Stand up monitoring and set alerting thresholds/recipients.

---

## Final handover checklist

Use this on handover day. Confirm each item before signing off.

- [ ] Schedule and conduct the formal handover meeting.
- [ ] Verify admin access to: Registrar, DNS, Hosting, WordPress, SFTP/SSH, Database, Email, CDN/WAF, Analytics, Payment gateways, Marketing tools, and any other third‑party services.
- [ ] Change all passwords and rotate all API keys/tokens.
- [ ] Enable 2FA on all services that support it.
- [ ] Remove/demote previous developer’s access from all systems.
- [ ] Validate backups and perform a test restore on staging.
- [ ] Smoke‑test critical user journeys (purchase/checkout, forms, login, search).
- [ ] Confirm monitoring/alerts are going to the correct recipients.
- [ ] Update the Master Inventory with final ownership status and renewal details.

---

## Exit interview questions

Ask open‑ended questions to uncover “unknown unknowns.”

- What are the most fragile or complex parts of the site? Any known pitfalls?
- If you had more time, what would you improve first and why?
- Any quirks, oddities, or manual workarounds we should know about?
- Biggest challenges during development; lessons learned.
- Any plugin conflicts, brittle integrations, or environment gotchas?

---

## Appendix: Inventories & templates

Use these tables as your single source of truth. Keep them current.

### Master Credentials & Services Inventory

| Service/Platform | Purpose            | Login URL                     | Username/Email | Password Method  | API Key/Token  | Cost | Renewal    | Owner     | Transfer Status |
| ---------------- | ------------------ | ----------------------------- | -------------- | ---------------- | -------------- | ---- | ---------- | --------- | --------------- |
| WordPress Admin  | Content Management | <https://domain.com/wp-admin> | new_admin_user | Password manager | —              | —    | —          | New Owner | ⏳ Pending       |
| Domain Registrar | Domain Control     |                               |                | Password manager | —              | $/yr | YYYY‑MM‑DD | New Owner | ⏳ Pending       |
| DNS Provider     | DNS/WAF            |                               |                | Password manager | Global API Key | $/mo | Monthly    | New Owner | ⏳ Pending       |
| Hosting          | Server             |                               |                | Password manager | —              | $/yr | YYYY‑MM‑DD | New Owner | ⏳ Pending       |
| Email Service    | Mailboxes          |                               |                | Password manager | —              | $/mo | Monthly    | New Owner | ⏳ Pending       |
| Backup Service   | Backups            |                               |                | Password manager | —              | $/mo | Monthly    | New Owner | ⏳ Pending       |
| Analytics        | Tracking           |                               |                | Password manager | —              | —    | —          | New Owner | ⏳ Pending       |
| Payment Gateway  | Payments           |                               |                | Password manager | Live keys      | Fees | —          | New Owner | ⏳ Pending       |

Notes

- Fill a row for every integration. Include billing email and invoice link where possible.
- After transfer, regenerate API keys/tokens and mark status as ✅ Completed.

### Plugin & Theme Audit

| Component       | Type         | Version | Purpose        | Premium? | License Status | Renewal    | Notes/Risks                  |
| --------------- | ------------ | ------- | -------------- | -------- | -------------- | ---------- | ---------------------------- |
| Active Theme    | Parent Theme | x.x.x   | Base framework | Premium  | Active         | YYYY‑MM‑DD | Do not edit directly         |
| Child Theme     | Child Theme  | x.x.x   | Customizations | Custom   | N/A            | N/A        | All customizations live here |
| WooCommerce     | Plugin       | x.x.x   | E‑commerce     | Free     | N/A            | N/A        | Critical; complex settings   |
| Security Plugin | Plugin       | x.x.x   | Hardening      | Premium  | Active         | YYYY‑MM‑DD | Firewall rules configured    |
| Caching Plugin  | Plugin       | x.x.x   | Performance    | Premium  | Active         | YYYY‑MM‑DD | Purge after deploy           |
| ACF PRO         | Plugin       | x.x.x   | Custom fields  | Premium  | Active/Missing | YYYY‑MM‑DD | If missing, high risk        |

### Server & Infrastructure Details

| Component     | Details                      | Access/Credentials | Notes |
| ------------- | ---------------------------- | ------------------ | ----- |
| Plan/Type     | Shared/VPS/Dedicated/Managed |                    |       |
| OS            | Linux/Windows + version      |                    |       |
| Web Server    | Apache/Nginx + version       |                    |       |
| PHP           | Version + extensions         |                    |       |
| Database      | MySQL/MariaDB + version      | Host/DB/User       |       |
| Control Panel | cPanel/Plesk/Custom          | URL/Access         |       |
| SSH/SFTP      | Host/Port/Keys               | Users/Permissions  |       |

### DNS Records Snapshot

| Name | Type        | Value | TTL | Notes |
| ---- | ----------- | ----- | --- | ----- |
| @    | A           |       |     |       |
| www  | CNAME       |       |     |       |
|      | MX          |       |     |       |
|      | TXT (SPF)   |       |     |       |
|      | TXT (DKIM)  |       |     |       |
|      | TXT (DMARC) |       |     |       |

### Deployment Runbook (Template)

1. Work from a feature branch; open PR to main/production.
2. Verify staging sync; run tests and manual QA.
3. Take fresh backups (files + DB). Confirm restore point.
4. Merge and deploy via pipeline/tooling. Avoid direct edits on prod.
5. Run DB migrations or configuration steps (if any).
6. Purge all caches (plugin, server, CDN) and verify.
7. Smoke‑test critical journeys. Roll back if needed.
8. Log changes in the Change Log (below).

### Change Log (Template)

| Date | Environment | Change | By  | Link/PR | Rollback |
| ---- | ----------- | ------ | --- | ------- | -------- |

### Handover Sign‑Off

- Date of handover: __________
- Parties present: __________
- Scope covered: __________
- Outstanding risks/issues: __________
- Post‑handover support: Duration _____, Scope _____, Rates _____

Signatures

- Outgoing developer: ____________________
- New owner/representative: ____________________

---

## Conclusion

A successful handover delivers complete control, deep system knowledge, and safe, repeatable operations. Use this guide, keep inventories current, and validate backups and access regularly. The handover is complete only after ownership is transferred, credentials are rotated, previous access is revoked, and critical paths are tested end‑to‑end.
