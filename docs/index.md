---
title: Vault
subtitle: An example
---

A vault is a personal knowledge base^[A database for storing and organising personal knowledge.]
consisting of a wiki hypermedia structure^[A hypertext web publication with little inherent structure.]
of markdown^[Markdown is a lightweight markup language for rich text whose files have the `.md` extension and is designed to also be human readable in its plain text source code form.] files.

# Wikilinks

Vault markdown files support wikilinks.

Wikilinks have the syntax `[[...]]` or `[[...|...]]`.
The first argument is the URL and the second is the markup text of the link.

The URL is relative, case sensitive, with spaces are replaced with underscores, and the file type suffix is ommitted.

# Contents

* [[./specification|Specification]]
* [[./headers]]
* [[./design-objectives|Design objectives]]
