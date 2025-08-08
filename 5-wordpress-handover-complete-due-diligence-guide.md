# WordPress Project Handoff: Complete Due Diligence Guide

A successful WordPress project handover is not just about sharing files and passwords—it's a comprehensive process of transferring knowledge, responsibility, and control. This guide provides a structured approach to ensure a seamless transition while minimizing risks and establishing a solid foundation for future management.

## Table of Contents

1. [Introduction](#introduction)
2. [Project Overview & Strategic Foundation](#1-project-overview--strategic-foundation)
3. [Stakeholders & Roles](#2-stakeholders--roles)
4. [Ownership & Legal Framework](#3-ownership--legal-framework)
5. [Domain & DNS Management](#4-domain--dns-management)
6. [Hosting & Server Infrastructure](#5-hosting--server-infrastructure)
7. [Database Access & Structure](#6-database-access--structure)
8. [WordPress Access & User Management](#7-wordpress-access--user-management)
9. [Server Access (FTP/SFTP/SSH)](#8-server-access-ftpsftpssh)
10. [Email Configuration](#9-email-configuration)
11. [Technical Architecture: Themes, Plugins & Custom Code](#10-technical-architecture-themes-plugins--custom-code)
12. [Third-Party Services & Integrations](#11-third-party-services--integrations)
13. [Backup & Disaster Recovery](#12-backup--disaster-recovery)
14. [Security Protocols](#13-security-protocols)
15. [Performance & Caching](#14-performance--caching)
16. [Analytics & SEO](#15-analytics--seo)
17. [Development Environments & Deployment](#16-development-environments--deployment)
18. [Documentation & Training](#17-documentation--training)
19. [Maintenance & Monitoring](#18-maintenance--monitoring)
20. [Final Handover Process](#19-final-handover-process)
21. [Exit Interview](#20-exit-interview)
22. [Inventory Templates](#21-inventory-templates)

---

## Introduction

The stakes of a poorly executed handover are exceptionally high. An incomplete transfer can lead to:

- **Security vulnerabilities** from lingering unauthorized access
- **Operational downtime** caused by unknown dependencies
- **Legal liabilities** from ambiguous ownership or privacy non-compliance
- **Escalating costs** due to undocumented technical debt

This guide provides a systematic approach to identify, assess, and mitigate these risks through comprehensive due diligence.

---

## 1. Project Overview & Strategic Foundation

Understanding the business context is essential before any technical examination can be meaningful.

### Core Purpose & History

- **What was the original business problem this website was built to solve?**
  - What were the primary goals and objectives at inception?
  - Has the purpose evolved over time?

- **Who was the target audience, and how has it changed?**
  - What user personas were defined originally?
  - Have there been demographic shifts or new user segments?

- **Can you provide a brief project history?**
  - Key milestones and major feature additions
  - Significant strategic pivots or architectural changes
  - Any major redesigns or platform migrations

- **What are the key performance indicators (KPIs) for success?**
  - Conversion rates, revenue metrics, engagement metrics
  - How is success currently measured?
  - What metrics matter most to stakeholders?

### Business Rules & Workflows

- **Are there unique business rules or workflows the site must follow?**
- **What compliance requirements exist (industry-specific, regulatory)?**
- **Are there any seasonal or cyclical business patterns that affect the site?**

---

## 2. Stakeholders & Roles

### Key Personnel

- **Who are the primary stakeholders and decision-makers?**
  - Project owner with final approval authority
  - Content managers and editors
  - Marketing team members
  - Technical administrators

- **What is the approval workflow for changes?**
  - Who needs to sign off on content changes?
  - Who approves technical updates or new features?
  - What is the escalation process for urgent issues?

- **Who participated in the original discovery/planning phase?**
  - These individuals hold institutional knowledge about requirements
  - They can clarify historical decisions and design rationale

### Post-Handover Management

- **Who will manage the website after handover?**
  - Content management responsibilities
  - Technical maintenance duties
  - Business decision authority

---

## 3. Ownership & Legal Framework

### Intellectual Property Rights

- **Can you confirm in writing that we will have 100% ownership of:**
  - The website and all its content
  - All custom-developed code and themes
  - All graphics, images, and design elements created for the project
  - All data and databases

- **Are there any exceptions or third-party components we don't own?**
  - Stock photos or licensed imagery
  - Premium themes or plugins
  - Third-party integrations or APIs

### Contractual Obligations

- **What ongoing contracts or agreements will we inherit?**
  - Hosting contracts and renewal dates
  - Premium software licenses and their terms
  - Service level agreements (SLAs)
  - Maintenance or support retainers

- **Are there any recurring subscription costs?**
  - List all services with costs and renewal dates
  - Include payment methods and billing contacts

### Privacy & Compliance

- **What data privacy policies are in place?**
  - GDPR, CCPA, or other regulatory compliance measures
  - Cookie consent mechanisms
  - Data retention and deletion policies

- **How is personally identifiable information (PII) handled?**
  - Data collection points (forms, user registration, e-commerce)
  - Storage location and security measures
  - Third-party data sharing agreements

---

## 4. Domain & DNS Management

### Domain Registration

- **What is the domain registrar and account details?**
  - Provider name (GoDaddy, Namecheap, etc.)
  - Account login credentials
  - Domain expiration and renewal date
  - Auto-renewal status and payment method

- **Are there any additional domains or subdomains?**
  - Redirects, staging sites, or development environments
  - Email-only domains or parked domains

### DNS Configuration

- **Who manages the DNS records?**
  - Is it the domain registrar or a separate DNS provider?
  - Are services like Cloudflare managing DNS?

- **What are the current DNS records?**
  - A records pointing to the web server
  - CNAME records for www and other subdomains
  - MX records for email routing
  - TXT records for domain verification or security

---

## 5. Hosting & Server Infrastructure

### Hosting Provider Details

- **Who is the hosting provider and what is the specific plan?**
  - Provider name and plan level
  - Server type (shared, VPS, dedicated, managed WordPress)
  - Geographic server location

- **What are the resource limits and specifications?**
  - Storage space and bandwidth limits
  - PHP memory limits and execution time
  - Database size restrictions
  - Number of allowed email accounts

### Server Configuration

- **What are the current software versions?**
  - PHP version and enabled extensions
  - MySQL/MariaDB version
  - Web server (Apache/Nginx) version and configuration

- **Are there any custom server configurations?**
  - Modified php.ini settings
  - Custom .htaccess rules
  - Special security or performance configurations

- **What control panel is used?**
  - cPanel, Plesk, or custom provider interface
  - Access credentials and feature limitations

### Security & Firewall

- **Is there a Web Application Firewall (WAF) in place?**
  - Server-level firewall (ModSecurity)
  - Provider-specific security features
  - Custom security rules or IP restrictions

---

## 6. Database Access & Structure

### Database Credentials

- **What are the database connection details?**
  - Database host, name, username, and password
  - Port number if non-standard
  - Database management tool access (phpMyAdmin)

### Database Structure

- **Are there any custom database tables?**
  - Tables beyond standard WordPress installation
  - Purpose and schema of custom tables
  - Any stored procedures or custom queries

- **What is the database backup and maintenance schedule?**
  - Automated backup frequency
  - Manual optimization procedures
  - Cleanup routines for logs or temporary data

---

## 7. WordPress Access & User Management

### Administrative Access

- **Provide credentials for a NEW administrator account**
  - Never take over existing accounts
  - Use a dedicated admin username for the new owner
  - Ensure the account has full administrative privileges

- **What are all existing user accounts and their roles?**
  - List all administrators, editors, authors, contributors
  - Identify which accounts can be removed post-handover
  - Document any special user permissions or restrictions

### Security Configuration

- **Is two-factor authentication (2FA) enabled?**
  - Which 2FA method is used?
  - How are backup codes managed?

- **Are there any login restrictions or security plugins?**
  - IP whitelisting or geographic restrictions
  - Login attempt limits and lockout policies
  - Password strength requirements

---

## 8. Server Access (FTP/SFTP/SSH)

### File System Access

- **What are the FTP/SFTP credentials?**
  - Host, port, username, and password
  - SSL/TLS requirements and security protocols

- **For SSH access, provide:**
  - SSH key pairs (private and public keys)
  - Location of authorized_keys file
  - Any sudo privileges or user restrictions

### File Structure

- **What is the document root path?**
  - Full path to WordPress installation
  - Location of logs, backups, or temporary files
  - Any symbolic links or unusual directory structures

- **Are there specific file permissions requirements?**
  - Ownership settings for files and directories
  - Any special permissions for uploads or cache directories

---

## 9. Email Configuration

### Email Services

- **How is email handled for the domain?**
  - Professional email service (G Suite, Office 365)
  - Server-based email through hosting provider
  - Third-party email service integration

- **What are the email account credentials?**
  - Admin or primary email account access
  - SMTP settings for transactional emails
  - Any email forwarding or alias configurations

### Email Integration

- **How does the website send emails?**
  - WordPress default mail function
  - SMTP plugin configuration
  - Third-party email service API (SendGrid, Postmark)

---

## 10. Technical Architecture: Themes, Plugins & Custom Code

### Theme Structure

- **What theme is the site using?**
  - Commercial theme name and version
  - Original purchase source and documentation
  - License key and account information

- **Is a child theme properly implemented?**
  - Confirm no modifications to parent theme files
  - Location of child theme customizations
  - Child theme structure and organization

### Plugin Inventory

- **Provide a complete list of all plugins (active and inactive):**
  - Plugin name, version, and purpose
  - Whether it's free or premium
  - License keys and renewal dates for premium plugins
  - Known conflicts or performance issues

### Custom Development

- **Where is custom code located?**
  - Custom PHP in functions.php or child theme files
  - Custom CSS and JavaScript files
  - Code snippets plugin usage
  - Custom plugins developed specifically for the site

- **Are there custom post types, fields, or taxonomies?**
  - How were they created (ACF, custom code, etc.)?
  - Dependencies and relationships between custom content
  - Export/import procedures for custom field configurations

### Code Standards & Documentation

- **What coding standards were followed?**
  - WordPress Coding Standards compliance
  - Code commenting and documentation quality
  - Development methodology and best practices used

---

## 11. Third-Party Services & Integrations

### Service Inventory

**For each integrated service, provide:**

- Service name and purpose
- Account credentials or API keys
- Billing information and renewal dates
- Integration method and dependencies

### Common Services to Document

- **Payment Processing:** Stripe, PayPal, Square
- **Email Marketing:** Mailchimp, ConvertKit, Constant Contact
- **Analytics:** Google Analytics, Google Tag Manager
- **CRM Systems:** Salesforce, HubSpot, Pipedrive
- **CDN Services:** Cloudflare, MaxCDN, KeyCDN
- **Social Media:** Facebook Pixel, Twitter integration
- **Customer Support:** Zendesk, Intercom, LiveChat
- **E-commerce:** WooCommerce extensions, inventory management

### Account Transfer Process

- **What is the procedure for transferring ownership of these accounts?**
- **Are there any services that cannot be transferred?**
- **Which API keys need to be regenerated post-transfer?**

---

## 12. Backup & Disaster Recovery

### Backup Strategy

- **What backup solutions are in place?**
  - Hosting provider automatic backups
  - WordPress backup plugins (UpdraftPlus, BackupBuddy, etc.)
  - Manual backup procedures

- **What is the backup schedule and retention policy?**
  - Frequency (daily, weekly, monthly)
  - How long are backups retained?
  - What components are backed up (files, database, both)?

### Storage & Recovery

- **Where are backups stored?**
  - On-server storage locations
  - Off-site storage (cloud services, remote servers)
  - Multiple backup locations for redundancy

- **What is the documented restoration procedure?**
  - Step-by-step restoration process
  - When was the last successful test restore?
  - Recovery time objectives and procedures

### Disaster Recovery Planning

- **Is there a disaster recovery plan?**
- **What are the procedures for different types of failures?**
- **Who is responsible for executing disaster recovery?**

---

## 13. Security Protocols

### Security Tools & Configuration

- **What security plugins are installed and configured?**
  - Wordfence, Sucuri, iThemes Security, etc.
  - Firewall rules and configurations
  - Malware scanning schedules and settings
  - Login security measures and restrictions

- **What is the user permission structure?**
  - Principle of Least Privilege implementation
  - Role-based access controls
  - Regular access reviews and cleanups

### SSL Certificate Management

- **Who provides the SSL certificate?**
  - Certificate authority (Let's Encrypt, commercial provider)
  - Automatic renewal configuration
  - Certificate expiration monitoring

### Security History

- **Have there been any security incidents?**
  - Past breaches, malware infections, or attacks
  - How were incidents resolved?
  - What preventive measures were implemented?

### Security Monitoring

- **Are there security monitoring tools in place?**
  - File integrity monitoring
  - Login attempt monitoring and alerting
  - Suspicious activity detection

---

## 14. Performance & Caching

### Caching Implementation

- **What caching layers are active?**
  - WordPress caching plugins (WP Rocket, W3 Total Cache, etc.)
  - Server-level caching (Varnish, Redis, Memcached)
  - CDN caching configurations
  - Browser caching settings

- **What is the cache clearing procedure?**
  - Step-by-step process to clear all cache layers
  - When should caches be cleared?
  - Automated cache clearing triggers

### Performance Optimization

- **What performance optimizations are in place?**
  - Image optimization and compression
  - Code minification and concatenation
  - Database optimization procedures
  - Server-level performance tuning

### Performance Monitoring

- **How is site performance monitored?**
  - Performance monitoring tools and services
  - Key performance metrics tracked
  - Alert thresholds and notification procedures

---

## 15. Analytics & SEO

### Analytics Implementation

- **Provide administrative access to:**
  - Google Analytics account and property
  - Google Search Console property
  - Any other analytics tools (Adobe Analytics, etc.)

- **What tracking is currently implemented?**
  - Standard pageview tracking
  - E-commerce or conversion tracking
  - Custom events and goals
  - Cross-domain or subdomain tracking

### SEO Configuration

- **What SEO plugin is used and how is it configured?**
  - Yoast SEO, RankMath, or other SEO plugins
  - XML sitemap configurations
  - Meta tag templates and settings
  - Schema markup implementation

- **What is the current SEO status?**
  - Key ranking keywords and positions
  - Any Google penalties or manual actions
  - Link building campaigns or strategies

---

## 16. Development Environments & Deployment

### Environment Setup

- **Are there development or staging environments?**
  - Staging site URL and access credentials
  - Development environment configuration
  - How environments are synchronized

### Version Control

- **Is the project under version control?**
  - Git repository location and access
  - Branching strategy (GitFlow, feature branches)
  - Which branch represents the live production code?

### Deployment Process

- **What is the exact deployment procedure?**
  - Step-by-step process for pushing changes live
  - Manual vs. automated deployment
  - Pre-deployment testing checklist
  - Rollback procedures for failed deployments

- **How are database changes managed?**
  - Migration scripts or manual procedures
  - Synchronization between environments
  - Data backup before deployment

---

## 17. Documentation & Training

### Available Documentation

- **What project documentation exists?**
  - Technical specifications and system architecture
  - User manuals and admin guides
  - Style guides and brand guidelines
  - API documentation for custom integrations

- **Where is documentation stored and how is it maintained?**

### Training Materials

- **Are training resources available?**
  - Video walkthroughs for common tasks
  - Written procedures for content management
  - Training for custom features or workflows

- **Is live training or handover session available?**
  - Scheduled training session with the development team
  - Q&A session for clarifying procedures
  - Ongoing support for training questions

---

## 18. Maintenance & Monitoring

### Maintenance Procedures

- **What is the established maintenance schedule?**
  - WordPress core, theme, and plugin updates
  - Database optimization and cleanup
  - Security scans and vulnerability assessments
  - Performance reviews and optimizations

### Monitoring Setup

- **What monitoring tools are in place?**
  - Uptime monitoring services and alert recipients
  - Performance monitoring and reporting
  - Error logging and notification systems
  - Resource usage monitoring (disk space, bandwidth)

### Support Structure

- **What ongoing support is available post-handover?**
  - Duration and scope of included support
  - Communication channels and response times
  - Escalation procedures for critical issues
  - Hourly rates for additional work beyond support period

---

## 19. Final Handover Process

### Pre-Handover Preparation

- **Schedule the formal handover meeting:** ________________
- **Complete all inventory tables (see templates below)**
- **Prepare secure credential sharing method (password manager)**

### Handover Day Checklist

- [ ] **Verify access to all systems using inventory tables**
- [ ] **Change all passwords immediately upon access confirmation**
- [ ] **Enable two-factor authentication on all accounts**
- [ ] **Remove previous developer's access from all systems**
- [ ] **Test critical functionality to ensure continuity**
- [ ] **Confirm backup procedures work correctly**

### Post-Handover Actions

- [ ] **Document any immediate issues discovered**
- [ ] **Set up new monitoring and alert recipients**
- [ ] **Review and update emergency contact information**
- [ ] **Plan and schedule first maintenance window**

---

## 20. Exit Interview

These open-ended questions help uncover crucial institutional knowledge:

### Technical Insights

- **What do you consider the most fragile or complex part of this website?**
  - Areas requiring special care or expertise
  - Known stability issues or workarounds
  - Dependencies that are not obvious

### Improvement Opportunities

- **If you had more time, what would you improve first?**
  - Technical debt that should be addressed
  - Performance bottlenecks or optimization opportunities
  - Security enhancements or modernization needs

### Operational Quirks

- **Are there any quirks, oddities, or manual workarounds we should know about?**
  - Unusual procedures for common tasks
  - Workarounds for plugin or theme limitations
  - Manual steps required for certain functions

### Lessons Learned

- **What were the biggest challenges during development?**
  - Problems with specific plugins or integrations
  - Server or hosting limitations encountered
  - Third-party service issues or limitations

- **What are the most important lessons learned from this project?**
  - Best practices that emerged during development
  - Approaches that worked particularly well
  - Things to avoid or be careful about in the future

---

## 21. Inventory Templates

### Master Credentials & Services Inventory

| Service/Platform | Purpose | Login URL | Username/Email | Password Method | API Key | Cost | Renewal Date | Transfer Status |
|-----------------|---------|-----------|----------------|-----------------|---------|------|--------------|----------------|
| WordPress Admin | Content Management | <https://domain.com/wp-admin> | new_admin_user | Bitwarden | -- | -- | -- | ⏳ Pending |
| Domain Registrar | Domain Control | | | | -- | $19.99/year | 2025-10-15 | ⏳ Pending |
| Web Hosting | Server Management | | | | -- | $299/year | 2025-09-01 | ⏳ Pending |
| SSL Certificate | Security | | | | -- | Free/Auto | Auto-renewal | ⏳ Pending |
| Email Service | Communication | | | | | $X/month | Monthly | ⏳ Pending |
| Backup Service | Data Protection | | | | | $X/month | Monthly | ⏳ Pending |
| CDN Service | Performance | | | | API Key | $X/month | Monthly | ⏳ Pending |
| Analytics | Tracking | | | | -- | Free | -- | ⏳ Pending |
| Payment Gateway | E-commerce | | | | API Keys | Transaction fees | -- | ⏳ Pending |

### Plugin & Theme Audit

| Component Name | Type | Version | Purpose | Premium/Free | License Status | Renewal Date | Notes/Risks |
|---------------|------|---------|---------|--------------|----------------|--------------|-------------|
| Active Theme | Parent Theme | x.x.x | Base framework | Premium | Active | 2025-XX-XX | Core visual framework |
| Child Theme | Child Theme | x.x.x | Custom modifications | Custom | N/A | N/A | All customizations here |
| Security Plugin | Plugin | x.x.x | Site protection | Premium | Active | 2025-XX-XX | Critical for security |
| Backup Plugin | Plugin | x.x.x | Data protection | Premium | Active | 2025-XX-XX | Essential for recovery |
| Caching Plugin | Plugin | x.x.x | Performance | Premium | Active | 2025-XX-XX | Key for site speed |
| SEO Plugin | Plugin | x.x.x | Search optimization | Free/Premium | Active/Free | 2025-XX-XX | Important for rankings |

### Server & Infrastructure Details

| Component | Details | Access/Credentials | Notes |
|-----------|---------|-------------------|-------|
| Server Type | Shared/VPS/Dedicated/Managed | | |
| Operating System | Linux/Windows version | | |
| Web Server | Apache/Nginx version | | |
| PHP Version | Current version & extensions | | |
| Database | MySQL/MariaDB version | Host, DB name, user, password | |
| Control Panel | cPanel/Plesk/Custom | Login URL & credentials | |
| FTP/SFTP | File transfer access | Host, port, credentials | |
| SSH Access | Command line access | Keys, authorized_keys location | |

---

## Conclusion

A successful WordPress handover is built on three fundamental principles:

1. **Complete Ownership Transfer** - Full legal and administrative control of all digital assets
2. **Comprehensive Knowledge Transfer** - Deep understanding of technical architecture and business context  
3. **Documented Operational Procedures** - Clear, tested processes for ongoing maintenance and development

By systematically working through this guide, you transform a potentially risky handover into a foundation for long-term success. The upfront investment in due diligence pays dividends in reduced future costs, improved security, and confident independent management of your digital asset.

Remember: A handover is not complete until you have verified access to every system, changed all credentials, removed previous developer access, and tested critical functionality. Take the time to do it right—your website's future health depends on it.
