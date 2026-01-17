---
name: web-security
description: Expert knowledge in implementing secure web applications and protecting against common vulnerabilities. Covers OWASP Top 10, authentication and authorization, data protection, Content Security Policy (CSP), HTTPS/TLS, input validation, secure dependencies, and API security. Use when implementing security features or addressing security vulnerabilities.
metadata:
  version: 1.0.0
---

# Web Security Skill

Expert knowledge in implementing secure web applications and protecting against common vulnerabilities.

## Core Competencies

- **OWASP Top 10**: Understanding and mitigating common web vulnerabilities
- **Authentication & Authorization**: Implementing secure auth systems
- **Data Protection**: Protecting sensitive data in transit and at rest
- **Content Security Policy (CSP)**: Preventing XSS and injection attacks
- **HTTPS/TLS**: Ensuring secure communication
- **Input Validation**: Sanitizing and validating user input
- **Secure Dependencies**: Managing and auditing third-party packages
- **API Security**: Securing REST and GraphQL APIs

## OWASP Top 10 Vulnerabilities

1. **Broken Access Control**
   - Implement proper authorization checks
   - Use principle of least privilege
   - Deny by default

2. **Cryptographic Failures**
   - Use TLS for data in transit
   - Encrypt sensitive data at rest
   - Use strong, standard algorithms
   - Never store passwords in plaintext

3. **Injection Attacks**
   - Use parameterized queries (prevent SQL injection)
   - Sanitize user input
   - Use Content Security Policy
   - Validate and escape output

4. **Insecure Design**
   - Threat modeling
   - Secure by design principles
   - Security requirements gathering

5. **Security Misconfiguration**
   - Remove default credentials
   - Keep software updated
   - Disable unnecessary features
   - Set secure headers

6. **Vulnerable and Outdated Components**
   - Regular dependency audits
   - Automated security scanning
   - Keep dependencies updated

7. **Identification and Authentication Failures**
   - Implement MFA
   - Strong password policies
   - Secure session management
   - Rate limiting

8. **Software and Data Integrity Failures**
   - Use Subresource Integrity (SRI)
   - Verify digital signatures
   - Validate data integrity

9. **Security Logging and Monitoring Failures**
   - Log security events
   - Monitor for suspicious activity
   - Implement alerting

10. **Server-Side Request Forgery (SSRF)**
    - Validate and sanitize URLs
    - Use allowlists for external resources
    - Network segmentation

## Security Headers

```
Content-Security-Policy: default-src 'self'
X-Content-Type-Options: nosniff
X-Frame-Options: DENY
X-XSS-Protection: 1; mode=block
Strict-Transport-Security: max-age=31536000; includeSubDomains
Referrer-Policy: strict-origin-when-cross-origin
Permissions-Policy: geolocation=(), microphone=(), camera=()
```

## Best Practices

1. **Input Validation**
   - Validate on client AND server
   - Use allowlists over denylists
   - Sanitize HTML input (use DOMPurify)
   - Validate file uploads

2. **Authentication**
   - Use proven authentication libraries
   - Implement proper session management
   - Use HttpOnly and Secure cookies
   - Implement CSRF protection

3. **Data Protection**
   - Never expose sensitive data in URLs
   - Use encryption for sensitive data
   - Implement proper access controls
   - Minimize data collection

4. **API Security**
   - Use authentication tokens (JWT, OAuth)
   - Implement rate limiting
   - Validate request origins (CORS)
   - Use API keys securely

5. **Dependency Management**
   - Regular npm/yarn audit
   - Use tools like Snyk or Dependabot
   - Pin dependency versions
   - Review dependencies before adding

## Testing Tools

- OWASP ZAP
- Burp Suite
- npm audit / yarn audit
- Snyk
- SonarQube
- Security headers checker
- SSL Labs (for HTTPS configuration)
