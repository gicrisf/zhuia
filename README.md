# Zhuia

An elegant theme for [Zola](https://getzola.org/) powered by [Spectre.css](https://picturepan2.github.io/spectre/) with (almost) no JavaScript (a small script runs the beautiful hamburger menu overlay: that's it!)

**DEMO**: [https://zhuia.netlify.app/](https://zhuia.netlify.app/)

---

## Contents

- [Installation](#installation)
- [Options](#options)
  - [Title](#title)
  - [SEO](#seo)
  - [Social](#social)
  - [Footer](#footer)
- [Name](#name)
- [Genesis](#genesis)
- [License](#license)


## Installation

First download this theme to your `themes` directory:

```bash
$ cd themes
$ git clone https://github.com/gicrisf/zhuia.git
```
and then enable it in your `config.toml`:

```toml
theme = "zhuia"
```

Posts should be placed directly in the `content` folder.

To sort the post index by date, enable sort in your index section `content/_index.md`:

```toml
sort_by = "date"
```

## Options

### Title

Set a title and description in the config to appear in the site header and on the RSS feed:

```toml
title = "Der Prozess"
description = "a novel written by Franz Kafka in 1914"
```

### SEO

Most SEO tags are populated by the page metadata, but you can set the `author` and for the `og:image` tag provide the path to an image:

```toml
[extra]

author = "Timothy Morton"
og_image = "Hyperobjects.png"
```

### Social

Set a field in `extra` with a key of `footer_links`:

```toml
[extra]

# Freely comment out or delete every field
social_links = [
    {url = "https://t.me/yourname", name = "telegram"},
    # {url = "https://facebook.com/yourname", name = "facebook"},
    {url = "https://twitter.com/yourname", name = "twitter"},
    # {url = "", name = "instagram"},
    {url = "https://github.com/gicrisf", name = "github"},
]
```

### Footer

You can add your own copyright or whatever to the footer with a through a simple option on the config file:

```toml
[extra]

footer_tagline = "What if everything is an illusion and nothing exists? In that case, I definitely overpaid for my carpet."
```

## Name

The name arise from two parts:
- The generator, Zola, gives the "Z";
- An extinct species of New Zealand wattlebird, the huia, provide the second part.

The theme is built on Spectre CSS framework, so I found reasonable evoking a spectral species.

## Genesis

This theme is based on a Pelican theme I originally made for my blog, which was in turn based on the 
Grav theme [Quark](https://github.com/getgrav/grav-theme-quark).

## License

Open sourced under the [MIT license](LICENSE.md).
