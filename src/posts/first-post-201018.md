---
title: Paladin START
description: First blog post at Paladin Prototypes. Currently undergoing testing...
date: 2020-10-18
tags:
  - test

---
This page is currently being used for testing. The following issues and obeservations are noted for October 18, 2020:

- NetlifyCMS requires configuration provided in `src/admin`. 
- The build directory `_site` (specified in `netlify.toml`) does not reflect the generated markup (i.e. no html or javascript files found in this folder) 
- Navigation for this site is managed via `navigation.yaml` and `quicklinks.yaml` (located in `src/_data`), where `title` and `url` are fields containing content for related HTML templates.
- Blog posts saved via NetlifyCMS ( [hosted collections page at Netlify](/admin/#/collections/blog) ) do not appear in the blog (i.e. the boilerplage content remains). The reason for this may be due to host server delay. or sync process in netlify deploy command (netlify-cli run script).
- The template for the blog index page is contained in `src/blog`, whereas post files are in `src/posts`
- The run script `netlify deploy --prod` returns a server log link that allows you to see logged output in the browser (i.e. logs that were saved at `app.netlify.com/teams`). This information is reached in the UI's teams view under `Builds`. For each build there is a link that loads a page with 3 sections: `Deploy successful`, `Deploy summary` and `Deploy log` (i.e. dated terminal logs)


## PENDING TASKS

**paladin-prototypes.com**

- Convert templates `_includes/*` into pug
- Install and configure pug in `.eleventy` config file; log results in this page.
- Document eleventy `_data` file generation (i.e. how YAML data is recognized during build step)

**paulopath.com**

- Install `js-yaml` and update `.eleventy`; convert `src/_data/*.json` into `src/_data/*.yml`
- Install and configure `pug`; convert `src/_includes/*.njk` into `src/_includes/*.pug`
