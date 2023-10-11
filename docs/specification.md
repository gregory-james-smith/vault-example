---
title: Specification
---

A Vault is a folder.

The folder can be held as a git repository to provide version control, but interfacing with git and version control as a feature is outside the scope of Vault.

Each page of a Vault is generated from a markdown file in `/docs` or `/src`.
While the markdown files can be nested in other folders, it is idiomatic for the files to be stored in a flat structure.

The entry point for the Vault is the `index.md` file.

Markdown files in dot folders do not generate Vault pages.
These files can be embedded in pages.

Markdown files can contain YAML frontmatter.

| Frontmatter key | Description |
|-|-|
| title | The title of the Vault page, displayed as the webpage title. |

The filename of the markdown file does not need to match the title of the Vault page, but it is idiomatic that they do.

The name of the Vault webpage will be the markdown filename with spaces replaced with underscores and with `.html` suffix.

# Markdown specification

The specification for the flavour of markdown used is given [here](https://gist.github.com/gregory-james-smith/89e2ebe65d95c3a227dee5ed93c0701a).

## Wikilinks

Vault markdown files support wikilinks.

Wikilinks have the syntax `[[...]]` or `[[...|...]]`.
The first argument is the URL and the second is the markup text of the link.

The URL is relative, case sensitive, with spaces are replaced with underscores, and the file type suffix is ommitted.
