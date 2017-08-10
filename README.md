Simple
======

A simple, blog-based theme for [Hugo](https://gohugo.io).

## Installation

You can install the theme either as a clone or submodule.

I recommend the latter. From the root of your Hugo site, type the following:

```bash
$ git submodule add https://github.com/aisola/hugo-simple.git themes/simple
$ git submodule init
$ git submodule update
```

Now you can get updates to Simple in the future by updating the submodule:

```bash
$ git submodule update --remote themes/simple
```

## Configuration

After installation, take a look at the `exampleSite` folder inside `themes/simple`.

To get started, copy the `config.toml` file inside `exampleSite` to the root of your Hugo site:

```bash
$ cp themes/simple/exampleSite/config.toml .
```

Now edit this file and add your own information. Note that some fields can be ommited.

I recommend you use the theme's archetypes so now delete your site's `archetypes/default.md`.

## Features

You can tweak the look of the theme to suit your needs in a number of ways:

- The accent color can be changed by using the `accent` field in `config.toml`.

- You can change the text color for text in accented areas by setting accentText.

For best results, I recommend you use a dark accent color with a light background, for example:

```toml
[params]
    accent = "#ffffff"
    accentText = "#000000"
```

### Fonts

The theme uses [Google Fonts](https://fonts.google.com) to load its font. To change the font:

```toml
[params]
    font = "Open Sans" # should match the name on Google Fonts!
```

### Syntax highlighting

The theme supports syntax highlighting thanks to [Prism](http://prismjs.com/). In order to activate highlighting be 
sure to set a language in your code blocks.


### SEO

Simple has Open Graph, Twitter, and Schema.org markup.

### Disqus Comments support

To activate [Disqus comments](https://disqus.com/), uncomment the `disqusShortname` parameter in your config.toml and
set it to your assigned Disqus shortname.
