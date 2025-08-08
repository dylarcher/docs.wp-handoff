# WordPress Project Handover: Comprehensive Due Diligence Checklist

A successful WordPress handover is not just about sharing files and passwords—it's a process of transferring knowledge, responsibility, and control. This checklist combines strategic, technical, operational, and legal considerations to ensure a seamless transition and minimize risks for the new owner.

---

## Table of Contents

1. [Project Overview & Intent](#1-project-overview--intent)
2. [Stakeholders & Roles](#2-stakeholders--roles)
3. [Ownership & Legal](#3-ownership--legal)
4. [Domain & Hosting](#4-domain--hosting)
5. [Server & Infrastructure](#5-server--infrastructure)
6. [Database](#6-database)
7. [WordPress Access](#7-wordpress-access)
8. [FTP/SFTP/SSH Access](#8-ftpsftpssh-access)
9. [Email](#9-email)
10. [Plugins, Themes & Custom Code](#10-plugins-themes--custom-code)
11. [Integrations & Third-Party Services](#11-integrations--third-party-services)
12. [Backups & Recovery](#12-backups--recovery)
13. [Security](#13-security)
14. [Performance & Caching](#14-performance--caching)
15. [Analytics & SEO](#15-analytics--seo)
16. [Environments & Deployment](#16-environments--deployment)
17. [Documentation & Training](#17-documentation--training)
18. [Support, Maintenance & Monitoring](#18-support-maintenance--monitoring)
19. [Final Handover & Exit Interview](#19-final-handover--exit-interview)
20. [Appendix: Inventory Tabular Data](#20-appendix-inventory-tabular-data)

---

## 1. Project Overview & Intent

- **What is the primary purpose of the website?**
  _Clarifies business goals and informs future decisions (e.g., e-commerce, lead generation, content hub)._

- **Are there unique business rules or workflows?**
  _Identifies custom logic or processes that may impact maintenance._

- **How has the website evolved over time?**
  _Highlights major pivots, technical debt, or legacy features._

- **What are the key performance indicators (KPIs) for success?**
  _Ensures future changes align with what matters most (sales, signups, traffic, etc.)._

---

## 2. Stakeholders & Roles

- **Who are the main points of contact (client, stakeholders, etc.)?**
  _Ensures clear communication lines and approval workflows._

- **Who manages the website now, and who will after handover?**
  _Defines responsibilities for content, technical, and business decisions._

- **Who participated in the original planning/discovery phase?**
  _Provides context for historical decisions and future reference._

---

## 3. Ownership & Legal

- **Do we fully own the website, code, and content after payment?**
  _Prevents disputes over intellectual property and future access._

- **Are there ongoing contracts (hosting, support, SLAs, etc.)?**
  _Identifies recurring obligations and costs._

- **Are there paid themes or plugins?**
  _List all with license info, renewal dates, and transfer steps._

- **How is user data handled?**
  _Ensures compliance with privacy regulations (GDPR, CCPA, etc.)._

---

## 4. Domain & Hosting

- **What is the domain name and registrar?**
  _Include login credentials, renewal date, and DNS management details._

- **Who is the hosting provider and what is the plan?**
  _Include login, plan limits, renewal date, server type (shared, VPS, managed), and OS/version._

- **Are there custom DNS records or CDN settings?**
  _Document all A, CNAME, MX, TXT, and CDN configurations._

---

## 5. Server & Infrastructure

- **Server IP address(es) and control panel access (cPanel, Plesk, etc.)**

- **Are there specific server configurations (PHP version, memory limits, caching, etc.)?**

- **Is there a Web Application Firewall (WAF) or other security layers?**

---

## 6. Database

- **Database host, type, version, name(s), and user credentials**

- **phpMyAdmin or other DB management tool access**

- **Are there custom tables or modifications beyond standard WordPress?**

- **Backup schedule and restore procedures for the database**

---

## 7. WordPress Access

- **Admin URL, usernames, and passwords for all admin/editor accounts**

- **2FA or security plugins in use**

- **List of all user roles and permissions**

---

## 8. FTP/SFTP/SSH Access

- **FTP/SFTP/SSH host, port, credentials, and key pairs**

- **Location of authorized_keys and file/folder permissions**

- **Root directory path for WordPress installation**

---

## 9. Email

- **Email provider and account credentials**

- **SMTP settings and email forwarding/alias rules**

---

## 10. Plugins, Themes & Custom Code

- **List of all active/inactive plugins (with versions and license keys)**

- **List of all installed themes (active/inactive, parent/child, customizations, documentation)**

- **Custom plugins/themes (location, documentation, update schedule)**

- **Custom code snippets (functions.php, code snippet plugins, custom CSS/JS, etc.)**

- **Are there custom post types, taxonomies, or fields (e.g., via ACF)?**

---

## 11. Integrations & Third-Party Services

- **List all connected services (payments, analytics, email, CRM, APIs, etc.)**

- **Login credentials or API keys for each service**

- **Ownership transfer steps for each account**

---

## 12. Backups & Recovery

- **Backup solution in use (plugin, server, third-party)**

- **Backup schedule, retention policy, and storage location**

- **Restore procedures and last tested date**

---

## 13. Security

- **Security plugins and configurations (firewall, malware scanning, login limits, etc.)**

- **SSL certificate details (provider, expiry, renewal, auto-renewal)**

- **User roles and permissions management (Principle of Least Privilege)**

- **Any past security issues and resolutions**

---

## 14. Performance & Caching

- **Caching plugins or server-side caching**

- **CDN provider and credentials**

- **Performance monitoring tools and procedures for clearing caches**

---

## 15. Analytics & SEO

- **Google Analytics/Tag Manager/Search Console access**

- **SEO plugin settings (Yoast, RankMath, etc.)**

- **Sitemap location**

---

## 16. Environments & Deployment

- **Development/staging/production environments (URLs, access, sync process)**

- **Deployment process (manual, CI/CD, scripts, documented steps)**

- **Version control (Git repo URL, access, branching strategy, commit history)**

---

## 17. Documentation & Training

- **Location of project documentation/readme, technical specs, style guides**

- **Availability of training sessions or video walkthroughs**

- **Known issues, technical debt, and support contacts**

---

## 18. Support, Maintenance & Monitoring

- **Maintenance schedule (updates, backups, testing)**

- **Uptime/performance monitoring tools and alert contacts**

- **Post-handover support period, communication channels, and hourly rates**

---

## 19. Final Handover & Exit Interview

- **Schedule a formal handover meeting and confirm all accesses**

- **Use inventory tables as checklists; new owner logs into every service**

- **Change all passwords and enable 2FA**

- **Remove old users and revoke previous developer access**

- **Exit Interview Questions:**
  - What are the most fragile or complex parts of the site?
  - If you had more time, what would you improve?
  - Are there any quirks, oddities, or manual workarounds?
  - What were the biggest challenges and lessons learned?

---

## 20. Appendix: Inventory Tabular Data

### Master Credentials & Services Inventory Table

| SERVICE                     | DETAILS             | ACCESS                                             | USER                                                      | EVENT/ACTION                 | TOKENS             | COSTS             | DUE BY      |
| :------------------------- | :----------------- | :------------------------------------------------- | :------------------------------------------------------------ | :----------------------- | :----------------- | :--------------- | :----------- |
| Content/Assets            | CMS | [WordPress Admin](https://yourdomain.com/wp-admin)                  | `new_admin_user`                                              | Shared via Bitwarden     | --                 | Free               | N/A           |
| SSH/Domain                   | Registrar   | [GoDaddy](https://dcc.godaddy.com/)                         | [owner@org.com](mailto:owner@yourcompany.com)         | To be reset by new owner | --                 | $20      | `2025-10-15` |
| Hosting         | Linux/Web        | [SiteGround](https://login.siteground.com/)                    | [owner@org.com](mailto:owner@yourcompany.com)         | To be reset by new owner | --                 | $299        | `2025-09-01` |
| Payment                    | Processing | [Stripe](https://dashboard.stripe.com/)                    | [finance@org.com](mailto:finance@yourcompany.com)     | Existing account         | pk_live_&hellip;        | _TBD_ | --           |
| Cloud                | CDN/Firewall     | [CloudFlare](https://dash.cloudflare.com/)                     | [tech@org.com](mailto:tech@yourcompany.com)           | To be reset by new owner | `GLOBAL_SECRET` | $12        | Monthly      |
| Email                 | Marketing    | [MailChip](https://login.mailchimp.com/)                     | [marketing@org.com](mailto:marketing@yourcompany.com) | Existing account         | `API_KEY`        | $50        | Monthly      |
| Plugin | License: `PRO`     | [Adv. Custom Fields](https://www.advancedcustomfields.com/my-account/) | [dev@co.com](mailto:developer@oldcompany.com)   | Transfer license         | `LICENSE_TOKEN`    | $25         | `2025-07-22` |

### Plugin & Theme Audit Table

| NAME                       | KIND         | VERSION  | PURPOSE                   | COST     | TOKEN                      | NOTICE                                                                                      |
| :------------------------- | :----------- | :------- | :------------------------ | :------- | :------------------------- | :------------------------------------------------------------------------------------------ |
| Astra                      | Parent Theme | `4.1.5`  | Base theme framework      | Freemium | PRO license active         | Core visual framework; **DO NOT** edit directly.                                            |
| Astra Child                | Child Theme  | `1.x`    | Holds all custom CSS/PHP  | Custom   | `N/A`                      | All customizations should be made here.                                                     |
| WooCommerce                | Plugin       | `8.0.1`  | E-commerce functionality  | Free     | `N/A`                      | Critical for sales; complex settings.                                                       |
| Wordfence Security         | Plugin       | `^7.9.2` | Firewall & malware scan   | Premium  | Active - Renews 2025-01-30 | Firewall rules are configured; **DO NOT** deactivate.                                       |
| WP Rocket                  | Plugin       | `3.12.5` | Caching & performance     | Premium  | Active - Renews 2025-03-12 | Key for site speed. Purge cache after changes.                                              |
| Advanced Custom Fields PRO | Plugin       | `6.1.6`  | Manages all custom fields | Premium  | Missing/Expired            | **CRITICAL RISK** - Site layouts depend on this. **CANNOT UPDATE WITHOUT** a valid license. |
| Really Simple SSL          | Plugin       | `7.0.5`  | Manages SSL certificate   | Free     | `N/A`                      | **Redundant** - Hosting provides SSL. Can likely be removed after verification.             |
| Classic Editor             | Plugin       | `~1.6.3` | Disables Gutenberg editor | Free     | `N/A`                      | Indicates site may not be compatible with modern block editor. Creates technical debt.      |

> **Tip:** Attach all relevant files (configurations, SSH keys, documentation, license files) and ensure all credentials are up to date and securely stored.

---

## Conclusion

A robust handover ensures the new owner has full control, understands the website's architecture and processes, and is equipped to maintain and grow the site with confidence. Use this checklist to guide the transition, reduce risk, and set the stage for long-term success.
