# Pull Request Manual

Pull Requests are an integral aspect of a collaborative project. Through this process, contributors
can propose modifications, enhancements, or new features to a codebase. **The true strength of a
pull request lies in the subsequent peer review.**

## Why Code Reviewing Matters

- **Code Quality and Consistency:** Code reviewing ensures that the code adheres to established
  standards, follows best practices, and maintains a high level of quality.
- **Knowledge Sharing:** With code reviews, contributors can learn from each other's problem-solving
  approaches, coding styles, promoting a culture of continuous learning within the team.
- **Bug Prevention:** A fresh set of eyes often catches issues that the original author might have
  overlooked.

## The Pull Request Template

The pull request template is a valuable tool for creating a successful pull request. It is a guide
to help contributors understand what is expected of them.

Here are some reasons why adding a pull request template to your repository is important:

- **Clarity and Consistency**: A pull request template ensures that every contributor provides the
  necessary information when proposing changes.
- **Efficiency**: With a template, reviewers don't have to ask basic questions about the pull
  request, as most of the essential details should be included in the template.
- **Documentation**: Detailed pull requests serve as a form of documentation, providing insight into
  the project's history and the rationale behind certain decisions.
- **Quality Control**: A checklist in the template can serve as a reminder for contributors to
  adhere to the project's standards and guidelines, leading to higher quality submissions.

### Adding a Pull Request Template

You can store your pull request template in `.github/pull_request_template.md`.
You can review other options on the [GitHub documentation][github-creating-pr-template].

### Example

Here's an example of a pull request template; feel free to use it in your project and modify it to
your needs:

```markdown
## Description

> Please provide a brief summary of the changes made. Please explain why
> this change was necessary. Was there a problem or an issue this change
> will address? What will be improved with this change?

## Changes Made

> Please detail the modifications made. This could include areas such as
> code, documentation, structure, or formatting.

## Checklist

- [ ] I have followed the project's style guidelines.
- [ ] I have performed a self-review of my own changes.
- [ ] I have made corresponding changes to the documentation.
- [ ] My changes do not generate new warnings.
- [ ] I have added tests that prove my fix is effective or that my feature works.
- [ ] I have reviewed the contribution guidelines.
```

#### Creating a Checklist

You can add a **Checklist** section to further guide contributors. In this section, add items that
reflect the "Definition of Done" for your project or any specific guidelines mentioned in the
"Contributing" section of the README. This could include items like:

- My code follows the code style of this project.
- I have added tests to cover my changes.
- All new and existing tests passed.
- My changes generate no new warnings.
- I have updated the documentation accordingly.

> [!Note]
> Remember, the goal of the pull request template is to make collaboration easier by setting clear
> expectations for contributions. Tailor it to suit the specific needs of your project.

[github-creating-pr-template]: https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/creating-a-pull-request-template-for-your-repository
