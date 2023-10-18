---
title: Implementation
---

A basic explaination of the implementation is that `pandoc` is used to generate a webpage from every markdown file.

See the actions in `/.github`.
🚧 This is a work in progress and other implementations will be created.

<!-- Make a table of the design objectives and then discuss how they were achieved. Maybe this should be in a design decision page. -->

## Styelsheet template

A CSS stylesheet file is used to style the pages.
This is stored in a separate repository.

The stylesheet is retrieved using the [GitHub CLI](https://docs.github.com/en/actions/using-workflows/using-github-cli-in-workflows) and a [personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens) stored as a secret to [access a repo content using the GitHub API](https://docs.github.com/en/rest/repos/contents?apiVersion=2022-11-28).
Alternatively the GitHub API can be called with [curl](https://docs.github.com/en/rest/overview/authenticating-to-the-rest-api?apiVersion=2022-11-28).
