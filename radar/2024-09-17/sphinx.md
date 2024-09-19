---
title: "Sphinx + Sphinx-Needs"
ring: adopt
quadrant: tools
tags: ["docs-as-code", "requirements", "architecture", "development"]
---

[Sphinx](https://www.sphinx-doc.org/) is a tool that makes it easy to create intelligent and beautiful documentation (originally for Python projects but nowadays also for other documentations) consisting of multiple markup files.
It's strength are it's extensibility (hundreds of available addons, themes etc.) and multiple output formats (HTML, PDF, ePub, etc.).

RestructuredText (reST) is Sphinx's default markup language but also Markdown is supported (with [Myst-Parser](https://myst-parser.readthedocs.io/en/latest/intro.html) extension).

[Sphinx-Needs](https://sphinx-needs.readthedocs.io/en/latest/) is an extension for Sphinx that allows to define requirements or in general objects with attributes and relations in a structured way in your documentation. It can be used to capture requirements, architecture, design decisions, test cases, etc. and visualize them in different views (e.g. table, graph, etc.).

We (:em AG) created a docs-as-code demo site for a past engineering process day:

* Final Sphinx-generated HTML documentation: [docs-as-code-demo](https://engineering-methods.github.io/docs-as-code-demo/).
* Source Code / Repository: [docs-as-code-demo on GitHub](https://github.com/engineering-methods/docs-as-code-demo).

It shows a sphinx rendered documentation, sphinx-needs based requirements and views and tracability of requirements down to the C++ source code with the help of [Doxysphinx](https://boschglobal.github.io/doxysphinx/).
