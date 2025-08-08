# WordPress Project Handover: Comprehensive Due Diligence Checklist

## Introduction

The handover of a WordPress project is a critical process that goes beyond sharing files and passwords. It involves transferring strategic, technical, operational, and legal knowledge to empower the new owner with full control and autonomy. A poorly executed handover can lead to security vulnerabilities, operational downtime, legal liabilities, and increased costs due to undocumented technical debt. This comprehensive checklist combines detailed due diligence questions with practical steps to ensure a seamless transition, reduce risks, and establish a solid foundation for the website's future management and growth.

## Table of Contents

1. Project Overview & Intent
2. Stakeholders & Roles
3. Ownership & Legal
4. Domain & Hosting
5. Server & Infrastructure
6. Database
7. WordPress Access
8. FTP/SFTP/SSH Access
9. Email
10. Plugins, Themes & Custom Code
11. Integrations & Third-Party Services
12. Backups & Recovery
13. Security
14. Performance & Caching
15. Analytics & SEO
16. Environments & Deployment
17. Documentation & Training
18. Support, Maintenance & Monitoring
19. Final Handover & Exit Interview
20. Appendix: Inventory Tabular Data

---

## 1. Project Overview & Intent

Understanding the website's business context and history is essential for evaluating its technical decisions and anticipating future needs.

**Detailed Considerations:**

- The original intent provides a lens to assess features and design choices.
- Historical evolution can reveal technical debt or misaligned functionalities.

**Questions to Ask:**

- What was the original business problem this website was built to solve? What were the primary goals (e.g., e-commerce, lead generation, content hub)?
- Who was the target audience at the outset, and has it evolved over time?
- Can you provide a brief history of the project, including key milestones, major feature additions, or strategic pivots?
- What are the key performance indicators (KPIs) used to measure success (e.g., sales, signups, traffic)?
- Are there any unique business rules or workflows that the website must adhere to?

---

## 2. Stakeholders & Roles

Identifying the network of individuals involved ensures clear communication and responsibility mapping.

**Detailed Considerations:**

- Stakeholders influence decision-making and provide historical context.

**Questions to Ask:**

- Who are the key internal and external stakeholders (client, marketing team, etc.)? Who has final authority for approving changes?
- Who manages the website currently, and who will after handover?
- Which stakeholders participated in the original planning or discovery phase?

---

## 3. Ownership & Legal

Clarifying ownership and legal obligations prevents disputes and ensures compliance.

**Detailed Considerations:**

- Ambiguity in ownership can lead to intellectual property conflicts.
- Ongoing contracts affect financial planning.

**Questions to Ask:**

- Can you confirm in writing that upon final payment, we own 100% of the website, design, custom code, and content?
- Are there any ongoing contracts (e.g., hosting, support, SLAs)? List details.
- Are there paid themes or plugins? Provide license keys, purchase dates, renewal dates, and costs.
- What data privacy policies are in place (e.g., GDPR, CCPA)? Where is user data stored, and how is it protected?

---

## 4. Domain & Hosting

Control over the domain and hosting is critical for operational continuity.

**Detailed Considerations:**

- Domain registrar and hosting access are foundational assets.

**Questions to Ask:**

- What is the domain name and registrar (e.g., GoDaddy, Namecheap)? Provide login credentials, renewal date, and DNS details (A, CNAME, MX, TXT).
- Who manages DNS (registrar, Cloudflare, etc.)?
- Who is the hosting provider and what is the plan (e.g., shared, VPS, managed)? Include login, plan limits, renewal date, and server type.

---

## 5. Server & Infrastructure

Server details impact performance, security, and scalability.

**Detailed Considerations:**

- Specific configurations may be critical for functionality.

**Questions to Ask:**

- What are the server IP address(es) and control panel access (e.g., cPanel, Plesk)?
- What are the server OS, PHP, and MySQL/MariaDB versions?
- Are there custom server configurations (e.g., PHP memory limits, caching)?
- Is a Web Application Firewall (WAF) active (e.g., ModSecurity)?

---

## 6. Database

The database stores all content and settings, requiring secure access and management.

**Detailed Considerations:**

- Custom tables may indicate bespoke functionality.

**Questions to Ask:**

- What are the database host, type, version, name(s), and user credentials?
- Provide phpMyAdmin or other DB management tool access.
- Are there custom tables beyond standard WordPress? What is their purpose and schema?
- What is the backup schedule and restore procedure?

---

## 7. WordPress Access

Administrative access to WordPress is essential for content and configuration management.

**Detailed Considerations:**

- A new admin user ensures a clean transition.

**Questions to Ask:**

- What is the admin URL? Provide credentials for a new admin user (e.g., for <dylarcher@gmail.com>).
- List all admin/editor accounts, roles, and permissions.
- Is 2FA or any security plugin in use?

---

## 8. FTP/SFTP/SSH Access

Direct server access enables advanced maintenance and troubleshooting.

**Detailed Considerations:**

- Secure credentials prevent unauthorized access.

**Questions to Ask:**

- Provide FTP/SFTP/SSH host, port, credentials, and key pairs (private/public).
- Where is the authorized_keys file located?
- What is the root directory path for the WordPress installation?
- Are there specific file/folder permissions or restrictions?

---

## 9. Email

Email services tied to the website must be transferred.

**Detailed Considerations:**

- Email configurations affect communication workflows.

**Questions to Ask:**

- What is the email provider (e.g., Gmail, server-based)? Provide credentials if managed.
- What are the SMTP settings (host, port, username, password)?
- Are there email forwarding or alias rules?

---

## 10. Plugins, Themes & Custom Code

The software stack defines functionality and maintenance needs.

**Detailed Considerations:**

- Customizations impact updateability and stability.

**Questions to Ask:**

- List all active/inactive plugins (with versions, purposes, and license keys).
- List all installed themes (active/inactive, parent/child, customizations).
- Are there custom plugins/themes? Provide location and documentation.
- Is custom code in functions.php, a snippets plugin, or elsewhere (e.g., CSS/JS)? Document its purpose.
- Are custom post types, taxonomies, or fields used (e.g., via ACF)? How are they implemented?

**Plugin & Theme Audit Table:**

| Done? | Component Name | Type         | SemVer | Purpose                  | Premium/Free | License Key/Status | Notes/Risks          |
|-------|----------------|--------------|--------|--------------------------|--------------|--------------------|----------------------|
| ❌    | Astra          | Parent Theme | 4.1.5  | Base theme framework    | Freemium     | PRO license active | Do not edit directly |
| ❌    | Astra Child    | Child Theme  | 1.x    | Custom CSS/PHP          | Custom       | N/A                | Customization hub   |
| ❌    | WooCommerce    | Plugin       | 8.0.1  | E-commerce functionality| Free         | N/A                | Critical for sales  |

---

## 11. Integrations & Third-Party Services

External services are vital dependencies that must be controlled.

**Detailed Considerations:**

- Ownership transfer prevents service disruptions.

**Questions to Ask:**

- List all connected services (e.g., payments, analytics, CRM, APIs) with credentials/API keys.
- What is the process for transferring ownership of these accounts?

---

## 12. Backups & Recovery

A robust backup strategy protects against data loss.

**Detailed Considerations:**

- Tested restores ensure reliability.

**Questions to Ask:**

- What backup solution is used (e.g., plugin, server, third-party)? Specify tools, schedule, retention policy, and storage location.
- Are backups stored off-site (e.g., S3, Dropbox)?
- Provide the documented restore procedure. When was it last tested?

---

## 13. Security

Proactive security measures safeguard the website.

**Detailed Considerations:**

- Past issues inform current vulnerabilities.

**Questions to Ask:**

- What security plugins/tools are used (e.g., Wordfence)? Detail configurations (firewall, login limits).
- What is the SSL certificate provider, expiry, and renewal process?
- How are user roles and permissions managed (e.g., Principle of Least Privilege)?
- Any past security issues? How were they resolved?

---

## 14. Performance & Caching

Performance optimization enhances user experience and SEO.

**Detailed Considerations:**

- Caching layers require specific management.

**Questions to Ask:**

- What caching is in place (e.g., WP Rocket, server-side, CDN)? Provide credentials if applicable.
- What is the procedure for clearing caches?
- Is a CDN used (e.g., Cloudflare)? Detail settings.

---

## 15. Analytics & SEO

Analytics and SEO tools provide visibility into performance.

**Detailed Considerations:**

- Access ensures ongoing monitoring.

**Questions to Ask:**

- Provide Google Analytics, Tag Manager, and Search Console access.
- What SEO plugin is used (e.g., Yoast)? Detail settings.
- Where is the sitemap located?

---

## 16. Environments & Deployment

Deployment processes affect update safety and reliability.

**Detailed Considerations:**

- Staging reduces live site risks.

**Questions to Ask:**

- Are there development/staging/production environments? Provide URLs and access.
- What is the step-by-step deployment process (e.g., Git, manual)? Is it documented?
- Is version control used (e.g., Git repo URL, branching strategy)?

---

## 17. Documentation & Training

Documentation and training facilitate independent management.

**Detailed Considerations:**

- Training bridges knowledge gaps.

**Questions to Ask:**

- Where is project documentation (e.g., readme, specs, guides) located?
- Are training sessions or video walkthroughs available for common tasks?
- What are known issues or technical debt?

---

## 18. Support, Maintenance & Monitoring

Ongoing care ensures website health.

**Detailed Considerations:**

- Clear schedules prevent neglect.

**Questions to Ask:**

- What is the maintenance schedule (updates, backups, testing)?
- Are uptime/performance monitoring tools in place? Who receives alerts?
- What is the post-handover support period, communication channels, and hourly rates?

---

## 19. Final Handover & Exit Interview

The formal handover completes the transition.

**Detailed Considerations:**

- Exit interview uncovers critical insights.

**Steps to Complete:**

- Schedule a handover meeting for [insert date, e.g., 08/14/2025].
- Use inventory tables as checklists; new owner logs into every service.
- Change all passwords and enable 2FA.
- Remove old users and revoke previous developer access.

**Exit Interview Questions:**

- What are the most fragile or complex parts of the site?
- If you had more time, what would you improve?
- Are there any quirks, oddities, or manual workarounds?
- What were the biggest challenges and lessons learned?

---

## 20. Appendix: Inventory Tabular Data

### Master Credentials & Services Inventory Table

| Service/Platform         | Purpose             | Login URL                        | Username/Email           | Password Transfer Method | API Key         | Cost           | Renewal Date | Ownership Transfer Status |
|--------------------------|---------------------|----------------------------------|--------------------------|--------------------------|-----------------|----------------|--------------|---------------------------|
| WordPress Admin          | Content Management  | <https://yourdomain.com/wp-admin>  | new_admin_user           | Shared via Bitwarden     | --              | --             | --           | ✅                |
| GoDaddy                  | Domain Registrar    | <https://dcc.godaddy.com/>         | <owner@yourcompany.com>    | To be reset              | --              | $19.99/year    | 2025-10-15   | Completed         |
| SiteGround Hosting       | Web Hosting         | <https://login.siteground.com/>    | <owner@yourcompany.com>    | To be reset              | --              | $299/year      | 2025-09-01   | Completed         |

*Tip:* Attach relevant files (configurations, SSH keys, documentation, licenses) and store credentials securely.

---

## Conclusion

A successful handover ensures the new owner has full control, a deep understanding of the website's architecture, and the processes to maintain and grow it confidently. By addressing these questions and steps, the transition becomes a foundation for long-term success, minimizing risks and empowering independent management.
