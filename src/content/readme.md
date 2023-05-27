---
title: "Readme"
description: "Readme"
---

# Readme

First, ensure you have `astro` installed:

```bash
npm install -g astro
```

Then, run the following command to start the dev server:

```bash
astro dev
```
If you see the following error:
```bash
Error: Cannot find module 'astro/config' imported from .../astro.config.mjs
```
Then run the following command:
```bash
npm install 
```
Then run the following command to start the dev server:
```bash
astro dev
```

At this point, another error could happen:
```bash
---
 failed to import "astro:content"
|- UnknownContentCollectionError: Unexpected error while parsing content entry IDs and slugs.
```
To fix this, you need to create a folder called `content` in the root directory of the project and create a file called `readme.md` inside it. If the readme.md file already exists, then you need to add the following line to the top of the file:
```bash
---
title: "Readme"
description: "Readme"
---
```
This snippet is called frontmatter and it contains the page's metadata.