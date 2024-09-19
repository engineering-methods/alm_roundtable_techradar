---
title: "Conan"
ring: adopt
quadrant: tools
tags: [c++, development, packages]
---

[Conan](https://conan.io/) is an open-source dependency management tool for C/C++ applications.

It provides an intuitive interface for defining, fetching and managing dependencies which makes it easy for developers to integrate third-party libraries into their projects.

Conan works across all major operating systems and can target a variety of platforms, including servers and desktop, mobile and embedded devices. It can also be used for building and publishing C/C++ libraries and packages which we view as it's main usecase.

The packages can be shared across teams via different repository systems like:

* [JFrog Artifactory](https://jfrog.com/community/open-source/),
* [Sonatype Nexus](https://github.com/sonatype/nexus-public) or
* [Gitlab](https://docs.gitlab.com/ee/user/packages/conan_repository/).

By leveraging prebuilt binaries, it significantly reduces build times, especially for hefty dependencies. Conan integrates with popular build systems like CMake and also has a Python SDK for extending the build system for tasks like signing.

For one automotive supplier in the audience conan is the standard for managing dependencies C++ (ADAS/embedded) projects.
