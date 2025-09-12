# repo-best-practices

From an [R Dev Day issue](https://github.com/r-devel/r-dev-day/issues/51), we are collating best-practices to apply to r-devel repos.

At the moment, we are gathering ideas on best practices.

See also [GitHub's guide to repo best practices](https://docs.github.com/en/repositories/creating-and-managing-repositories/best-practices-for-repositories)

## General best practices for all repos

- README.md
    - Include example of how to use the project.
    - Comments should include break down of code describing function and method responsibility.
- CONTRIBUTING.md
    - Decribe process for code review for developers to review changes.
    - (Do we have a general one for the R Contributor project?)
- LICENSE.md
    - Make sure this is appropriate for the repo
- CODE_OF_CONDUCT.md
    - (Do we have one for the R Contributor group?)
- Securing the repo
    See [GitHub's Quickstart guide](https://docs.github.com/en/code-security/getting-started/quickstart-for-securing-your-repository)
- Protecting branches
- [All Contributors](https://allcontributors.org/)
- [CITATION.cff](https://citation-file-format.github.io/)
- Accessibility (at minimum)
    - Alt-text for all images
    - Colour contrast requirements
    - Screen reader compatibility
    - Keyboard navigation
- Issue and PR templates
- Issue labels
- Repository topics and tags
- CHANGELOG.md or NEWS.md to document version history and breaking changes
- Website or homepage URL

## Repo-specific considerations

- CI/CD
    - For Quarto books and websites, use GHA for publishing
        - Is publication on push to main appropriate in these cases?
- pre-commit hooks
    - Which would be useful for which type of project?
- For website projects, check accessibility with the [wave tool](https://wave.webaim.org/)  
    via their [browser extensions](https://wave.webaim.org/extension/)
    - Note that there are [some issues](https://github.com/quarto-dev/quarto-cli/issues?q=is%3Aissue%20state%3Aopen%20label%3Aaccessibility) that will need raising with Quarto

