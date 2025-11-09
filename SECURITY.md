# Security Policy

## Supported Versions

We actively support the following versions of FileOut with security updates:

| Version | Supported          |
| ------- | ------------------ |
| 1.0.x   | :white_check_mark: |
| < 1.0   | :x:                |

## Reporting a Vulnerability

We take security seriously at FileOut. If you discover a security vulnerability, please help us protect our users by following responsible disclosure practices.

### How to Report

**DO NOT** create public GitHub issues for security vulnerabilities.

Instead, please report vulnerabilities privately to:

**Email:** shady2000gh@gmail.com
**Subject:** [SECURITY] Brief description of the issue

### What to Include

Please provide as much information as possible:

1. **Description:** Clear explanation of the vulnerability
2. **Impact:** Potential consequences if exploited
3. **Reproduction Steps:** Detailed steps to reproduce the issue
4. **Proof of Concept:** Code, screenshots, or video demonstration
5. **Environment:** Browser, OS, FileOut version
6. **Suggested Fix:** If you have recommendations (optional)

### Response Timeline

- **Initial Response:** Within 48 hours
- **Status Update:** Within 7 days
- **Fix Timeline:** Critical issues within 30 days, others within 90 days
- **Disclosure:** Coordinated disclosure after fix is deployed

### Security Reward

While we do not currently have a formal bug bounty program, we appreciate security researchers and may offer:
- Public acknowledgment (if desired)
- Free premium credits
- Recognition in our security hall of fame

## Security Best Practices for Users

### Account Security
- Use strong, unique passwords (minimum 12 characters)
- Enable two-factor authentication (when available)
- Never share your account credentials
- Log out from shared or public devices
- Review account activity regularly

### Data Protection
- Do not include sensitive information in document prompts (SSN, passwords, etc.)
- Delete documents containing confidential data after download
- Use encryption for highly sensitive documents
- Review generated content before sharing externally

### Phishing Awareness
- Verify email sender addresses (official emails come from shady2000gh@gmail.com)
- Be cautious of unsolicited emails requesting account information
- Access FileOut directly via https://fileout.online (not email links)
- Report suspicious emails to shady2000gh@gmail.com

## Our Security Measures

### Infrastructure
- **Encryption:** TLS 1.3 for data in transit, AES-256 for data at rest
- **Authentication:** Bcrypt password hashing, JWT tokens
- **Database:** PostgreSQL with parameterized queries (SQL injection prevention)
- **Cloud Security:** Supabase with row-level security policies
- **Firewall:** Web application firewall (WAF) protection
- **Monitoring:** Real-time security monitoring and alerting

### Application Security
- **Input Validation:** All user inputs sanitized and validated
- **CSRF Protection:** Cross-Site Request Forgery tokens
- **XSS Prevention:** Content Security Policy (CSP) headers
- **Rate Limiting:** API throttling to prevent abuse
- **Dependency Scanning:** Automated vulnerability scanning of npm/pip packages
- **Code Review:** Security review for all major changes

### Data Privacy
- **Minimal Collection:** Only collect data necessary for service operation
- **Access Controls:** Role-based access with principle of least privilege
- **Audit Logs:** Comprehensive logging of sensitive operations
- **Data Retention:** Automatic deletion of documents after 90 days (configurable)
- **GDPR/CCPA Compliance:** Data protection rights and deletion tools

### Third-Party Security
- **Vendor Assessment:** Due diligence on all third-party services
- **API Security:** Secure API key management and rotation
- **Payment Security:** PCI-DSS compliant payment processors
- **AI Model Providers:** Vetted providers with data protection agreements

## Security Audits

- **Internal Audits:** Quarterly security reviews
- **Penetration Testing:** Annual third-party security assessments
- **Dependency Updates:** Weekly automated scans for vulnerable packages
- **Compliance:** Regular GDPR, CCPA, and SOC 2 compliance reviews

## Incident Response

In the event of a security incident:

1. **Detection:** Automated monitoring and user reports
2. **Containment:** Immediate action to limit impact
3. **Investigation:** Root cause analysis and affected user identification
4. **Remediation:** Patch deployment and system hardening
5. **Notification:** Affected users notified within 72 hours (GDPR requirement)
6. **Post-Mortem:** Incident review and prevention measures

## Known Security Considerations

### AI-Generated Content
- AI models may occasionally produce sensitive or inappropriate content
- Users should review all generated documents before use
- We implement content filtering but cannot guarantee 100% accuracy

### Third-Party Dependencies
- We rely on OpenRouter, Supabase, and other services
- We monitor their security advisories and update promptly
- Service interruptions may occur due to third-party incidents

## Security Updates

Subscribe to security notifications:
- **GitHub Watch:** Click "Watch" → "Custom" → "Security alerts"
- **Email:** Opt-in for security announcements in account settings
- **Status Page:** https://status.fileout.online (coming soon)

## Compliance and Certifications

FileOut is committed to compliance with:
- **GDPR** (General Data Protection Regulation)
- **CCPA** (California Consumer Privacy Act)
- **SOC 2** (in progress)
- **OWASP Top 10** security practices

## Contact

For security concerns:

**Email:** shady2000gh@gmail.com
**Security Lead:** Shady Ghonim

---

**Last Updated:** November 9, 2025

Thank you for helping us keep FileOut secure!

Copyright © 2025 Shady Ghonim. All rights reserved.
