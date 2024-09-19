# ALM Roundtable 2024 Tech Radar

![pipeline status](https://github.com/engineering-methods/alm_roundtable_techradar/actions/workflows/generate_radar.yaml/badge.svg)

## Usage / Anatomy

In the folder `radar` the radars are stored.

Each subfolder, e.g. `2024-09-17` represents a radar and markdown files in it represent blips.

Each blip mardown file has to have a markdown frontmatter and the full text description for the blip:

```markdown
---
title: "Blip Name"
ring: ring-name
quadrant: quadrant-name
tags: [ comma-separated-tags ]
---

Description text here... can be any markdown text...
use links to the homepages of the technologies and techniques to make the descriptions more interactive.
```

### Editing

No need to checkout the code, **just hit `.` (point) in the gitlab/github repo main page** to start a browser based visual studio code instance and edit the full repo right there.

Alternatively you can go to a blips' detail screen by clicking on it and click the edit button in the top right corner. This will lead you right to the file in a browser vscode instance.

When you check into main the pipeline will automatically build the radar and publish it to gitlab pages.

> **Is there still a reason to check this repo out?**
>
> Yes, in a local Vscode instance you can have useful extensions like `perkovec.emoji` or `github.copilot` (which is a great help in writing descriptions).

## Development

To build the radar locally:

* clone this repo
* open in vscode
* open devcontainer
* run:

  ```bash
  npm install
  npm run build # build output is in ./build then... run npm run serve for testing
  ```

These two commands are also utilized in the [pipeline](./.github/workflows/generate_radar.yaml).
