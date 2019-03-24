# saber-theme-minima

> A Saber Port of the Default Jekyll Theme: Minima

## Install

```bash
yarn add sass sass-loader saber-theme-minima
```

In your `saber-config.yml`:

```yml
theme: minima
```

This theme is better working with following plugins:

- `saber-plugin-query-posts`: Inject `posts` to homepage's `page` prop, generate tag pages
- `saber-plugin-generate-feed`: Generate JSON feed at `/feed.json`.

```bash
yarn add saber-plugin-query-posts saber-plugin-generate-feed
```

```yml
plugins:
  - resolve: saber-plugin-query-posts
  - resolve: saber-plugin-generate-feed
```

## Site Config

Configure site title, description etc in your `saber-config.yml`:

```yml
siteConfig:
  title: My Site
  description: About this website..
  author: My Name
  email: my@email.com
```

## Theme Config

### Navbar

Configure `nav` to show a set of links in header:

```yml
themeConfig:
  nav:
    - text: Home
      link: /
    - text: About
      link: /about.html
```

### Social

Configure the accounts of your social network to show at the bottom of homepage:

```yml
themeConfig:
  social:
    dribbble: username
    facebook: username
    flickr: username
    github: username
    instagram: username
    linkedin: username
    pinterest: username
    twitter: username
    youtube: username
    telegram: username
    microdotblog: username
    googleplus: username
    rss: true
```

### Comments

You can use Disqus:

```yml
themeConfig:
  disqus: disqus-short-name
```

Comments are only enabled for `post` layout, to disable comments in specific page, you can use the page attribute `comments`:

```markdown
---
title: Hello
layout: post
date: 2018-08-12
comments: false
---

Hello World!
```

## License

MIT.