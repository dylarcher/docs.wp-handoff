# The Definitive WordPress Handover Protocol: A Comprehensive Due Diligence Questionnaire

**Table of Contents**

- [Introduction](#intro)
- [Part I: Strategic & Commercial Foundation](#part-1)
  - [A. Project Purpose & History](#project-purpose-history)
  - [B. Stakeholder & Audience Landscape](#stakeholder-audience-landscape)
  - [C. Commercial & Legal Framework](#commercial-legal-framework)
- [Part II: The Keys to the Kingdom: Access, Credentials, & Third-Party Services](#part-2)
  - [A. Core Platform Credentials](#core-platform-credentials)
  - [B. Infrastructure & Development Access](#infrastructure-development-access)
  - [C. Integrated Services & APIs](#integrated-services-apis)
  - [D. The Secure Transfer Process](#the-secure-transfer-process)
  - [Master Credentials & Services Inventory](#master-credentials-services-inventory)
- [Part III: Deconstructing the Technical Architecture](#part-3)
  - [A. The Code Repository & Version Control](#the-code-repository-version-control)
  - [B. Theme & Parent/Child Theme Structure](#theme-parent-child-theme-structure)
  - [C. Plugin Ecosystem Audit](#plugin-ecosystem-audit)
  - [D. Custom Code & Development Practices](#custom-code-development-practices)
  - [E. Database & Content Structure](#database-content-structure)
  - [Plugin & Theme Audit](#checklist)
- [Part IV: The Hosting Environment & Deployment Pipeline](#part-4)
  - [A. Server & Hosting Plan Details](#server-hosting-plan-details)
  - [B. Server Configuration & Dependencies](#server-configuration-dependencies)
  - [C. The Staging & Production Workflow](#staging-production-workflow)
  - [D. Performance & Caching Layers](#performance-caching-layers)
  - [E. SSL Certificate](#ssl-certificate)
- [Part V: Operations, Security, & Maintenance Protocols](#part-5)
  - [A. Backup & Disaster Recovery Strategy](#backup-disaster-recovery-strategy)
  - [B. Security Posture & Tooling](#security-posture-tooling)
  - [C. Update & Maintenance Cadence](#update-maintenance-cadence)
  - [D. Monitoring & Analytics](#monitoring-analytics)
- [Part VI: The Handover Execution & Post-Transition Support](#part-6)
  - [A. Documentation & Training](#documentation-training)
  - [B. The Final Transfer Checklist](#final-transfer-checklist)
  - [C. Defining Post-Handover Support](#post-handover-support)
  - [D. The Exit Interview: Uncovering the **Unknown Unknowns**](#exit-interview)
- [Conclusion](#conclusion)
- [Sources](#sources)

The handover of a WordPress project is a critical inflection point in the lifecycle of a digital asset. It is frequently misconstrued as a simple, transactional event involving the exchange of files and passwords. This perspective is dangerously incomplete. A successful handover is not an event but a comprehensive process of knowledge transfer, moving far beyond the delivery of technical components to encompass the full strategic, legal, and operational context of the website[^1]. The ultimate objective is to de-risk the transition by eliminating dependency on the departing developer, thereby empowering the new owner with complete and unencumbered autonomy over their digital property.

## <a href="#intro">#</a> Introduction

The stakes of a poorly executed handover are exceptionally high. An incomplete transfer can precipitate a cascade of negative consequences that manifest long after the original developer has departed. These risks include severe security vulnerabilities stemming from lingering, unauthorized access to critical systems[^3]; operational downtime caused by unknown dependencies or undocumented, fragile workflows[^5]; significant legal liabilities arising from ambiguous ownership of intellectual property or non-compliance with data privacy regulations[^6]; and escalating future costs as the new team grapples with undocumented **technical debt** that is difficult and expensive to remediate[^8]. Many of these issues can be traced back to a failure to ask the right questions at the right time.

This guide provides a structured, exhaustive set of questions designed to serve as a definitive due diligence protocol for any WordPress project handover. It is engineered to be a practical tool, enabling the incoming owner or team to proactively identify, assess, and mitigate the myriad risks inherent in the transition process. By systematically addressing each area—from high-level strategy to the most granular technical detail—the new owner can ensure a truly complete and seamless transfer of control, establishing a firm foundation for the future management, maintenance, and growth of the website.

[`🔼 RETURN TO TOP`](#top)

## <a href="#part-1">#</a> Part I: Strategic & Commercial Foundation

Before any technical examination of the website can be meaningful, it is imperative to establish a deep understanding of its business context. The technical architecture, features, and code are merely instruments designed to serve a strategic purpose. Their quality and appropriateness can only be judged against the business goals they were intended to achieve. This section provides the questions necessary to uncover the **why** behind the website, clarifying its purpose, history, stakeholders, and the legal framework that governs it.

### <a href="#project-purpose-history">#</a> A. Project Purpose & History

Understanding the original intent and historical evolution of a project is fundamental. It provides the context for all subsequent technical decisions and can reveal architectural layers or features that may no longer align with the current business strategy. This historical perspective is a map to understanding the site's current state and its potential hidden complexities.

- [ ] **What was the original business problem this website was built to solve? What were the primary goals and objectives defined at the project's inception?**  
  This foundational question seeks to establish the core rationale for the website's existence[^2]. A clear answer, such as **to generate qualified leads for our consulting services** or **to sell handmade goods directly to consumers**, provides a lens through which all features and design choices can be evaluated. A vague or non-existent answer may indicate a lack of strategic direction from the outset, which can often translate into a disjointed and ineffective website.
- [ ] **Who was the target audience defined at the project's outset, and has that audience evolved over time?**  
  A website's design, content, and functionality should be tailored to its intended users[^5]. Understanding the defined audience helps assess the appropriateness of the user experience (UX) and user interface (UI). Furthermore, inquiring about the evolution of this audience can highlight areas where the site may need to be adapted to meet new user needs or demographic shifts.
- [ ] **Can you provide a brief history of the project, including key milestones, major feature additions, or significant strategic pivots?**  
  This question is not merely about creating a timeline; it is a powerful diagnostic tool for uncovering technical debt[^1]. A project's history is often a story of its compromises. For example, a website that began as a simple **brochure** site and later had e-commerce functionality **bolted on** may suffer from significant architectural weaknesses. The theme may not be optimized for online sales, or the chosen e-commerce plugin might be poorly integrated, leading to performance issues and maintenance nightmares. Understanding these historical pivots allows the new owner to probe deeper into the implementation of major features and anticipate areas of fragility that are not immediately apparent from a surface-level review.
- [ ] **What were the key performance indicators (KPIs) used to measure the website's success?**  
  Knowing the metrics that matter—such as lead conversion rates, average order value, or user engagement time—clarifies what aspects of the site are considered most valuable[^2]. This information is crucial for prioritizing future development efforts and ensuring that any changes made do not negatively impact the site's primary commercial or strategic functions.

### <a href="#stakeholder-audience-landscape">#</a> B. Stakeholder & Audience Landscape

A website does not exist in a vacuum. It serves and is managed by a network of individuals, each with their own set of expectations and responsibilities. Identifying these stakeholders is essential for establishing clear lines of communication and understanding the project's internal political landscape.

- [ ] **Who are the key internal and external stakeholders involved with the website? Who has the final authority for approving changes?**  
  This question aims to create a definitive map of influence and responsibility[^1]. The answer should identify the project owner, marketing team members, content editors, and any other individuals who have a vested interest in the site's operation. Crucially, it must clarify the approval workflow, which will prevent future delays and conflicts when changes need to be implemented.
- [ ] **Which stakeholders were involved in the original 'Discovery' or research phase of the project?**  
  The initial research or **Discovery** phase is where the foundational requirements and strategies for a project are established[^10]. Identifying the participants of this phase provides a direct line to the sources of the original project vision. If questions arise later about why a particular feature was built in a certain way, these are the individuals who will likely hold the answer.

### <a href="#commercial-legal-framework">#</a> C. Commercial & Legal Framework

The handover process involves the transfer of a valuable business asset, and with it comes a host of commercial and legal responsibilities. Failing to clarify these details can lead to severe financial and legal repercussions, including loss of ownership, unexpected costs, and data privacy violations.

- [ ] **Can you confirm in writing that upon final payment, our organization will have 100% ownership of the website, its design, all custom-developed code, and all content created specifically for the project?**  
  This is arguably one of the most critical questions in the entire handover process. It directly addresses the fundamental issue of asset ownership[^7]. Ambiguity in contracts or verbal agreements has led to numerous disputes where developers claim ownership of the work, effectively holding the client's website hostage[^11]. A clear, written confirmation of a complete transfer of intellectual property rights is non-negotiable.
- [ ] **Are there any third-party or premium software licenses (for themes, plugins) that need to be transferred or repurchased? Please provide a comprehensive list of all such software, including license keys, original purchase dates, renewal dates, and annual costs.**  
  Modern WordPress sites are often built upon a foundation of premium themes and plugins. These components require active licenses to receive crucial security updates and technical support[^5]. If these licenses are registered to the departing developer, they may expire without the new owner's knowledge, leaving the site vulnerable to security exploits or causing critical features to cease functioning. A complete inventory of these licenses is essential for both security and financial planning.
- [ ] **Are there any ongoing service level agreements (SLAs), hosting contracts, or other contractual obligations with your company or external third parties that we will be inheriting?**  
  This question aims to uncover any hidden or recurring financial commitments associated with the website[^1]. The new owner must be aware of all contracts they are assuming, whether for specialized hosting, maintenance retainers, or other third-party services. This prevents unexpected invoices and ensures continuity of essential services.
- [ ] **What data privacy agreements or policies are in place to comply with regulations such as GDPR or CCPA? Where is user data stored, and what measures are in place to protect it?**  
  In the modern regulatory environment, data privacy is a significant area of legal liability[^6]. The new owner must understand how the website collects, stores, and manages personally identifiable information (PII). This includes data from contact forms, e-commerce transactions, and user registrations. The developer should be able to point to the relevant privacy policy pages and explain the technical safeguards that have been implemented to ensure compliance.

[`🔼 RETURN TO TOP`](#top)

## <a href="#part-2">#</a> Part II: The Keys to the Kingdom: Access, Credentials, & Third-Party Services

This section constitutes a non-negotiable inventory of all access points required to control the website and its surrounding ecosystem. The primary goal is to achieve full, exclusive administrative control over every component. A handover cannot be considered complete until every credential has been securely transferred and the previous developer's access has been systematically and verifiably revoked from every platform. Failure to do so represents a critical and ongoing security risk[^3].

### <a href="#core-platform-credentials">#</a> A. Core Platform Credentials

These are the fundamental access points for managing the website's content, hosting environment, and domain name. Without these, the new owner is effectively locked out of their own property.

- [ ] **Please provide credentials for a new, unique Administrator-level user for the WordPress dashboard.**  
  It is a critical best practice to never take over an existing user account[^8]. A new, dedicated administrator account should be created for the new owner. This ensures a clean audit trail and prevents any ambiguity about who performed which actions. Once the new owner has confirmed their access, all other administrator accounts, including the one used by the departing developer, should be demoted or deleted.
- [ ] **What are the login details for the website's hosting control panel (e.g., cPanel, Plesk, or a custom provider dashboard)?**  
  The hosting control panel is the gateway to the server environment. It allows for the management of files, databases, email accounts, and other server-level configurations[^8]. Access to this panel is essential for troubleshooting, performing backups, and managing the underlying infrastructure of the website.
- [ ] **What are the login details for the domain registrar (e.g., GoDaddy, Namecheap) where the site's domain name is managed?**  
  Control over the domain registrar account is paramount[^13]. This account governs the ownership of the domain name itself, as well as the DNS settings that direct traffic to the web server. Losing control of this account can result in the loss of the domain name, a catastrophic event for any business. The new owner must ensure that the account is transferred into their name and that they control the billing information for renewals.

### <a href="#infrastructure-development-access">#</a> B. Infrastructure & Development Access

For more advanced management, maintenance, and development, direct access to the server's file system and database is often required.

- [ ] **Please provide SFTP (Secure File Transfer Protocol) or SSH (Secure Shell) credentials for direct file access to the server.**  
  SFTP/SSH access allows for the direct manipulation of WordPress core files, themes, and plugins[^4]. This level of access is necessary for manual updates, troubleshooting complex issues, and managing file permissions. Each user who requires this access should have their own unique credentials.
- [ ] **What are the credentials for direct database access, including the Database Name, Username, Password, and Hostname?**  
  The WordPress database is the heart of the website, storing all content, settings, and user information. Direct access via a tool like phpMyAdmin (often available through the hosting control panel) is sometimes necessary for complex data migrations, repairs, or manual cleanup[^8]. These credentials should be treated with the utmost security.

### <a href="#integrated-services-apis">#</a> C. Integrated Services & APIs

Modern websites are rarely monolithic; they are ecosystems of interconnected services. Each of these services represents an access point that must be controlled.

- [ ] **Please provide a comprehensive list of all third-party services integrated with the site. This must include, but is not limited to: Payment Gateways (e.g., Stripe, PayPal), Content Delivery Networks (CDNs) like Cloudflare, Email Marketing Platforms (e.g., Mailchimp, ConvertKit), CRM systems, Analytics platforms (e.g., Google Analytics, Google Tag Manager), and any other services connected via an API key.**  
  This question forces a thorough inventory of the entire digital ecosystem[^5]. Many critical site functions, such as payment processing or email list sign-ups, depend on these external services. Without a complete list, the new owner may be unaware of a dependency until it fails.
- [ ] **For each service identified, what are the login credentials or API keys, and what is the process for transferring ownership of these accounts to us?**  
  It is not enough to simply have the login details; legal and administrative ownership of these third-party accounts must be transferred[^5]. This often involves the departing developer adding the new owner as an administrator, who then removes the developer's access. For services using API keys, these keys should be regenerated after the handover to invalidate the old ones.

### <a href="#the-secure-transfer-process">#</a> D. The Secure Transfer Process

The method by which credentials are transferred is as important as the credentials themselves. Insecure practices can expose sensitive information and undermine the entire handover process.

- [ ] **ACTION ITEM: Insist on Secure Credential Sharing.**  
  Under no circumstances should passwords or API keys be sent in plain text via email, as this is a major security vulnerability[^13]. The new owner should insist on the use of a secure sharing method, such as a one-time, self-destructing note service (e.g., Privnote) or, preferably, a shared vault within a reputable password manager (e.g., 1Password, Bitwarden).
- [ ] **ACTION ITEM: Immediate Credential Rotation & 2FA Activation.**  
  Upon receiving all credentials, the new owner's first action should be to log in to every single service, change the password to a new, strong, and unique one, and enable two-factor authentication (2FA) wherever possible. This immediately secures the accounts under the new owner's control.
- [ ] **ACTION ITEM: Systematic Revocation of Old Access.**  
  The final and most crucial step of the access transfer is to systematically remove the previous developer's user accounts from every platform: WordPress, hosting, domain registrar, CDN, and all other third-party services[^3]. This step should be performed methodically, using the inventory created as a checklist. The handover is not complete until this de-provisioning process is finished.

### <a href="#master-credentials-services-inventory">#</a> Master Credentials & Services Inventory

To facilitate this critical process, the use of a centralized inventory document is strongly recommended. The following table provides a template for creating a single source of truth for all access points, which serves as both an inventory and a dynamic checklist for the transfer of ownership.

| Service/Platform | Purpose | Login URL | Username / Account Email | Password Transfer Method | API Key (if applicable) | License/Subscription Cost | Renewal Date | Ownership Transfer Status |
|------------------|-----------------|--------------------------------------------------|-------------------------------------------------------------|------------------------|-----------------------|-------------------------|------------|-------------------------|
| WordPress Admin | Content Management | <https://yourdomain.com/wp-admin> | `new_admin_user` | Shared via Bitwarden | -- | -- | -- | [x] Completed |
| GoDaddy | Domain Registrar | <https://dcc.godaddy.com/> | [owner@yourcompany.com](mailto:owner@yourcompany.com) | To be reset by new owner | -- | $19.99/year | `2025-10-15` | Completed |
| SiteGround Hosting | Web Hosting | <https://login.siteground.com/> | [owner@yourcompany.com](mailto:owner@yourcompany.com) | To be reset by new owner | -- | $299/year | `2025-09-01` | Completed |
| Stripe | Payment Processing | <https://dashboard.stripe.com/> | [finance@yourcompany.com](mailto:finance@yourcompany.com) | Existing account | pk_live_... | Transaction fees | -- | Completed |
| Cloudflare | CDN / Firewall | <https://dash.cloudflare.com/> | [tech@yourcompany.com](mailto:tech@yourcompany.com) | To be reset by new owner | [Global API Key] | $20/month | Monthly | Completed |
| Mailchimp | Email Marketing | <https://login.mailchimp.com/> | [marketing@yourcompany.com](mailto:marketing@yourcompany.com) | Existing account | [API Key] | $50/month | Monthly | Completed |
| Advanced Custom Fields PRO | Plugin License | <https://www.advancedcustomfields.com/my-account/> | [developer@oldcompany.com](mailto:developer@oldcompany.com) | Transfer license | [License Key] | $49/year | `2025-07-22` | _Pending_ |

This structured approach transforms a potentially chaotic and insecure exchange into a systematic and auditable process. It forces a complete inventory, preventing omissions of forgotten but critical services like a transactional email API. By including columns for cost and renewal dates, the table evolves from a simple access log into a vital financial and operational planning tool, preventing unexpected service disruptions due to non-payment[^7]. The **Ownership Transfer Status** column acts as a progress tracker, providing a clear visual indicator of what has been completed and what remains, ensuring that the critical final step of revoking the old developer's access is never overlooked[^4].

[`🔼 RETURN TO TOP`](#top)

## <a href="#part-3">#</a> Part III: Deconstructing the Technical Architecture

Understanding how a website was built is a prerequisite for being able to effectively maintain, troubleshoot, and extend it. This section focuses on creating a comprehensive **blueprint** of the site's technical construction. The questions are designed to uncover the development practices, tools, and structural decisions that define the website's functionality and, by extension, its future maintainability.

### <a href="#the-code-repository-version-control">#</a> A. The Code Repository & Version Control

The use of a version control system (VCS) like Git is a hallmark of professional web development. It provides a complete history of changes, facilitates collaboration, and enables safe deployment and rollback procedures.

- [ ] **Is the website's code managed in a version control system like Git? If so, please provide access to the repository (e.g., on GitHub, Bitbucket, or GitLab).**  
  The answer to this question is a primary indicator of the developer's professionalism. If the code is managed in a repository, it suggests a structured and disciplined workflow[^8]. If the answer is _no_, or if the developer is unfamiliar with the concept, it is a major red flag. It implies that changes were likely made directly on the live server via FTP, a practice that is highly prone to error and offers no way to track changes or revert mistakes.
- [ ] **What is the branching strategy used in the repository (e.g., GitFlow, feature branches)? Which branch represents the code currently running on the live production site?**  
  Understanding the branching strategy is key to safely contributing new code. A common practice is to have a main or master branch that reflects the live site, a develop branch for integrating new features, and separate feature branches for individual tasks. Knowing this structure prevents accidental deployments of unfinished work to the production environment.
- [ ] **Can you confirm that the repository contains the complete and unabridged history of the project's development?**  
  A repository with a shallow or very recent commit history may indicate that version control was not used consistently throughout the project's life. A complete history is an invaluable diagnostic tool, allowing the new owner to see when and why specific changes were made.

### <a href="#theme-parent-child-theme-structure">#</a> B. Theme & Parent/Child Theme Structure

The WordPress theme controls the entire visual presentation of the site. The way it has been structured and customized has profound implications for future updates and maintenance.

- [ ] **What theme is the site built on? Is it a pre-built commercial theme from a marketplace, or is it a fully custom theme built from scratch?**  
  This question establishes the foundation of the site's design[^10]. If it is a commercial theme, the new owner will need to know where to find its documentation and support channels. If it is a custom theme, all documentation must come from the departing developer.
- [ ] **If it's a commercial theme, is a child theme being used for all customizations? Can you provide explicit confirmation that no modifications have been made directly to the parent theme's files?**  
  This is a critically important technical question. The WordPress best practice for customizing a commercial theme is to use a child theme[^5]. A child theme inherits all the functionality and styling of the parent theme but allows customizations to be stored in separate files. This structure ensures that when the parent theme is updated (for example, to patch a security vulnerability), the custom modifications are not overwritten and lost. If the developer has edited the parent theme's files directly, the site becomes **un-updateable**, posing a massive long-term security and maintenance risk.
- [ ] **Where are the theme's original purchase files and official documentation located?**  
  For any commercial theme, having access to the original .zip file and the official documentation is essential for troubleshooting and understanding its built-in features and options.

### <a href="#plugin-ecosystem-audit">#</a> C. Plugin Ecosystem Audit

Plugins extend the core functionality of WordPress, but they also add complexity and potential points of failure. A thorough audit of the plugin stack is essential for assessing the site's health and security.

- [ ] **Please provide a complete list of all installed plugins. For each plugin, can you briefly explain its purpose and the rationale for why it was chosen over alternatives?**  
  This question forces a justification for each component of the site's software stack[^5]. It helps identify plugins that may be redundant, unnecessary, or not the best tool for the job. A site with an excessive number of plugins can suffer from poor performance and an increased attack surface.
- [ ] **Which of these plugins are premium (paid) versions? Please provide the associated license keys and account information required to receive future updates and technical support.**  
  As with premium themes, premium plugins require active licenses for updates[^12]. An expired license can leave a plugin vulnerable to known exploits. This information should be recorded in the Master Credentials & Services Inventory.
- [ ] **Are there any custom-built plugins developed specifically for this site? If so, where is their source code managed, and is there documentation for their functionality?**  
  A custom plugin represents a piece of bespoke software that the new owner will be responsible for maintaining[^11]. It is crucial to have access to its source code (ideally in the same Git repository as the theme) and comprehensive documentation explaining what it does and how it works.
- [ ] **Are there any known conflicts between plugins in the current stack, or are there any plugins known to cause performance issues?**  
  This question seeks to uncover latent problems that may not be immediately obvious. An experienced developer will often be aware of subtle conflicts or performance bottlenecks caused by specific combinations of plugins.
