# WordPress Project Takeover: A Guide to Due Diligence

A successful WordPress project takeover is not just about receiving files and passwords; it is a meticulous process of due diligence designed to ensure a seamless transfer of knowledge, ownership, and control. This guide provides a comprehensive framework for the incoming owner or team to de-risk the transition, uncover hidden liabilities, and establish a stable foundation for future management and development.

The process is framed as a series of critical questions. The goal is not to express distrust, but to achieve absolute clarity. An inability or unwillingness on the part of the seller or outgoing developer to provide clear, verifiable answers to these questions should be considered a significant red flag.

## 1. Foundational & Strategic Inquiry

Before diving into technical specifics, it is crucial to understand the strategic context and historical landscape of the project.

- What is the primary purpose and business model of the website?
  (e.g., e-commerce, lead generation, content publishing, SaaS)
  This clarifies the core business objectives that the website must support. Every technical decision should ultimately align with this purpose.
- What are the key performance indicators (KPIs) for success?
  (e.g., conversion rate, monthly recurring revenue, number of active users, lead form submissions)
  This defines what "success" looks like and ensures that future work is focused on metrics that matter.
- Who were the original stakeholders and what was the initial vision?
  Understanding the project's origin story can provide invaluable context for its current state, including its technical architecture and feature set.
- How has the website evolved over time? Have there been major pivots?
  This can uncover layers of legacy code, abandoned features, or "technical debt" that may complicate future development.

## 2. Ownership, Legal & Compliance

This is arguably the most critical phase of the takeover. Failure to secure unambiguous ownership of all assets can have catastrophic long-term consequences.

- Is there a formal contract or statement of work that explicitly transfers 100% of the intellectual property—including all custom code, graphics, and content—to us upon final payment?
  You must have this in writing. Without it, you may not truly own the work you paid for.
- Are there any ongoing contracts, licenses, or service level agreements (SLAs) that we will be inheriting?
  This includes hosting, premium plugin licenses, maintenance plans, and third-party service subscriptions. Request copies of all agreements.
- How is user data collected, stored, and managed? Is the site compliant with relevant privacy regulations (e.g., GDPR, CCPA)?
  Verify the existence of a clear privacy policy, cookie consent mechanisms, and processes for handling user data requests. Non-compliance can lead to severe legal and financial penalties.

## 3. Technical & Infrastructure Deep Dive

This section focuses on gaining complete administrative control and a deep understanding of the technical stack.

### Domain, DNS & Hosting

- **Who is the domain registrar?** Provide full account credentials.
- **Who is the hosting provider?** Provide full account credentials for the hosting control panel (e.g., cPanel, SiteGround, WP Engine).
- **What are the server specifications?** (e.g., Shared/VPS/Dedicated, OS, PHP version, memory limits).
- **Are there any custom DNS records or a Content Delivery Network (CDN) in place?** (e.g., Cloudflare). Provide full account credentials.

### WordPress & Database Access

- **What are the credentials for ALL administrator-level WordPress accounts?**
- **What is the direct access information for the database?** (Host, DB Name, DB User, DB Password).
- **Is there a database management tool like phpMyAdmin?** Provide access.

### Code & Version Control

- **Is the project under version control?** (e.g., Git). Provide access to the repository (e.g., GitHub, Bitbucket).
- **What is the branching strategy and deployment process?** Is it manual (FTP) or automated (CI/CD)?
- **Where is custom code located?** (e.g., a child theme, custom plugin). Request a full code walkthrough.
- **Provide a complete list of all plugins and themes (active and inactive).** Note which are premium and provide license keys and proof of transfer.

### Security, Backups & Email

- **What security measures are in place?** (e.g., security plugin, Web Application Firewall (WAF)). Provide access and configurations.
- **What is the backup solution?** (e.g., plugin, server-level). Confirm the schedule, storage location, and—most importantly—the **tested** restore procedure.
- **How are transactional emails (e.g., password resets, form notifications) handled?** (e.g., via a third-party service like SendGrid or Postmark). Provide credentials.

## 4. The Exit Interview: Uncovering "Tribal Knowledge"

The final step is a formal exit interview with the outgoing developer or team. This is where you uncover the "tribal knowledge"—the undocumented quirks and manual workarounds that are critical for smooth operation.

- What are the most fragile or complex parts of the site?
  This question encourages honesty about technical debt and potential problem areas.
- If you had another month to work on this project, what would you improve?
  This often reveals the developer's own assessment of the site's weaknesses and opportunities for improvement.
- Are there any quirks, oddities, or manual processes we should be aware of?
  This is perhaps the most valuable question of the entire handover. It is designed to capture the undocumented, informal knowledge that is essential for the smooth day-to-day operation of the site. These are the details that are never written down but can cause hours of frustration for a new team.
- What were the biggest challenges you faced during the project? What were the most important lessons learned?
  Understanding past struggles—whether with a particular plugin, a server configuration, or a third-party API—can help the new owner avoid repeating them.

## Conclusion

A successful WordPress project handover is a direct result of a diligent, systematic, and comprehensive process of inquiry. It is an exercise in proactive risk management, not an expression of mistrust. By methodically pursuing the answers to these questions, the incoming owner transforms the handover from a moment of high risk into an opportunity to establish a stable and secure foundation for the future. This upfront investment of time and diligence is the most effective strategy for protecting the value of the digital asset, ensuring business continuity, and dramatically reducing the long-term costs and complexities of website ownership.

## Appendix: Comprehensive Handover Checklist

### **Project Overview & Intent**

- [ ] What is the primary purpose of the website? (e.g., e-commerce, lead generation)
- [ ] Are there unique business rules or workflows?
- [ ] How has the website evolved over time?
- [ ] What are the key performance indicators (KPIs) for success?

### **Stakeholders & Roles**

- [ ] Who are the main points of contact?
- [ ] Who manages the website now, and who will after handover?
- [ ] Who participated in the original planning/discovery phase?

### **Ownership & Legal**

- [ ] Do we fully own the website, code, and content after payment?
- [ ] Are there ongoing contracts (hosting, support, SLAs)?
- [ ] Are there paid themes or plugins? (List all with license info, renewal dates, and transfer steps)
- [ ] How is user data handled? (GDPR, CCPA compliance)

### **Domain & Hosting**

- [ ] What is the domain name and registrar? (Include login, renewal date, DNS management details)
- [ ] Who is the hosting provider and what is the plan? (Include login, plan limits, renewal date, server type)
- [ ] Are there custom DNS records or CDN settings? (Document all A, CNAME, MX, TXT records)

### **Server & Infrastructure**

- [ ] Server IP address(es) and control panel access (cPanel, Plesk, etc.)
- [ ] Are there specific server configurations (PHP version, memory limits)?
- [ ] Is there a Web Application Firewall (WAF)?

### **Database**

- [ ] Database host, type, version, name(s), and user credentials.
- [ ] phpMyAdmin or other DB management tool access.
- [ ] Are there custom tables or modifications?
- [ ] Backup schedule and restore procedures for the database.

### **WordPress Access**

- [ ] Admin URL, usernames, and passwords for all admin/editor accounts.
- [ ] 2FA or security plugins in use.
- [ ] List of all user roles and permissions.

### **FTP/SFTP/SSH Access**

- [ ] FTP/SFTP/SSH host, port, credentials, and key pairs.
- [ ] Root directory path for WordPress installation.

### **Email**

- [ ] Email provider and account credentials.
- [ ] SMTP settings and email forwarding/alias rules.

### **Plugins, Themes & Custom Code**

- [ ] List of all active/inactive plugins (with versions and license keys).
- [ ] List of all installed themes (active/inactive, parent/child).
- [ ] Custom plugins/themes (location, documentation).
- [ ] Custom code snippets (functions.php, custom CSS/JS).
- [ ] Are there custom post types, taxonomies, or fields (e.g., via ACF)?

### **Integrations & Third-Party Services**

- [ ] List all connected services (payments, analytics, email, CRM, APIs).
- [ ] Login credentials or API keys for each service.
- [ ] Ownership transfer steps for each account.

### **Backups & Recovery**

- [ ] Backup solution in use (plugin, server, third-party).
- [ ] Backup schedule, retention policy, and storage location.
- [ ] Restore procedures and last tested date.

### **Security**

- [ ] Security plugins and configurations.
- [ ] SSL certificate details (provider, expiry, renewal).
- [ ] User roles and permissions management (Principle of Least Privilege).
- [ ] Any past security issues and resolutions.

### **Performance & Caching**

- [ ] Caching plugins or server-side caching.
- [ ] CDN provider and credentials.
- [ ] Performance monitoring tools and procedures for clearing caches.

### **Analytics & SEO**

- [ ] Google Analytics/Tag Manager/Search Console access.
- [ ] SEO plugin settings (Yoast, RankMath, etc.).
- [ ] Sitemap location.

### **Environments & Deployment**

- [ ] Development/staging/production environments (URLs, access, sync process).
- [ ] Deployment process (manual, CI/CD, scripts).
- [ ] Version control (Git repo URL, access, branching strategy).

### **Documentation & Training**

- [ ] Location of project documentation, technical specs, style guides.
- [ ] Availability of training sessions or video walkthroughs.
- [ ] Known issues, technical debt, and support contacts.

### **Final Handover & Exit Interview**

- [ ] Schedule a formal handover meeting.
- [ ] Use inventory tables as checklists; new owner logs into every service.
- [ ] **Change all passwords and enable 2FA.**
- [ ] **Remove old users and revoke previous developer access.**
- [ ] Conduct Exit Interview (What's fragile? What would you improve? Any quirks?)

### **Inventory Tables**

#### Master Credentials & Services Inventory

| **Service/Platform** | **Purpose**        | **Login URL** | **Username / Account Email** | **Password Transfer Method** | **API Key (if applicable)** | **License/Subscription Cost** | **Renewal Date** | **Ownership Transfer Status** |
| ---------------------- | -------------------- | --------------- | ------------------------------ | ------------------------------ | ----------------------------- | ------------------------------- | ------------------ | ------------------------------- |
| WordPress Admin      | Content Management | `[URL]`       | `[user]`                     | `[method]`                   | --                          | --                            | --               | [ ]                           |
| Domain Registrar     | Domain             | `[URL]`       | `[user]`                     | `[method]`                   | --                          | `[cost]`                      | `[date]`         | [ ]                           |
| Web Hosting          | Hosting            | `[URL]`       | `[user]`                     | `[method]`                   | --                          | `[cost]`                      | `[date]`         | [ ]                           |
| Stripe               | Payments           | `[URL]`       | `[user]`                     | `[method]`                   | `[key]`                     | `[cost]`                      | `[date]`         | [ ]                           |
| Cloudflare           | CDN / Firewall     | `[URL]`       | `[user]`                     | `[method]`                   | `[key]`                     | `[cost]`                      | `[date]`         | [ ]                           |
| Mailchimp            | Email              | `[URL]`       | `[user]`                     | `[method]`                   | `[key]`                     | `[cost]`                      | `[date]`         | [ ]                           |
| ACF PRO              | Plugin License     | `[URL]`       | `[user]`                     | `[method]`                   | `[key]`                     | `[cost]`                      | `[date]`         | [ ]                           |

#### Plugin & Theme Audit

| **Done?** | **Component Name** | **Type**     | **Version** | **Purpose**    | **Premium/Free** | **License Key/Status** | **Notes/Risks**                          |
| ----------- | -------------------- | -------------- | ------------- | ---------------- | ------------------ | ------------------------ | ------------------------------------------ |
| [ ]       | Astra              | Parent Theme | `x.x.x`     | Base theme     | Freemium         | `[key]`                | Core framework;**DO NOT** edit directly. |
| [ ]       | Astra Child        | Child Theme  | `x.x.x`     | Customizations | Custom           | N/A                    | All customizations should be made here.  |
| [ ]       | WooCommerce        | Plugin       | `x.x.x`     | E-commerce     | Free             | N/A                    | Critical for sales; complex settings.    |
| [ ]       | Wordfence          | Plugin       | `x.x.x`     | Security       | Premium          | `[key]`                | Firewall rules are configured.           |
| [ ]       | WP Rocket          | Plugin       | `x.x.x`     | Caching        | Premium          | `[key]`                | Key for site speed.                      |
