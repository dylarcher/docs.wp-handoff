# WordPress Project Hand-Off Questions

## 1. Hosting Service

### Provider and Account Access

- What is the name of the hosting provider?
- How do I access the hosting account (e.g., control panel URL, username, password)?
- Are there any multi-factor authentication (MFA) or additional security measures in place?

### Server Details

- What type of hosting plan is being used (e.g., shared, VPS, dedicated)?
- What is the server operating system (e.g., Linux, Windows)?
- Are there any specific server configurations or settings I should be aware of (e.g., PHP version, memory limits, caching setups)?

### Domain and DNS

- Is the domain registered through the hosting provider or a separate registrar?
- How do I access the domain management panel (if separate)?
- Are there any custom DNS settings or records that need to be maintained?

---

## 2. WordPress Website

### Admin Access

- What is the URL for the WordPress admin dashboard?
- What are the admin login credentials (username and password)?
- Are there any additional security measures for the admin area (e.g., 2FA, IP restrictions)?

### Themes and Plugins

- Which theme is currently active, and is it a custom or third-party theme?
- Are there any child themes in use?
- What plugins are installed and activated? Are there any custom or premium plugins?
- Are there specific versions of themes or plugins that must be maintained for compatibility?

### Customizations

- Are there any custom code modifications in the theme or plugins (e.g., via functions.php or custom templates)?
- Are there any custom post types, taxonomies, or fields (e.g., via ACF or other plugins)?
- Is there any custom CSS or JavaScript added to the site (and where is it located)?

---

## 3. SSH and Server Access

### SSH Provider and Credentials

- Is SSH access provided through the hosting service or a separate provider?
- What are the SSH login credentials (username, password, or key file)?
- What is the SSH host address and port number?
- Are there any specific SSH configurations or commands I should use to connect?

### File System Access

- What is the root directory path for the WordPress installation?
- Are there any specific directories or files that require special permissions?
- Is there an SFTP or FTP setup in addition to SSH, and if so, what are the credentials?

---

## 4. Database Access

### Database Details

- What is the name of the WordPress database?
- What are the database credentials (username, password, host)?
- How do I access the database (e.g., via phpMyAdmin, command line)?

### Database Management

- Are there any custom tables or database modifications beyond standard WordPress?
- Is there a backup schedule for the database, and how can I access or restore backups?

---

## 5. Custom Configurations and Server Files

### Custom Server Files

- Are there any custom PHP files outside of the WordPress core (e.g., in the root directory)?
- Are there modifications to the `.htaccess` file (for Apache) or `nginx.conf` (for Nginx)?
- Are there any cron jobs or scheduled tasks set up on the server?

### Environment-Specific Settings

- Are there different configurations for development, staging, and production environments?
- Is there a `wp-config.php` file with custom constants or settings?

---

## 6. Backup, Updates, and Security

### Backup Procedures

- What is the current backup strategy for the website (e.g., frequency, storage location)?
- Are backups automated, and if so, how can I access or manage them?

### Update Schedule

- How are updates handled for WordPress core, themes, and plugins (e.g., manual or automatic)?
- Is there a specific time or process for applying updates to avoid downtime?

### Security Measures

- What security plugins or measures are in place (e.g., firewalls, malware scanners)?
- Are there any custom security configurations (e.g., in `.htaccess` or server settings)?
- Is SSL/TLS enabled, and how is the certificate managed (e.g., auto-renewal)?

---

## 7. Development Workflow and Version Control

### Staging and Testing

- Is there a staging or development environment? If so, how do I access it?
- What is the process for testing changes before deploying to the live site?

### Version Control

- Is version control (e.g., Git) used for the project? If so, where is the repository hosted (e.g., GitHub, Bitbucket)?
- What is the branching strategy (e.g., main branch for production, feature branches for development)?
- Are there any specific deployment scripts or tools used to push changes to the server?

### Documentation

- Is there any existing documentation for the project (e.g., setup guides, code comments)?
- Are there any known issues or bugs that need attention?

---

## 8. Additional Information

### Third-Party Integrations

- Are there any third-party services integrated with the website (e.g., payment gateways, APIs, email services)?
- What are the credentials or API keys for these services, and where are they stored?

### Monitoring and Analytics

- Is there any monitoring or analytics setup (e.g., Google Analytics, server monitoring tools)?
- How can I access these tools or reports?

### Client or Team Access

- Are there other team members or clients who have access to the website or hosting?
- What are their roles and permissions?

---

By gathering answers to these questions, the new developer will have all the necessary information to take over the WordPress project effectively, ensuring continuity and minimizing disruptions.
