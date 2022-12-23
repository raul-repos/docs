---
title: Migrating from WordPress
description: Tips for migrating an existing WordPress project to Astro
layout: ~/layouts/MigrationLayout.astro
stub: true
framework: WordPress
---

[WordPress](https://wordpress.org) is an open-source, personal publishing system built on PHP and MySQL.


:::tip
You can [use WordPress as a headless CMS for your Astro project](/en/guides/cms/wordpress/). Follow our guide to use your existing WordPress content in a new Astro project.
:::

## Key Similarities between WordPress and Astro

WordPress and Astro share some similarities that will help you migrate your project:

- Both WordPress and Astro are ideal for content-focused sites like blogs and support writing your content in Markdown. Although the process for adding new content is different, writing in Markdown files for your Astro blog should feel familiar if you have used Markdown syntax in your WordPress editor.

- Both WordPress and Astro encourage you to think about the design of your site in "blocks" (components). In Astro you will probably write more of your own code to create these blocks rather than repy on pre-built plugins. But thinking about the individual pieces of your site and how they are presented on the page should feel familiar.

## Key Differences between WordPress and Astro

When you rebuild your WordPress site in Astro, you will notice some important differences:

- A WordPress site is edited using an online dashboard. In Astro, you will use a code editor and development environment to maintain your site. You can develop locally on your machine, or choose a cloud editor/development environment.

- WordPress has an extensive plugin and theme market. In Astro, you will find some themes and integrations available, but you will probably now have to build many of your existing features yourself instead of looking for third-party solutions. Or, you can choose to start with an [Astro theme](https://astro.build/themes) with built-in features!

- WordPress stores your content in a database. In Astro, you will have individual files (typically Markdown or MDX) in your project directory for each page's content. Or, you can choose to use a headless CMS for your content, and use Astro to fetch and present the data.

## Switch from WordPress to Astro

To convert a WordPress blog to Astro, start with our blog theme starter template, or explore more community blog themes in our [theme showcase](https://astro.build/themes). 

You can continue to [use your existing WordPress blog as your CMS for Astro](/en/guides/cms/wordpress/), which means you will keep using your WordPress dashboard for writing your posts. Your content will be managed at WordPress, but all other aspects of your Astro site will be built in your code editing environment, and you will [deploy your Astro site](/en/guides/deploy/) separately from your WordPress site. (Be sure to update your domain at your host to keep the same website URL!)

You may wish to take [Astro's Build a Blog Tutorial](/en/tutorial/0-introduction/) if you are new to working in a code editor and using GitHub to store and deploy your site. It will walk you through all the accounts and setup you need! You will also learn how to build Astro components yourself, and it will show you how to add blog posts directly in Astro if choose not to use WordPress for you content.

If you want to move all of your existing post content to Astro, you may find this [tool for exporting Markdown to WordPress helpful](https://github.com/lonekorean/wordpress-export-to-markdown). This may be enough for most sites, but you may need to make some adjustments to the result if you have to [convert a large or complicated WordPress site to Markdown](https://swizec.com/blog/how-to-export-a-large-wordpress-site-to-markdown/).

## Community Resources

- Blog Post: [Why I switched from WordPress to Astro](https://dev.to/fratzinger/why-i-switched-from-wordpress-to-astro-5ge) by fratzinger

- Add your own!