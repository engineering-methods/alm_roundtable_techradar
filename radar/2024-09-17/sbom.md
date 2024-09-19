---
title: "Software Bill of Materials (SBOM)"
ring: assess
quadrant: platforms-and-operations
tags: [ci-cd, security]
---

A Software Bill of Materials (SBOM) is an artifact that aggregates information about a software's dependencies.

There are a number of standards that define the content and format of SBOMs. The 2 most widely used open source formats/specifications are:

- [CycloneDX](https://cyclonedx.org/) (OWASP): developed in 2017 with the initial goal of identifying vulnerabilities in the software supply chain.
- [SPDX](https://spdx.dev/) (Linux Foundation): at first primarily focused on license compliance in the context of open source software. In 2016, SPDX 2.1 added support for vulnerability tracking.

With more and more software supply chain attacks, SBOMs are becoming increasingly important.
Also license compliance is a big topic especially in the context of open source software utilization.

We see the potential for SBOMs to improve the security of the software supply chain by

- Providing visibility into direct and transitive software dependencies.
- Automating the discovery of software dependencies with known vulnerabilities.
- Capturing dependency information of software components that are otherwise not visible anymore once the software is built and/or deployed.
