---
title: Migrating from Docusaurus
description: Tips for migrating an existing Docusaurus project to Astro
layout: ~/layouts/MigrationLayout.astro
stub: true
framework: Docusaurus
---

[Docusaurus](https://Docusaurus.io) is popular documentation website builder built on React.


## Key Similarities between Docusaurus and Astro

Docusaurus and Astro share some similarities that will help you migrate your project:

- Both Astro and Docusaurus are modern, JavaScript-based (Jamstack) site builders intended for content-focused websites, like documenation sites. Both use file-based routing to generate page routes automatically for any MDX file located in `src/pages`. Astro's existing file structure for your page contents, as well as adding new pages, should feel familiar.

- Both Astro and Docusaurus support [MDX pages](/en/guides/markdown-content/), allowing you to author your content in Markdown while incorporating variables, JSX expressions, and component imports.

- Astro has [an official integration for using React components](/en/guides/integrations-guide/react/) and support for NPM packages and community integrations, including several for React. You will be able to write React UI components for interactivity, and may be able to keep some or all of your existing components and dependencies. Astro's JSX-like syntax should feel familiar if you are used to writing React.


## Key Differences between Docusaurus and Astro

When you rebuild your Docusaurus site in Astro, you will notice some important differences:

- Docusaurus is a React-based single-page application (SPA). Astro sites are multi-page apps built using `.astro` components, but can also support React, Preact, Vue.js, Svelte, SolidJS, AlpineJS, Lit and raw HTML templating.

- Docusaurus was designed to build documentation websites and has some built-in, documentation-specific website features that you would have to build yourself in Astro. Instead, Astro offers some documentation-specific features through an [official docs theme](https://github.com/withastro/astro/tree/latest/examples/docs?on=github). This website was built using that template!

- Docusaurus sites use MDX pages for content which allow you to write a combination of JSX and Markdown (although not all of Markdown's features are supported). Astro's docs theme uses Markdown (`.md`) files by default and does not require you to use MDX. You can optionally install Astro's MDX integration and use `.mdx` files in addition to standard Markdown files.


## Switch from Docusaurus to Astro


To convert a Docusaurus documentation site to Astro, start with our docs starter template. Add our MDX integration and bring your existing content files to [create MDX pages](/en/guides/markdown-content/). You can still take advantage of [file-based routing](/en/core-concepts/routing/) by copying these documents directly into `src/pages/` in Astro, the same folder you currently use. Create folders with names that correspond to your existing Docusaurus project, and you should be able to keep your existing URLs. 

Docusaurus probably handled much of your site layout and meta data for you. You may wish to read about [building Astro Layouts as Markdown page wrappers](/en/core-concepts/layouts/#markdownmdx-layouts) to see how to manage templating yourself in Astro, including your page `<head>`.

You can find this, and other templates, on [astro.new](https://astro.new) with links to a GitHub repository as well as one-click links to open a working project in StackBlitz, CodeSandbox and Gitpod online development environments.


## Community Resources

- Add your own!