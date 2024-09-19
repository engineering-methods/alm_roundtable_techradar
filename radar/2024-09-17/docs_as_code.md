---
title: "Docs As Code"
ring: adopt
quadrant: techniques
tags: [ method, docs, lta ]
---

Docs-as-Code is an approach to documentation that treats documentation in a way similar to how code is treated in software development. This means applying software development best practices to the creation, management, and maintenance of documentation.

Documentation is typically written with markup languages like Markdown, reStructuredText or AsciiDoc and then rendered into different formats (HTML, PDF, etc) through different open source tools.

It is then stored in version control (usually git) so full auditability is given.

Collaboration is easy because of the established processes like pull requests etc, and pipelines can automatically generate the documentation, merge in data from external sources and push the resulting htmls to a web server (or some service like github/gitlab pages).

The benefits are no vendor lock in, documentation lives right where the code lives.

We think that, especially for documentation around software, ALM and processes this is a really viable option, especially as as-good-as all source code management systems have the ability to view markup files directly at the repo level (even without using html generation).

There is also a more "extended" variant of docs-as-code utilized in the automotive industry where also requirements, architecture, tests or assets along the aspice V-model are represented in neutral formats and then rendered into an interactive linkable documentation to capture tracability information.

The blip author is utilizing this to full extend and while the integration with brownfield projects is a challenge because of integrating the "classic" tool zoo the benefits still outweigh the challenges.
The recommended tooling there is [Sphinx](https://www.sphinx-doc.org/) with [Sphinx-Needs](https://sphinx-needs.readthedocs.io/en/latest/) (also on this radar). There is however some integration work there to be done but there aren't many alternatives that are as powerful Sphinx.

At :em AG we also thinking about using some sort of docs-as-code approach in the long term archiving space, as the neutral text based formats are a good way to ensure that the data is accessible in the future.
