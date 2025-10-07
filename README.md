# repo-best-practices

From an [R Dev Day issue](https://github.com/r-devel/r-dev-day/issues/51), we are collating best-practices to apply to r-devel repos.

At the moment, we are gathering ideas on best practices.

See also [GitHub's guide to repo best practices](https://docs.github.com/en/repositories/creating-and-managing-repositories/best-practices-for-repositories)

## Essential best practices (advised for all r-devel repos)

- README.md
    - Include example of how to use the project.
    - Comments should include break down of code describing function and method responsibility.
- CONTRIBUTING.md
    - Decribe process for code review for developers to review changes.
    - Create one for the r-devel org as a whole - see https://github.com/r-devel/repo-best-practices/issues/1
- LICENSE.md
    - Make sure this is appropriate for the repo (see https://choosealicense.com/)
        - (Could consider making recommendations for different project types)
- .gitignore
    -  A standard .gitignore including basics for R & quarto 
- CODE_OF_CONDUCT.md
    - Create one for the r-devel org as a whole - see https://github.com/r-devel/repo-best-practices/issues/2
- [CODEOWNERS](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners) file
- Securing the repo
    - Dependabot alerts
    - Secret scanning
    - Push protection
    - Code scanning
    See [GitHub's guide to repo best practices](https://docs.github.com/en/repositories/creating-and-managing-repositories/best-practices-for-repositories) and [GitHub's security Quickstart guide](https://docs.github.com/en/code-security/getting-started/quickstart-for-securing-your-repository) for more details
- Website or homepage URL

## Advisable best practices (nice to have at maintainer's discretion)

- [Issue and PR templates](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/about-issue-and-pull-request-templates)
- Issue labels
- [All Contributors](https://allcontributors.org/)
- [CITATION.cff](https://citation-file-format.github.io/)
- [Branch protection](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/about-protected-branches)
- [Repository topics](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/classifying-your-repository-with-topics) 

## Repo-specific considerations

### Quarto projects

- Use [GHA for publishing](https://quarto.org/docs/publishing/github-pages.html#github-action)
- Check accessibility with the [wave tool](https://wave.webaim.org/)  
    via their [browser extensions](https://wave.webaim.org/extension/)
    - Alt-text for all images
    - Colour contrast requirements
    - Note that there are [some issues](https://github.com/quarto-dev/quarto-cli/issues?q=is%3Aissue%20state%3Aopen%20label%3Aaccessibility) with Quarto sites revealed by wave that will need raising with Quarto
- Encourage engagement and contribution with repository links
```
website:
  repo-url: https://github.com/r-devel/YOUR-REPO
  repo-actions: [edit, issue]
```
- Consider "editions" of books (with changes tracked in a CHANGELOG.md or NEWS.md)
    - Look at other community books (e.g. [The Turing Way](https://book.the-turing-way.org/)) to see how they handle this

### Software Projects

- Document changes by version number in CHANGELOG.md or NEWS.md
- Create GitHub releases for new versions
- Use [semantic versioning](https://semver.org/)
- Release strategy, e.g. semantic versioning, release notes, deployment process

### Further considerations
- pre-commit hooks
    - Which would be useful for which type of project?



