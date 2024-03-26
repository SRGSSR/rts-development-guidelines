# GitHub Security Guide

## Repository Access Settings
For products with sensitive information or proprietary code, set the repository as private to
maintain confidentiality and control access. For open-source projects or non-sensitive content,
consider making the repository public to encourage collaboration and transparency.

## Enable Dependency Graph for Private Repositories
Enable the Dependency Graph feature for private repositories to automatically track and manage
dependencies.
This feature helps identify and address vulnerabilities in project dependencies by providing
insights into package versions and usage.

## Enable Dependabot Alerts, Security Updates, and Version Updates
Enable Dependabot alerts to receive notifications about vulnerable dependencies in your
repositories.
Configure Dependabot to automatically apply security updates and version updates when available.
Regularly review and merge Dependabot pull requests to keep dependencies up-to-date and secure.

## Code Scanning
You may enable GitHub code scanning to automatically detect and flag potential security
vulnerabilities in your code.
You can also integrate code scanning into your CI/CD pipeline to catch issues early in the
development process.
Address identified vulnerabilities promptly and thoroughly to minimize security risks.

## Secret Scanning
You may enable secret scanning to detect and prevent the exposure of sensitive information, such as
API keys, passwords, and tokens, in your repositories.
Regularly review secret scanning alerts and take action to remove or secure any exposed secrets.

---

*You can find more information about these security features in the official [GitHub documentation][github-doc].*

## Write a security policy
Having a security policy ensures easy access to maintained versions list, major security rules and
vulnerabilities report guidelines among other things.

This template will assist you in creating a concise SECURITY POLICY for your project which should
be a `SECURITY.md` file at the root of the repository.

```markdown
# Security Policy

## Supported versions
> Use this section to tell people about which versions of your project are currently being
> supported with security updates.

Sample table:
| Version | Supported          |
| ------- | ------------------ |
| 5.1.x   | :white_check_mark: |
| 5.0.x   | :x:                |
| 4.0.x   | :white_check_mark: |
| < 4.0   | :x:                |

## Dependencies
Only supported versions of software, libraries, and frameworks shall be used. Regularly update
dependencies to ensure compliance with supported versions and address known vulnerabilities.

## Secrets
Under no circumstances shall sensitive information, such as passwords, API keys, or access tokens,
be stored in the repository. Securely manage secrets using a dedicated secrets management tool
or environment variables.

## Reporting a Vulnerability
To report a vulnerability, open an issue with the "security" label on GitHub. Additionally, open a
Jira SMAC issue with a link to the GitHub issue for tracking and coordination.

## Code Reviews
All code changes must undergo thorough review by at least one other team member before being merged
into the main branch. Code reviewers shall ensure that changes meet coding standards, security
requirements, and best practices.

## Compliance
This repository shall comply with relevant laws, regulations, and industry standards governing the
protection of data and intellectual property. Regular audits and assessments shall be conducted to
verify compliance and address any non-compliance issues promptly.
```

[github-doc]: https://docs.github.com/en/code-security/getting-started/securing-your-repository