# Welcome to Minidyne, a minimalist hexo theme

![Screenshot of this site](https://hexo-theme-minidyne-demo.netlify.com/screenshot.png)

[Live Demo on Netlify](https://hexo-theme-minidyne-demo.netlify.com/)
([Source for the demo on Github](https://github.com/tomap/hexo-theme-minidyne-demo))

<!-- more -->

[![NPM version](https://badge.fury.io/js/hexo-theme-minidyne.svg)](https://www.npmjs.com/package/hexo-theme-minidyne)

This is V3. 
For V2 of this theme, [head over to V2](https://github.com/tomap/hexo-theme-minidyne/tree/v2).
For V1 of this theme, [head over to V1](https://github.com/tomap/hexo-theme-minidyne/tree/v1).

## Features Overview

- Responsive
- Tags Support
- Accessible colors (at least the default one)
- Responsive Images
- Social Accounts configuration
- Pages
- Stylus CSS preprocessor
- ejs HTML templates
- Standalone (single css file, no external file) 🥊
- Static (no js, one single css) 🍊
- Emoji Icons for blog posts ✨
- SVG for social icons (Twitter, StackOverflow, LinkedIn, Mastodon, Github, Flickr 📰)
- Rss Icon (can be disabled)

## External libraries used

- [tachyons](https://tachyons.io/) for Css Framework
- [SimpleIcons](https://simpleicons.org/) for brand icons

## Installation

### Install the theme

Install the theme by using:

```bash
npm i hexo-theme-mindyne --save
```

Then update your blog's main `_config.yml` to set the theme to `minidyne`:

i.e:

``` yaml
theme: minidyne
```

You'll also need the following hexo plugins for this theme to work.
Add them in the package.json (they should already be there, but just in case):

```json
"dependencies": {
    "hexo-generator-feed": "^3.0.0",
    "hexo-generator-index": "^2.0.0",
    "hexo-generator-tag": "^1.0.0",
    "hexo-renderer-ejs": "^1.0.0",
    "hexo-renderer-stylus": "^2.0.0",
  }
```

## Limitations

This theme does not handle:

- Categories (so you can drop the default dependency to "hexo-generator-category" )
- Archives (so you can drop the default dependency to "hexo-generator-archive". If you want archives, [head over to V1](https://github.com/tomap/hexo-theme-minidyne/tree/v1))
- Images gallery
- Pagination (if you want pagination, [head over to V1 branch](https://github.com/tomap/hexo-theme-minidyne/tree/v1))

## Post Configuration

Each post supports the standard `title`, `date`, `tags`.

### Post Icon

On top of that, you can specify an icon (ascii/unicode emoji):

Example:

``` yaml
title: Welcome to Minidyne
tags: ["ThisIsATag", "Intro", "Welcome", "Minidyne"]
icon: 🤝
---
```

Pick one from https://emojipedia.org/

## Theme Configuration

The theme's global configuration is done in the main `_config.yml` under the config key `theme_config`:

``` yaml
theme_config:
  default_post_title: "Untitled"
  # Header
  menu:
    Home: /
    About: /about.html
  
  # Index banner text
  index_banner_text: Welcome to Minidyne

  # Logo
  index_icon: ❤️

  default_post_title: "Untitled"

  default_post_icon: 🧙

  # Social Media Platforms, also used for comments
  social_platforms:
    - url: https://stackoverflow.com/users/12345/johndoe
      icon: stackoverflow
      name: Stack Overflow
    - url: https://github.com/johndoe/
      icon: github
      type: github
      name: GitHub
      repository: johndoe.blog
    - url: https://linkedin.com/in/johndoe
      icon: linkedin
      type: linkedin
      name: LinkedIn
    - url: https://twitter.com/johndoe
      icon: twitter
      type: twitter
      name: Twitter
      account: johndoe
    - url: https://www.flickr.com/photos/johndoe/
      icon: flickr
      type: flickr
      name: Flickr
    - url: https://mastodon.social/@johndoe
      icon: mastodon
      type: mastodon
      name: Mastodon
    - url: /rss2.xml
      icon: rss
      type: rss
      name: Rss
```

* `menu`: The object key is the label and the value is the path.
* `index_banner_text` The title appears on the home page.
* `index_icon` The icon should be an emoji. Pick one from https://emojipedia.org/
* `default_post_title` The default post title (used when no title is specified).
* `default_post_icon` The default post icon (used when no icon is specified) is configured in the main `_config.yml`.
* `social_platforms` Social Account: Setup the links to your social pages in the theme's `_config.yml` as an array of objects. Links are in the footer. They are used for sharing comments on your posts. Some need more properties than others

## Note

The devDependency in package.json is just here to know when there is an update for Tachyons

## Creator

This theme was created by [Thomas Piart](https://tpî.eu) initially based upon (Anodyne Theme)(https://github.com/klugjo/hexo-theme-anodyne) by [Jonathan Klughertz](http://www.codeblocq.com/) and also influenced by other minimalist approaches like [mnmlist](http://mnmlist.com/w/).

## Bugs

If you have a question, feature request or a bug you need me to fix, please [file an issue](https://github.com/tomap/hexo-theme-minidyne/issues/new).

## License

MIT
