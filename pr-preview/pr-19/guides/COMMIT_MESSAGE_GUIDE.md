# Effective Commit Messaging

Clear and informative commit messages contribute significantly to a project's success. This guide
outlines the importance of well-structured commit messages and descriptions.

## Basic commit message structure

A well-crafted commit message is structured to convey concise and actionable information about the
changes made. It typically consists of a single-line summary and an optional extended description.

### Summary line

A good summary line is:

- **Directive**: start with a concise imperative verb to indicate the action,
  e.g.: `add`, `fix`, `update`.
- **Specific**: it answers the question: What was done in this commit?
- **Concise**: Keep it short and focused.

Example: `add authentication integration`.

### Description

You can and should extend the commit message with a description. In the description you can
reference issues, provide more detail and motivate your changes. Use bullet points for readability.

Following the previous example:

```
Resolves #123 by securing access through authentication.

- Implemented OAuth2 for secure user login
- Implemented a custom login screen
- Updated database schema to store user credentials securely
```

Here are some benefits of using commits descriptions:

- **Motivate Choices**: Helps collaborators understand the reasoning behind specific decisions.
- **Ease PR Creation**: Pre-populated the description of a pull request with the commit description.
- **Archival Information**: Provides insight as a historical record when using inspection tools.
- **Better collaboration**: A clean history makes it easier to understand and build upon previous
  work.
- **Traceability**: Tracing back changes allows developers to easily identify the introduction of
  bugs or issues.

## A case for conventional commits

The [Conventional Commits specification][conventional-commits] provides a set of rules to simplify
creating a clear commit history, making it easier to build automated tools on top of it. Some
of the benefits of this approach:

- **Automated Version Bumping**: Enable automated version bumping.
- **Automated Release Notes**: Generate consistent release notes based on commit messages.
- **Granular Filtering**: Facilitate filtering and navigation through commits based on their type.
- **Enforceable**: Ensure adherence to the convention through a pre-commit hook.

### Case of study

Explore the commit histories of [pillarbox-web][pillarbox-web-history]
and [pillarbox-web-demo][pillarbox-web-demo-history]. Both projects diligently adhere to the
guidelines outlined in this article, incorporating conventional commits. A pre-commit hook is
implemented in both cases to enforce adherence to the conventional commit format.

For the former project, automated processes generate release notes and versions using semantic
versioning. See the outcome for the [1.1.0 release of pillarbox-web][semver-release-example].

## Conclusion

Incorporating the practices outlined in this guide ensures that your commit messages and
descriptions contribute positively to your project's development lifecycle. A well-documented commit
history is a powerful collaboration tool.

[conventional-commits]: https://www.conventionalcommits.org/en/v1.0.0/

[pillarbox-web-history]: https://github.com/SRGSSR/pillarbox-web/commits/main/

[pillarbox-web-demo-history]: https://github.com/SRGSSR/pillarbox-web-demo/commits/main/

[semver-release-example]: https://github.com/SRGSSR/pillarbox-web/releases/tag/v1.1.0
