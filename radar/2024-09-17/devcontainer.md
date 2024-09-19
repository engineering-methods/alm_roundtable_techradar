---
title: "Dev Containers"
ring: adopt
quadrant: techniques
tags: [vscode, container, development]
---

[Devcontainers](https://containers.dev/) are a mechanism to define a development environment in a container.
This includes tooling inside the container, as well as extensions for the IDE which typically runs "outside" on the host.

The most prominent (and also first) implementation is available in Visual Studio Code. Other IDEs like the Jetbrains IDEs (IntelliJ IDEA, Pycharm etc) also support this feature.

This is especially useful when you have a complex development environment that you want to share with your team.
It allows you to define the tools, runtime, and extensions that are needed for your project in a `devcontainer.json` file that lives right in the source code repository.
When a team member opens the project in a supporting IDE, they will be prompted to open the project in a container. The IDE will then start the container, attach to it and also reconfigure itself based on the settings defined in the `devcontainer.json` (extensions, etc).
With this each developer in your team will have the exact same development environment.
It also resonates very well with [Intelligent repository templates](https://de.linkedin.com/pulse/softwareentwicklung-professionalisieren-mit-0taie).

One attendee and also the :em AG are using devcontainers in their projects and libraries. From :em AG's perspective also some customers are starting to use this feature with great success.

Another attendee mentioned that they evaluated devcontainers, but for small teams of around 3 developers it was faster for them to just install the Java IDE for their development. So this tends to be more useful for larger teams or teams with more complex development environments - with many different tools to setup, many project specific settings etc.
