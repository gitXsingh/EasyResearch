# Security Policy

## Supported Versions

Use this section to tell people about which versions of your project are currently being supported with security updates.

| Version | Supported          |
| ------- | ------------------ |
| 1.0.x   | :white_check_mark: |
| < 1.0   | :x:                |

## Reporting a Vulnerability

We take the security of PaperTeller seriously. If you believe you have found a security vulnerability, please report it to us as described below.

**Please do not report security vulnerabilities through public GitHub issues.**

Instead, please report them via email to [security@paperteller.com](mailto:security@paperteller.com).

You should receive a response within 48 hours. If for some reason you do not, please follow up via email to ensure we received your original message.

Please include the requested information listed below (as much as you can provide) to help us better understand the nature and scope of the possible issue:

- Type of issue (buffer overflow, SQL injection, cross-site scripting, etc.)
- Full paths of source file(s) related to the vulnerability
- The location of the affected source code (tag/branch/commit or direct URL)
- Any special configuration required to reproduce the issue
- Step-by-step instructions to reproduce the issue
- Proof-of-concept or exploit code (if possible)
- Impact of the issue, including how an attacker might exploit it

This information will help us triage your report more quickly.

## Preferred Languages

We prefer all communications to be in English.

## Policy

PaperTeller follows the principle of [Responsible Disclosure](https://en.wikipedia.org/wiki/Responsible_disclosure).

## Security Best Practices

### For Users
- Keep your API keys secure and never commit them to version control
- Use environment variables for sensitive configuration
- Regularly update dependencies
- Use HTTPS in production
- Validate all user inputs

### For Developers
- Follow secure coding practices
- Use parameterized queries to prevent SQL injection
- Implement proper input validation
- Use HTTPS for all communications
- Keep dependencies updated
- Follow the principle of least privilege

## Security Features

PaperTeller includes several security features:
- Input validation and sanitization
- CORS protection
- Rate limiting (can be configured)
- Secure file upload handling
- Environment variable configuration
- No sensitive data in logs

## Updates

Security updates will be released as patch versions (e.g., 1.0.1, 1.0.2) and will be clearly marked in the release notes.

## Acknowledgments

We would like to thank all security researchers and users who responsibly report vulnerabilities to us. 