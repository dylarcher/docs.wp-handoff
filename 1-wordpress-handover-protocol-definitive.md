# <a href="#top">#</a> The Definitive WordPress Handover Protocol: A Comprehensive Due Diligence Questionnaire

The handover of a WordPress project is a critical inflection point in the lifecycle of a digital asset. It is frequently misconstrued as a simple, transactional event involving the exchange of files & passwords. This perspective is dangerously incomplete. A successful handover is not an event but a comprehensive process of knowledge transfer, moving far beyond the delivery of technical components to encompass the full strategic, legal, & operational context of the website[^1]. The ultimate objective is to de-risk the transition by eliminating dependency on the departing developer, thereby empowering the new owner w/complete & unencumbered autonomy over their digital property.

## <a href="#intro">#</a> Introduction

The stakes of a poorly executed handover are exceptionally high. An incomplete transfer can precipitate a cascade of negative consequences that manifest long after the original developer has departed. These risks include severe security vulnerabilities stemming from lingering, unauthorized access to critical systems[^3]; operational downtime caused by unknown dependencies or undocumented, fragile workflows[^5]; significant legal liabilities arising from ambiguous ownership of intellectual property or non-compliance w/data privacy regulations[^6]; & escalating future costs as the new team grapples w/undocumented **technical debt** that is difficult & expensive to remediate[^8]. Many of these issues can be traced back to a failure to ask the right questions at the right time.

This guide provides a structured, exhaustive set of questions designed to serve as a definitive due diligence protocol for any WordPress project handover. It is engineered to be a practical tool, enabling the incoming owner or team to proactively identify, assess, & mitigate the myriad risks inherent in the transition process. By systematically addressing each area—from high-level strategy to the most granular technical detail—the new owner can ensure a truly complete & seamless transfer of control, establishing a firm foundation for the future management, maintenance, & growth of the website.

---

[`🔼 RETURN TO TOP`](#top)

## <a href="#part-1">#</a> Part I: Strategic & Commercial Foundation

Before any technical examination of the website can be meaningful, it is imperative to establish a deep understanding of its business context. The technical architecture, features, & code are merely instruments designed to serve a strategic purpose. Their quality & appropriateness can only be judged against the business goals they were intended to achieve. This section provides the questions necessary to uncover the **why** behind the website, clarifying its purpose, history, stakeholders, & the legal framework that governs it.

### <a href="#project-purpose-history">#</a> A. Project Purpose & History

Understanding the original intent & historical evolution of a project is fundamental. It provides the context for all subsequent technical decisions & can reveal architectural layers or features that may no longer align w/the current business strategy. This historical perspective is a map to understanding the site's current state & its potential hidden complexities.

- **What was the original business problem this website was built to solve? What were the primary goals & objectives defined at the project's inception?**
 This foundational question seeks to establish the core rationale for the website's existence[^2]. A clear answer, such as **to generate qualified leads for our consulting services** or **to sell handmade goods directly to consumers,** provides a lens through which all features & design choices can be evaluated. A vague or non-existent answer may indicate a lack of strategic direction from the outset, which can often translate into a disjointed & ineffective website.
- **Who was the target audience defined at the project's outset, & has that audience evolved over time?**
 A website's design, content, & functionality should be tailored to its intended users[^5]. Understanding the defined audience helps assess the appropriateness of the user experience (UX) & user interface (UI). Furthermore, inquiring about the evolution of this audience can highlight areas where the site may need to be adapted to meet new user needs or demographic shifts.
- **Can you provide a brief history of the project, including key milestones, major feature additions, or significant strategic pivots?**
 This question is not merely about creating a timeline; it is a powerful diagnostic tool for uncovering technical debt[^1]. A project's history is often a story of its compromises. For example, a website that began as a simple **brochure** site & later had e-commerce functionality **bolted on** may suffer from significant architectural weaknesses. The theme may not be optimized for online sales, or the chosen e-commerce plugin might be poorly integrated, leading to performance issues & maintenance nightmares. Understanding these historical pivots allows the new owner to probe deeper into the implementation of major features & anticipate areas of fragility that are not immediately apparent from a surface-level review.
- **What were the key performance indicators (KPIs) used to measure the website's success?**
 Knowing the metrics that matter—such as lead conversion rates, average order value, or user engagement time—clarifies what aspects of the site are considered most valuable[^2]. This information is crucial for prioritizing future development efforts & ensuring that any changes made do not negatively impact the site's primary commercial or strategic functions.

### <a href="#stakeholder-audience-landscape">#</a> B. Stakeholder & Audience Landscape

A website does not exist in a vacuum. It serves & is managed by a network of individuals, each w/their own set of expectations & responsibilities. Identifying these stakeholders is essential for establishing clear lines of communication & understanding the project's internal political landscape.

- **Who are the key internal & external stakeholders involved w/the website? Who has the final authority for approving changes?**
 This question aims to create a definitive map of influence & responsibility[^1]. The answer should identify the project owner, marketing team members, content editors, & any other individuals who have a vested interest in the site's operation. Crucially, it must clarify the approval workflow, which will prevent future delays & conflicts when changes need to be implemented.
- **Which stakeholders were involved in the original 'Discovery' or research phase of the project?**
 The initial research or **Discovery** phase is where the foundational requirements & strategies for a project are established[^10]. Identifying the participants of this phase provides a direct line to the sources of the original project vision. If questions arise later about why a particular feature was built in a certain way, these are the individuals who will likely hold the answer.

### <a href="#commercial-legal-framework">#</a> C. Commercial & Legal Framework

The handover process involves the transfer of a valuable business asset, & w/it comes a host of commercial & legal responsibilities. Failing to clarify these details can lead to severe financial & legal repercussions, including loss of ownership, unexpected costs, & data privacy violations.

- **Can you confirm in writing that upon final payment, our organization will have 100% ownership of the website, its design, all custom-developed code, & all content created specifically for the project?**
 This is arguably one of the most critical questions in the entire handover process. It directly addresses the fundamental issue of asset ownership.[^7] Ambiguity in contracts or verbal agreements has led to numerous disputes where developers claim ownership of the work, effectively holding the client's website hostage[^11]. A clear, written confirmation of a complete transfer of intellectual property rights is non-negotiable.
- **Are there any third-party or premium software licenses (for themes, plugins) that need to be transferred or repurchased? Please provide a comprehensive list of all such software, including license keys, original purchase dates, renewal dates, & annual costs.**
 Modern WordPress sites are often built upon a foundation of premium themes & plugins. These components require active licenses to receive crucial security updates & technical support.[^5] If these licenses are registered to the departing developer, they may expire without the new owner's knowledge, leaving the site vulnerable to security exploits or causing critical features to cease functioning. A complete inventory of these licenses is essential for both security & financial planning.
- **Are there any ongoing service level agreements (SLAs), hosting contracts, or other contractual obligations w/your company or external third parties that we will be inheriting?**
 This question aims to uncover any hidden or recurring financial commitments associated w/the website.[^1] The new owner must be aware of all contracts they are assuming, whether for specialized hosting, maintenance retainers, or other third-party services. This prevents unexpected invoices & ensures continuity of essential services.
- **What data privacy agreements or policies are in place to comply w/regulations such as GDPR or CCPA? Where is user data stored, & what measures are in place to protect it?**
 In the modern regulatory environment, data privacy is a significant area of legal liability.[^6] The new owner must understand how the website collects, stores, & manages personally identifiable information (PII). This includes data from contact forms, e-commerce transactions, & user registrations. The developer should be able to point to the relevant privacy policy pages & explain the technical safeguards that have been implemented to ensure compliance.

---

[`🔼 RETURN TO TOP`](#top)

## <a href="#part-2">#</a> Part II: The Keys to the Kingdom: Access, Credentials, & Third-Party Services

This section constitutes a non-negotiable inventory of all access points required to control the website & its surrounding ecosystem. The primary goal is to achieve full, exclusive administrative control over every component. A handover cannot be considered complete until every credential has been securely transferred & the previous developer's access has been systematically & verifiably revoked from every platform. Failure to do so represents a critical & ongoing security risk.[^3]

### <a href="#core-platform-credentials">#</a> A. Core Platform Credentials

These are the fundamental access points for managing the website's content, hosting environment, & domain name. Without these, the new owner is effectively locked out of their own property.

- **Please provide credentials for a new, unique Administrator-level user for the WordPress dashboard.**
 It is a critical best practice to never take over an existing user account[^8]. A new, dedicated administrator account should be created for the new owner. This ensures a clean audit trail & prevents any ambiguity about who performed which actions. Once the new owner has confirmed their access, all other administrator accounts, including the one used by the departing developer, should be demoted or deleted.
- **What are the login details for the website's hosting control panel (e.g., cPanel, Plesk, or a custom provider dashboard)?**
 The hosting control panel is the gateway to the server environment. It allows for the management of files, databases, email accounts, & other server-level configurations[^8]. Access to this panel is essential for troubleshooting, performing backups, & managing the underlying infrastructure of the website.
- **What are the login details for the domain registrar (e.g., GoDaddy, Namecheap) where the site's domain name is managed?**
 Control over the domain registrar account is paramount[^13]. This account governs the ownership of the domain name itself, as well as the DNS settings that direct traffic to the web server. Losing control of this account can result in the loss of the domain name, a catastrophic event for any business. The new owner must ensure that the account is transferred into their name & that they control the billing information for renewals.

### <a href="#infrastructure-development-access">#</a> B. Infrastructure & Development Access

For more advanced management, maintenance, & development, direct access to the server's file system & database is often required.

- **Please provide SFTP (Secure File Transfer Protocol) or SSH (Secure Shell) credentials for direct file access to the server.**
 SFTP/SSH access allows for the direct manipulation of WordPress core files, themes, & plugins[^4]. This level of access is necessary for manual updates, troubleshooting complex issues, & managing file permissions. Each user who requires this access should have their own unique credentials.
- **What are the credentials for direct database access, including the Database Name, Username, Password, & Hostname?**
 The WordPress database is the heart of the website, storing all content, settings, & user information. Direct access via a tool like phpMyAdmin (often available through the hosting control panel) is sometimes necessary for complex data migrations, repairs, or manual cleanup[^8]. These credentials should be treated w/the utmost security.

### <a href="#integrated-services-apis">#</a> C. Integrated Services & APIs

Modern websites are rarely monolithic; they are ecosystems of interconnected services. Each of these services represents an access point that must be controlled.

- **Please provide a comprehensive list of all third-party services integrated w/the site. This must include, but is not limited to: Payment Gateways (e.g., Stripe, PayPal), Content Delivery Networks (CDNs) like Cloudflare, Email Marketing Platforms (e.g., Mailchimp, ConvertKit), CRM systems, Analytics platforms (e.g., Google Analytics, Google Tag Manager), & any other services connected via an API key.**
 This question forces a thorough inventory of the entire digital ecosystem[^5]. Many critical site functions, such as payment processing or email list sign-ups, depend on these external services. Without a complete list, the new owner may be unaware of a dependency until it fails.
- **For each service identified, what are the login credentials or API keys, & what is the process for transferring ownership of these accounts to us?**
 It is not enough to simply have the login details; legal & administrative ownership of these third-party accounts must be transferred[^5]. This often involves the departing developer adding the new owner as an administrator, who then removes the developer's access. For services using API keys, these keys should be regenerated after the handover to invalidate the old ones.

### <a href="#the-secure-transfer-process">#</a> D. The Secure Transfer Process

The method by which credentials are transferred is as important as the credentials themselves. Insecure practices can expose sensitive information & undermine the entire handover process.

- `ACTION ITEM` **Insist on Secure Credential Sharing.**
 Under no circumstances should passwords or API keys be sent in plain text via email, as this is a major security vulnerability[^13]. The new owner should insist on the use of a secure sharing method, such as a one-time, self-destructing note service (e.g., Privnote) or, preferably, a shared vault within a reputable password manager (e.g., 1Password, Bitwarden).
- `ACTION ITEM` **Immediate Credential Rotation & 2FA Activation.**
 Upon receiving all credentials, the new owner's first action should be to log in to every single service, change the password to a new, strong, & unique one, & enable two-factor authentication (2FA) wherever possible. This immediately secures the accounts under the new owner's control.
- `ACTION ITEM` **Systematic Revocation of Old Access.**
 The final & most crucial step of the access transfer is to systematically remove the previous developer's user accounts from every platform: WordPress, hosting, domain registrar, CDN, & all other third-party services[^3]. This step should be performed methodically, using the inventory created as a checklist. The handover is not complete until this de-provisioning process is finished.

To facilitate this critical process, the use of a centralized inventory document is strongly recommended. The following table provides a template for creating a single source of truth for all access points, which serves as both an inventory & a dynamic checklist for the transfer of ownership.

### <a href="#master-credentials-services-inventory">#</a> Master Credentials & Services Inventory

| Service/Platform           | Purpose            | Login URL                                          | Username / Account Email                                      | Password Transfer Method | API Key (if applicable) | License/Subscription Cost | Renewal Date | Ownership Transfer Status |
| -------------------------- | ------------------ | -------------------------------------------------- | ------------------------------------------------------------- | ------------------------ | ----------------------- | ------------------------- | ------------ | ------------------------- |
| WordPress Admin            | Content Management | <https://yourdomain.com/wp-admin>                  | `new_admin_user`                                              | Shared via Bitwarden     | --                      | --                        | --           | :check:                   |
| GoDaddy                    | Domain Registrar   | <https://dcc.godaddy.com/>                         | [owner@yourcompany.com](mailto:owner@yourcompany.com)         | To be reset by new owner | --                      | $19.99/year               | `2025-10-15` | Completed                 |
| SiteGround Hosting         | Web Hosting        | <https://login.siteground.com/>                    | [owner@yourcompany.com](mailto:owner@yourcompany.com)         | To be reset by new owner | --                      | $299/year                 | `2025-09-01` | Completed                 |
| Stripe                     | Payment Processing | <https://dashboard.stripe.com/>                    | [finance@yourcompany.com](mailto:finance@yourcompany.com)     | Existing account         | pk_live_...             | Transaction fees          | --           | Completed                 |
| Cloudflare                 | CDN / Firewall     | <https://dash.cloudflare.com/>                     | [tech@yourcompany.com](mailto:tech@yourcompany.com)           | To be reset by new owner | [Global API Key]        | $20/month                 | Monthly      | Completed                 |
| Mailchimp                  | Email Marketing    | <https://login.mailchimp.com/>                     | [marketing@yourcompany.com](mailto:marketing@yourcompany.com) | Existing account         | [API Key]               | $50/month                 | Monthly      | Completed                 |
| Advanced Custom Fields PRO | Plugin License     | <https://www.advancedcustomfields.com/my-account/> | [developer@oldcompany.com](mailto:developer@oldcompany.com)   | Transfer license         | [License Key]           | $49/year                  | `2025-07-22` | _Pending_                 |

This structured approach transforms a potentially chaotic & insecure exchange into a systematic & auditable process. It forces a complete inventory, preventing omissions of forgotten but critical services like a transactional email API. By including columns for cost & renewal dates, the table evolves from a simple access log into a vital financial & operational planning tool, preventing unexpected service disruptions due to non-payment[^7]. The **Ownership Transfer Status** column acts as a progress tracker, providing a clear visual indicator of what has been completed & what remains, ensuring that the critical final step of revoking the old developer's access is never overlooked.[^4]

---

[`🔼 RETURN TO TOP`](#top)

## <a href="#part-3">#</a> Part III: Deconstructing the Technical Architecture

Understanding how a website was built is a prerequisite for being able to effectively maintain, troubleshoot, & extend it. This section focuses on creating a comprehensive **blueprint** of the site's technical construction. The questions are designed to uncover the development practices, tools, & structural decisions that define the website's functionality and, by extension, its future maintainability.

### <a href="#the-code-repository-version-control">#</a> A. The Code Repository & Version Control

The use of a version control system (VCS) like Git is a hallmark of professional web development. It provides a complete history of changes, facilitates collaboration, & enables safe deployment & rollback procedures.

- **Is the website's code managed in a version control system like Git? If so, please provide access to the repository (e.g., on GitHub, Bitbucket, or GitLab).**
 The answer to this question is a primary indicator of the developer's professionalism. If the code is managed in a repository, it suggests a structured & disciplined workflow.[^8] If the answer is _no_, or if the developer is unfamiliar w/the concept, it is a major red flag. It implies that changes were likely made directly on the live server via FTP, a practice that is highly prone to error & offers no way to track changes or revert mistakes.
- **What is the branching strategy used in the repository (e.g., GitFlow, feature branches)? Which branch represents the code currently running on the live production site?**
 Understanding the branching strategy is key to safely contributing new code. A common practice is to have a main or master branch that reflects the live site, a develop branch for integrating new features, & separate feature branches for individual tasks. Knowing this structure prevents accidental deployments of unfinished work to the production environment.
- **Can you confirm that the repository contains the complete & unabridged history of the project's development?**
 A repository w/a shallow or very recent commit history may indicate that version control was not used consistently throughout the project's life. A complete history is an invaluable diagnostic tool, allowing the new owner to see when & why specific changes were made.

### <a href="#theme-parent-child-theme-structure">#</a> B. Theme & Parent/Child Theme Structure

The WordPress theme controls the entire visual presentation of the site. The way it has been structured & customized has profound implications for future updates & maintenance.

- **What theme is the site built on? Is it a pre-built commercial theme from a marketplace, or is it a fully custom theme built from scratch?**
 This question establishes the foundation of the site's design.[^10] If it is a commercial theme, the new owner will need to know where to find its documentation & support channels. If it is a custom theme, all documentation must come from the departing developer.
- **If it's a commercial theme, is a child theme being used for all customizations? Can you provide explicit confirmation that no modifications have been made directly to the parent theme's files?**
 This is a critically important technical question. The WordPress best practice for customizing a commercial theme is to use a child theme[^5]. A child theme inherits all the functionality & styling of the parent theme but allows customizations to be stored in separate files. This structure ensures that when the parent theme is updated (for example, to patch a security vulnerability), the custom modifications are not overwritten & lost. If the developer has edited the parent theme's files directly, the site becomes **un-updateable,** posing a massive long-term security & maintenance risk.
- **Where are the theme's original purchase files & official documentation located?**
 For any commercial theme, having access to the original.zip file & the official documentation is essential for troubleshooting & understanding its built-in features & options.

### <a href="#plugin-ecosystem-audit">#</a> C. Plugin Ecosystem Audit

Plugins extend the core functionality of WordPress, but they also add complexity & potential points of failure. A thorough audit of the plugin stack is essential for assessing the site's health & security.

- **Please provide a complete list of all installed plugins. For each plugin, can you briefly explain its purpose & the rationale for why it was chosen over alternatives?**
 This question forces a justification for each component of the site's software stack[^5]. It helps identify plugins that may be redundant, unnecessary, or not the best tool for the job. A site w/an excessive number of plugins can suffer from poor performance & an increased attack surface.
- **Which of these plugins are premium (paid) versions? Please provide the associated license keys & account information required to receive future updates & technical support.**
 As w/premium themes, premium plugins require active licenses for updates[^12]. An expired license can leave a plugin vulnerable to known exploits. This information should be recorded in the Master Credentials & Services Inventory.
- **Are there any custom-built plugins developed specifically for this site? If so, where is their source code managed, & is there documentation for their functionality?**
 A custom plugin represents a piece of bespoke software that the new owner will be responsible for maintaining[^11]. It is crucial to have access to its source code (ideally in the same Git repository as the theme) & comprehensive documentation explaining what it does & how it works.
- **Are there any known conflicts between plugins in the current stack, or are there any plugins known to cause performance issues?**
 This question seeks to uncover latent problems that may not be immediately obvious. An experienced developer will often be aware of subtle conflicts or performance bottlenecks caused by specific combinations of plugins.

### <a href="#custom-code-development-practices">#</a> D. Custom Code & Development Practices

Beyond the theme & plugins, custom code can be added in various places within WordPress. Locating & understanding all custom code is vital for preventing accidental breakage.

- **Is there any custom PHP code that has been added to the theme's functions.php file or implemented via a code snippets plugin?**
 The functions.php file is a common location for developers to add custom functionality, from simple tweaks to complex features[^5]. A code snippets plugin is another popular method. All such code must be documented & understood, as it can have a significant impact on the site's behavior.
- **Where is custom CSS or JavaScript stored? Is it located in the theme customizer's 'Additional CSS' field, within the child theme's stylesheet, or loaded via other methods?**
 Custom styling (CSS) & interactivity (JavaScript) can be injected in multiple ways[^11]. A systematic developer will consolidate all custom code in the child theme's
 style.css & scripts.js files. A less organized approach might scatter code across theme options panels, customizer fields, & even within the content of individual pages. A full inventory is needed to ensure that styles are not lost or overridden during future development.
- **Was a specific coding standard (e.g., the official WordPress Coding Standards) followed during the development of custom code? Is the custom code well-commented to explain its purpose & logic?**
 Code that adheres to a standard is easier for other developers to read & understand. More importantly, well-commented code is exponentially easier & cheaper to maintain[^8]. Code without comments forces the new developer to spend significant time reverse-engineering its purpose, which increases costs & the risk of introducing new bugs.

### <a href="#database-content-structure">#</a> E. Database & Content Structure

The way content is structured in the WordPress database dictates how it can be managed & displayed. Understanding this structure is key to managing the site's information architecture.

- **Does the site utilize custom post types, custom fields, or custom taxonomies? If so, how were these created (e.g., w/custom code in functions.php, or w/a plugin like Advanced Custom Fields (ACF) or Custom Post Type UI)?**
 These features allow for the creation of structured content beyond standard posts & pages (e.g., **Team Members,** **Events,** **Products**)[^5]. Knowing how they were implemented is crucial for maintenance. If they were created w/a plugin like ACF, the new owner must understand how to manage the field groups.
- **If the site uses a page builder (e.g., Elementor, Beaver Builder, Divi) or a framework like ACF, are there any global settings, saved templates, or reusable blocks that I should be aware of?**
 Modern page builders & frameworks often include powerful systems for creating global elements (like headers & footers) & reusable content templates[^12]. Understanding where these global settings are controlled is essential to avoid making a change on one page that unintentionally affects the entire site.
- **Are there any custom database tables that were created for the site, separate from the standard WordPress tables? If so, what is their purpose & what is their schema?**
 While less common, some plugins or custom solutions create their own tables in the database[^8]. These tables will not be understood by standard WordPress functions, & their purpose must be thoroughly documented.

To consolidate this architectural audit, a detailed inventory of all active software components is invaluable. The following table provides a template for this audit, functioning as both an inventory & a risk assessment tool.

### <a href="#checklist">#</a> Plugin & Theme Audit

| Done? | Component Name             | Type         | SemVer   | Purpose                   | Premium/Free | License Key/Status         | Notes/Risks                                                                                          |
| :---: | -------------------------- | ------------ | -------- | ------------------------- | ------------ | -------------------------- | ---------------------------------------------------------------------------------------------------- |
|  ❌   | Astra                      | Parent Theme | `4.1.5`  | Base theme framework      | Freemium     | PRO license active         | Core visual framework; <ins>DO NOT</ins> edit directly.                                              |
|  ❌   | Astra Child                | Child Theme  | `1.x`    | Holds all custom CSS/PHP  | Custom       | `N/A`                      | All customizations should be made here.                                                              |
|  ❌   | WooCommerce                | Plugin       | `8.0.1`  | E-commerce functionality  | Free         | `N/A`                      | Critical for sales; complex settings.                                                                |
|  ❌   | Wordfence Security         | Plugin       | `^7.9.2` | Firewall & malware scan   | Premium      | Active - Renews 2025-01-30 | Firewall rules are configured; <ins>DO NOT</ins> deactivate.                                         |
|  ❌   | WP Rocket                  | Plugin       | `3.12.5` | Caching & performance     | Premium      | Active - Renews 2025-03-12 | Key for site speed. Purge cache after changes.                                                       |
|  ❌   | Advanced Custom Fields PRO | Plugin       | `6.1.6`  | Manages all custom fields | Premium      | Missing/Expired            | **`CRITICAL RISK`** - Site layouts depend on this. <ins>CANNOT UPDATE WITHOUT</ins> a valid license. |
|  ❌   | Really Simple SSL          | Plugin       | `7.0.5`  | Manages SSL certificate   | Free         | `N/A`                      | **Redundant** - Hosting provides SSL. Can likely be removed after verification.                      |
|  ❌   | Classic Editor             | Plugin       | `~1.6.3` | Disables Gutenberg editor | Free         | `N/A`                      | Indicates site may not be compatible w/modern block editor. Creates technical debt.                  |

This systematic audit transforms a simple list of plugins into a powerful strategic document. It immediately highlights critical dependencies & risks. For instance, the **Missing/Expired** license for ACF PRO is a red alert; it means a core component of the site cannot receive security updates & may break in a future version of WordPress. The presence of the Classic Editor plugin signals that the site is built on older technology & will require significant effort to modernize. This table provides the new owner w/an immediate, prioritized action plan for stabilizing & improving the website.

---

[`🔼 RETURN TO TOP`](#top)

## <a href="#part-4">#</a> Part IV: The Hosting Environment & Deployment Pipeline

A website's code is only one half of the equation; the infrastructure it runs on is the other. The hosting environment dictates the site's performance, security, scalability, & reliability. This section delves into the specifics of the server & the processes used to deploy changes, which together form the operational foundation of the website.

### <a href="#server-hosting-plan-details">#</a> A. Server & Hosting Plan Details

Understanding the specifics of the hosting plan is the first step in assessing the site's infrastructural capabilities & limitations.

- > Knowing the provider & plan name allows the new owner to look up the official specifications, features, & support policies[^16]. Different hosts & plans offer vastly different levels of performance & service.
  - **Who is the hosting provider? What is the specific name of the hosting plan (e.g., 'Managed WordPress - Grow', 'VPS Level 3')?**
- > Every hosting plan has resource constraints[^16]. Exceeding these limits can result in overage fees or, in a worst-case scenario, the suspension of the website. The PHP memory limit is a particularly important figure, as insufficient memory can cause errors & crashes, especially on sites w/many plugins or high traffic.
  - **What are the key resource limits of this plan, such as storage space, monthly visits or bandwidth, & the PHP memory limit?**
- > The type of hosting defines the level of control, responsibility, & performance isolation.[^17]
  - **Is this a shared, VPS (Virtual Private Server), dedicated, or managed WordPress hosting environment?**
    - **Shared Hosting** - The cheapest option, but resources are shared w/many other websites, leading to potential performance & security issues (the **noisy neighbor** effect).
    - **VPS Hosting** - Offers a dedicated slice of server resources, providing better performance & more control than shared hosting.
    - **Dedicated Hosting** - An entire physical server is dedicated to the website, offering maximum performance & control but requiring expert management.
    - **Managed WordPress Hosting** - A specialized environment optimized specifically for WordPress. The host manages security, backups, & updates, offering convenience at a higher price point. It may also come w/restrictions on which plugins can be used.[^18]
- > This is a critical piece of financial information needed for budgeting & ensuring the continuity of service[^7]. This data should be logged in the Master Credentials & Services Inventory.
  - **What is the current cost of the hosting plan, & what is its renewal date?**

### <a href="#server-configuration-dependencies">#</a> B. Server Configuration & Dependencies

The software running on the server can have a major impact on the website's compatibility & security.

- **What versions of PHP & MySQL/MariaDB is the server currently running?**
 WordPress relies on PHP (the programming language) & MySQL or MariaDB (the database software). Using outdated versions of this software can expose the site to serious security vulnerabilities & prevent the use of modern themes & plugins[^5]. Conversely, a site built on old code may not be compatible w/the latest PHP versions.
- **Are there any specific server configurations (e.g., custom php.ini settings) or required PHP extensions that are critical for the site to function properly?**
 Sometimes, a specific plugin or theme requires a non-standard server setting or a particular PHP extension to be enabled. This information is crucial for disaster recovery or if the site ever needs to be migrated to a new hosting environment. Without this knowledge, the site may fail to work correctly on a new server.
- **Is there a Web Application Firewall (WAF) active at the server level (e.g., ModSecurity or a provider-specific firewall)?**
 A WAF provides an important layer of security by filtering malicious traffic before it even reaches WordPress[^20]. Understanding if a server-level WAF is in place helps to form a complete picture of the site's security posture.

### <a href="#staging-production-workflow">#</a> C. The Staging & Production Workflow

The process of moving changes from a development environment to the live production site is one of the most risk-prone activities in website management. A disciplined, well-documented workflow is a sign of a mature development practice, while an ad-hoc process is a recipe for disaster.

- > A staging site is a private clone of the live site used for testing changes safely[^12]. Professional hosting providers often include one-click staging environments. The absence of a staging site means that updates & changes are likely being tested directly on the live site, a practice that is extremely risky & can easily lead to public-facing errors or downtime.
  - **Is there a dedicated staging or development environment? If so, how is it kept in sync w/the production site?**
- > This question probes the very core of the developer's operational discipline[^15]. A developer's ability to clearly articulate a repeatable, logical deployment process is a strong indicator of the project's overall stability. If the developer cannot provide a clear, step-by-step process, or if the process is overly complex & manual (**First I FTP these three files, then I go into the database & manually copy this one table...**), it reveals a massive operational risk. This undocumented, memory-based process is fragile & highly susceptible to human error. It signals that the new owner's first priority must be to stabilize & document this workflow to prevent a catastrophic failure during the first critical security update.
  - **Please provide the exact, step-by-step process for deploying changes from development to production. For example: '1. Pull latest changes to the staging branch. 2. Test functionality on the staging site. 3. Take a manual backup of the production site. 4. Push changes from the staging branch to the production branch. 5. Clear all server & plugin caches.' Is this process documented?**
- > This is a notoriously difficult aspect of WordPress development. While files can be easily managed w/Git, synchronizing database changes is more complex. The developer should be able to explain their solution, whether it involves a specialized plugin (like WP Migrate DB Pro) or a carefully documented manual process.
  - **How are database changes (e.g., from a plugin settings update or a change made in the theme customizer) migrated from the staging environment to the production site?**

### <a href="#performance-caching-layers">#</a> D. Performance & Caching Layers

Website speed is critical for user experience & search engine optimization (SEO). Caching is the primary technique used to improve performance.

- **What caching layers are in place? Please specify any caching plugins (e.g., WP Rocket, W3 Total Cache), server-side caching technologies (e.g., Varnish, Redis, Memcached), or CDN-level caching.**
 A modern WordPress site often has multiple layers of caching[^5]. Understanding each layer is essential for troubleshooting issues where changes do not appear on the live site.
- **What is the specific procedure for clearing or purging all caches when a change is made but is not visible on the live site?**
 This is a common & frustrating problem. The developer should provide a clear, step-by-step guide for purging every layer of cache, from the browser cache to the plugin cache, server cache, & CDN cache.
- **Is a Content Delivery Network (CDN) like Cloudflare or StackPath being used? If so, are there any specific page rules, firewall settings, or other configurations that I should be aware of?**
 A CDN improves performance & security by distributing the site's assets across a global network of servers. However, misconfigured CDN settings can cause a wide range of issues, from incorrect content being displayed to the site being completely inaccessible. Access to & knowledge of the CDN configuration is essential.

### <a href="#ssl-certificate">#</a> E. SSL Certificate

An SSL certificate encrypts the connection between the user's browser & the web server, which is essential for security & is a requirement for modern websites.

- **Who is the provider of the SSL certificate (e.g., Let's Encrypt, a premium commercial provider)? Is it configured to renew automatically?**
 Most hosts now provide free SSL certificates from Let's Encrypt that renew automatically[^7]. However, it is crucial to confirm this. An expired SSL certificate will cause browsers to display prominent security warnings to visitors, effectively killing traffic to the site until it is fixed.

---

[`🔼 RETURN TO TOP`](#top)

## <a href="#part-5">#</a> Part V: Operations, Security, & Maintenance Protocols

A website is not a static, one-time creation; it is a living system that requires continuous care & attention to remain healthy, secure, & functional. This section covers the ongoing operational procedures that form the core of a responsible website management strategy. Neglecting these protocols is a leading cause of website hacks, data loss, & performance degradation.

### <a href="#backup-disaster-recovery-strategy">#</a> A. Backup & Disaster Recovery Strategy

A robust backup strategy is the single most important defense against a wide range of catastrophic events, including server failure, hacking, or a critical error during an update.

- **What is the complete backup strategy? Please specify the tools used (e.g., hosting provider's built-in backup, a WordPress plugin like Duplicator or UpdraftPlus), the frequency of the backups (e.g., daily, weekly), & what, specifically, is included (e.g., full files & database).**
 A comprehensive answer to this question should detail a multi-faceted strategy[^4]. Relying on a single backup method is risky. A good strategy might involve daily automated backups from the hosting provider combined w/a separate, plugin-based backup solution.
- **Where are the backups stored? Is at least one copy stored in a secure, off-site location (e.g., Amazon S3, Dropbox, Google Drive)?**
 This is a critical detail. Backups stored on the same server as the website are of limited use if the entire server is compromised or fails[^4]. A fundamental principle of disaster recovery is to maintain at least one copy of the backups in a geographically separate, secure, off-site location.
- **Most importantly: Can you walk me through the documented procedure for a full site restoration from a backup? When was the last time a restoration was successfully tested?**
 This question cuts to the heart of operational readiness. An untested backup is not a reliable strategy; it is merely a hope. Many organizations have discovered, to their horror, that their backups were corrupted or incomplete only when they desperately needed them. A mature operational plan focuses not just on the act of creating backups, but on the proven ability to restore service from them. The developer should be able to provide a clear, documented procedure for restoration. The question **When was the last time this was tested?** separates a developer who has simply installed a backup plugin from one who has implemented a genuine, business-saving disaster recovery plan. The absence of a tested restoration procedure should be considered a critical risk that must be remediated immediately.

### <a href="#security-posture-tooling">#</a> B. Security Posture & Tooling

Given WordPress's popularity, it is a constant target for malicious actors. A proactive security posture is not optional; it is a fundamental requirement of website ownership.

- **What security plugins (e.g., Wordfence, Sucuri, iThemes Security) are installed? What are their key configurations, such as login attempt limits, file change detection, & firewall rules?**
 Security plugins provide essential hardening & monitoring capabilities[^4]. The new owner must understand which tools are in place & how they have been configured to protect the site. For example, knowing the login attempt limit is crucial for preventing brute-force attacks.
- **What are the established policies for user roles & permissions? Is the Principle of Least Privilege (PoLP) enforced?**
 The Principle of Least Privilege is a foundational security concept which dictates that users should only be granted the minimum level of access necessary to perform their job functions[^4]. For example, a content writer does not need the ability to install plugins or change theme settings. Enforcing PoLP dramatically reduces the site's attack surface & limits the potential damage that can be caused by a compromised user account.
- **Have there been any security breaches, malware infections, or hacking attempts in the past? If so, how were they resolved, & what specific measures were put in place to prevent a recurrence?**
 Understanding the site's security history can reveal persistent vulnerabilities. If the site has been compromised before, the new owner must know how the breach occurred, how the site was cleaned, & what steps were taken to close the security hole.

### <a href="#update-maintenance-cadence">#</a> C. Update & Maintenance Cadence

Outdated software is the leading cause of WordPress security vulnerabilities. A regular, disciplined update process is therefore a critical security function.

- **What is the established schedule & process for updating the WordPress core, themes, & plugins?**
 There should be a regular, predictable cadence for performing updates (e.g., weekly or bi-weekly)[^15]. Updates should not be applied haphazardly as they become available. A disciplined process ensures that updates are managed in a controlled manner.
- **How are updates tested before being applied to the live site?**
 This question links directly back to the staging & deployment workflow discussed in Part IV. The only safe way to apply updates is to first test them on a staging site to ensure they do not cause conflicts or break functionality[^12]. Applying updates directly to a live production site without testing is a high-risk gamble.

### <a href="#monitoring-analytics">#</a> D. Monitoring & Analytics

It is impossible to manage what is not measured. Monitoring tools provide essential visibility into the site's health, performance, & user behavior.

- **Are there any tools in place for uptime monitoring? Who receives alerts if the site goes down?**
 Uptime monitoring services (e.g., Uptime Robot, Pingdom) constantly check if a website is online & send immediate alerts if it becomes unavailable[^20]. This allows the owner to respond to downtime quickly, often before clients or customers notice.
- **How is website performance monitored? Are there any analytics or logging tools configured to track errors or performance degradation over time?**
 Beyond simple uptime, tools can be used to monitor server response times, page load speeds, & application errors. Proactive performance monitoring can help identify & fix issues before they significantly impact the user experience.
- **Please provide administrative access to the site's Google Analytics & Google Search Console profiles.**
 These two tools are the industry standard for understanding website traffic & search performance. Google Analytics provides detailed insights into user behavior, while Google Search Console offers crucial data on how the site is performing in Google search results, including any indexing errors or manual penalties. Access to both is non-negotiable for any serious website owner.

---

[`🔼 RETURN TO TOP`](#top)

## <a href="#part-6">#</a> Part VI: The Handover Execution & Post-Transition Support

The final phase of the handover process deals w/the logistics of the knowledge transfer itself and, crucially, establishes clear & unambiguous expectations for the relationship between the new owner & the departing developer moving forward. This is where the process is formalized & the transition of responsibility is officially completed.

### <a href="#documentation-training">#</a> A. Documentation & Training

Comprehensive documentation & training are the bridge that allows the new owner to confidently take control of the website. They are the tangible outputs of the knowledge transfer process.

- **What project documentation is available (e.g., technical specifications, user manuals, design style guides), & where can it be found?**
  The existence & quality of documentation are strong indicators of a project's overall health & the developer's professionalism[^1]. A well-documented project is significantly easier & less costly to maintain. The absence of any documentation is a major red flag, suggesting that all critical knowledge resides solely in the head of the departing developer.
- **Are you available to conduct a live training session for our team? Could you provide recorded video walkthroughs for common tasks, such as adding a new blog post, updating an e-commerce product, or managing contact form entries?**
  While written documentation is essential, live or recorded training can be far more effective for demonstrating workflows & user interfaces[^2]. Video walkthroughs are particularly valuable as they create a reusable training asset that can be used to onboard future team members, reducing long-term dependency on any single individual.

### <a href="#final-transfer-checklist">#</a> B. The Final Transfer Checklist

This is the culminating event of the handover process, where control is officially & verifiably transferred. It should be conducted methodically to ensure no steps are missed.

- **Agree on a specific date & time for the final handover:** _______,
  Scheduling a formal handover meeting ensures that both parties are available & focused on completing the transition.
- **Use the Master Credentials & Services Inventory table as a final checklist:** [Go to Checklist](#checklist)
  During the handover meeting, the new owner should systematically go through the inventory table created in [Part II](#part-ii-the-keys-to-the-kingdom-access-credentials-and-third-party-services).
- **The new owner logs into every single service to confirm access.**
  This step verifies that all credentials provided are correct & functional.
- **The new owner changes all passwords & enables Two-Factor Authentication (2FA).**
  This is the critical step of securing all accounts under the new owner's exclusive control.
- **The new owner confirms that the previous developer's user accounts have been removed from all systems.**
  This final de-provisioning step officially completes the transfer of control & mitigates the risk of unauthorized future access.[^3]

### <a href="#post-handover-support">#</a> C. Defining Post-Handover Support

It is unrealistic to expect a perfectly flawless transition. Minor issues or questions will inevitably arise. Defining the terms of post-handover support in advance is crucial for managing expectations & preventing future disputes.

- **What is the specific duration & scope of the post-handover support period? (e.g. `"14 days for critical"`, `"site-breaking bug fixes only"`).**
  The terms of this support window should be explicitly defined in writing[^1]. It should be clear that this period is for addressing unforeseen issues related to the existing state of the site, not for new feature development or general consulting.
- **What are the designated communication channels (e.g. `"a specific email address"`) & the expected response times for support requests during this period?**
  Establishing clear communication protocols prevents confusion & frustration[^13]. Knowing whether to expect a response within a few hours or a few business days helps to manage expectations appropriately.
- **What are your standard hourly rates for any work that may be requested after the formal support period ends?**
  It is wise to establish the cost of potential future work now, even if none is anticipated[^7]. Having a rate sheet in writing prevents disagreements over pricing should the new owner wish to re-engage the developer for new projects or more extensive support down the line.

### <a href="#exit-interview">#</a> D. The Exit Interview: Uncovering the **Unknown Unknowns**

This final set of open-ended questions is designed to elicit the kind of nuanced, contextual information that is often missed in a standard checklist. This is an opportunity to tap into the departing developer's unique, ingrained knowledge of the project's quirks & subtleties.

- **From your expert perspective, what do you consider to be the most fragile or technically complex part of this website?** _Every project has a weak point or a piece of convoluted code that the developer knows to handle w/extreme care. This question encourages them to reveal it, allowing the new owner to be aware of the risk._
- **If you were given another week to work on this project, what is the first thing you would fix or improve?** _This question often uncovers the developer's own assessment of the project's technical debt.[^1] Their answer can provide a valuable starting point for the new owner's own improvement roadmap._
- **Are there any _quirks_, oddities, or manual workarounds that we should be aware of? For example, (e.g. `"To update the CEO's photo, you have to do this one weird thing in the media library"`, etc.)** _This is often the most valuable question of the entire handover. It is designed to capture the undocumented, informal knowledge that is essential for the smooth day-to-day operation of the site. These are the details that are never written down but can cause hours of frustration for a new team._
- **What were the biggest challenges you faced during the project? What were the most important lessons learned?** _This question provides insight into the project's history from a different angle.[^1] Understanding the past struggles—whether w/a particular plugin, a server configuration, or a third-party API—can help the new owner avoid repeating them in the future._

---

[`🔼 RETURN TO TOP`](#top)

## <a href="#conclusion">#</a> Conclusion

The successful handover of a WordPress project is a direct result of a diligent, systematic, & comprehensive process of inquiry. It is an exercise in proactive risk management, not an expression of mistrust. The exhaustive set of questions detailed in this guide is designed to form the backbone of this process, ensuring that the transfer of responsibility is built upon a foundation of clarity, security, & complete knowledge.

**The core principles underpinning a successful handover are threefold:**

- **Full & Unambiguous Ownership** - The new owner must secure complete legal & administrative control over every digital asset, from the domain name & source code to all associated third-party service accounts.
- **Complete System Knowledge** - The new owner must possess a deep understanding of the website's technical architecture, its operational dependencies, & the strategic goals it is designed to serve. This knowledge is the prerequisite for effective maintenance & future development.
- **Clear & Documented Processes** - The ongoing health of the website depends on robust, repeatable processes for security, backups, updates, & deployments. These processes must be clearly documented & tested.

> "By methodically pursuing the answers to these questions, the incoming owner transforms the handover from a moment of high risk into an opportunity to establish a stable & secure foundation for the future. This upfront investment of time & diligence is the most effective strategy for protecting the value of the digital asset, ensuring business continuity, & dramatically reducing the long-term costs & complexities of website ownership. The ultimate goal is to achieve a state of confident, informed, & truly independent control." &mdash;**[@dylarcher](https://github.com/dylarcher)**

### <a href="#sources">#</a> Sources

[^1]: Project handover templates & checklists for effective transitions: [&lt;https://project-management.com/the-project-handover-checklist&gt;](https://project-management.com/the-project-handover-checklist/)
[^2]: How to Create a Handover Document; free Templates & key elements. (`Scribe`): [&lt;https://scribehow.com/library/handover-document-template&gt;](https://scribehow.com/library/handover-document-template/)
[^3]: How to use an employee offboarding checklist. (`Revelo`): [&lt;https://www.revelo.com/blog/employee-offboarding-checklist-the-ultimate-guide&gt;](https://www.revelo.com/blog/employee-offboarding-checklist-the-ultimate-guide/)
[^4]: How to grant WordPress access to your developer (or, Team…) (`Servebolt`): [&lt;https://servebolt.com/articles/wordpress-developer-access&gt;](https://servebolt.com/articles/wordpress-developer-access/)
[^5]: WordPress handoffs&hellip; because, "figure it out" is not a client strategy. (`Delicious Brains`): [&lt;https://deliciousbrains.com/wordpress-handoffs-because-figure-it-out-is-not-a-client-strategy&gt;](https://deliciousbrains.com/wordpress-handoffs-because-figure-it-out-is-not-a-client-strategy/)
[^6]: Project handover checklist template; Your complete guide. (`Atlassian apps`): [&lt;https://www.resolution.de/post/project-handover-checklist-template&gt;](https://www.resolution.de/post/project-handover-checklist-template/)
[^7]: Know what to ask your web developer. (`Business Victoria`): [&lt;https://business.vic.gov.au/business-information/ecommerce/build-a-website/know-what-to-ask-your-web-developer&gt;](https://business.vic.gov.au/business-information/ecommerce/build-a-website/know-what-to-ask-your-web-developer)
[^8]: Checklist for final project hand-over from website&hellip. (`Capsquery`): [&lt;https://capsquery.com/8-checklists-for-final-project-hand-over-from-website-development-team&gt;](https://capsquery.com/8-checklists-for-final-project-hand-over-from-website-development-team/)
[^10]: Questions to ask your website designer before&hellip. (`Design Powers`): [&lt;https://designpowers.com/blog/25-questions-to-ask-your-website-designer-before-hiring&gt;](https://designpowers.com/blog/25-questions-to-ask-your-website-designer-before-hiring)
[^11]: **Handover documentation** - (`r/Wordpress` `Reddit`): [&lt;https://www.reddit.com/r/wordpress/comments/17mv4wk/handover_documentation&gt;](https://www.reddit.com/r/wordpress/comments/17mv4wk/handover_documentation/)
[^12]: What is your offboarding process for hosting/maintenance? (`r/Wordpress` `Reddit`): [&lt;https://www.reddit.com/r/wordpress/comments/1i07lam/what_is_your_offboarding_process_for&gt;](https://www.reddit.com/r/wordpress/comments/1i07lam/what_is_your_offboarding_process_for/)
[^13]: How To Successfully Hand off a Website To Your Clients. (`Elementor`): [&lt;https://elementor.com/blog/how-to-handover-website-client&gt;](https://elementor.com/blog/how-to-handover-website-client/)
[^15]: Checklist Pointer for Oversee/Senior Dev. (`Axioned Handbook`): [&lt;https://handbook.axioned.com/processes/guidelines/wordpress&gt;](https://handbook.axioned.com/processes/guidelines/wordpress/)
[^16]: Questions you should ask a web host before purchasing WordPress hosting w/theme: [&lt;https://pressidium.com/blog/eight-questions-you-should-ask-a-web-host-before-purchasing-wordpress-hosting-with-them&gt;](https://pressidium.com/blog/eight-questions-you-should-ask-a-web-host-before-purchasing-wordpress-hosting-with-them/)
[^17]: Top WordPress Hosting Questions Answered. (`Crocoblock`): [&lt;https://crocoblock.com/blog/wordpress-hosting-questions-answers&gt;](https://crocoblock.com/blog/wordpress-hosting-questions-answers/)
[^18]: **Managed WordPress Hosting** - _Is It Worth It?_ Here's how to decide: [&lt;https://wordpress.com/blog/2025/04/28/managed-wordpress-hosting&gt;](https://wordpress.com/blog/2025/04/28/managed-wordpress-hosting/)
[^20]: Common questions on WordPress enterprise hosting everyone should ask before upgrading. (`Nestify`): [&lt;https://nestify.io/blog/wordpress-enterprise-hosting&gt;](https://nestify.io/blog/wordpress-enterprise-hosting/)
