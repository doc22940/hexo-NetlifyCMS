# Landscape

A brand new default theme for [Hexo](https://hexo.io/).

* [Preview](http://hexo.io/hexo-theme-landscape/)

## Installation

### Install

```bash
$ git clone https://github.com/hexojs/hexo-theme-landscape.git themes/landscape
```

**Landscape requires Hexo 2.4 and above.** If you would like to enable the RSS, the [hexo-generate-feed](https://github.com/hexojs/hexo-generator-feed) plugin is also required.

### Enable

Modify `theme` setting in `_config.yml` to `landscape`.

### Update

```bash
cd themes/landscape
git pull
```

## Configuration

```text
# Header
menu:
  Home: /
  Archives: /archives
rss: /atom.xml

# Content
excerpt_link: Read More
fancybox: true

# Sidebar
sidebar: right
widgets:
  - category
  - tag
  - tagcloud
  - archives
  - recent_posts

# Miscellaneous
google_analytics:
favicon: /favicon.png
twitter:
google_plus:
```

* **menu** - Navigation menu
* **rss** - RSS link
* **excerpt\_link** - "Read More" link at the bottom of excerpted articles. `false` to hide the link.
* **fancybox** - Enable [Fancybox](http://fancyapps.com/fancybox/)
* **sidebar** - Sidebar style. You can choose `left`, `right`, `bottom` or `false`.
* **widgets** - Widgets displaying in sidebar
* **google\_analytics** - Google Analytics ID
* **favicon** - Favicon path
* **twitter** - Twiiter ID
* **google\_plus** - Google+ ID

## Features

### Fancybox

Landscape uses [Fancybox](http://fancyapps.com/fancybox/) to showcase your photos. You can use Markdown syntax or fancybox tag plugin to add your photos.

```text
![img caption](img url)

{% fancybox img_url [img_thumbnail] [img_caption] %}
```

### Sidebar

You can put your sidebar in left side, right side or bottom of your site by editing `sidebar` setting.

Landscape provides 5 built-in widgets:

* category
* tag
* tagcloud
* archives
* recent\_posts

All of them are enabled by default. You can edit them in `widget` setting.

## Development

### Requirements

* [Grunt](http://gruntjs.com/) 0.4+
* Hexo 2.4+

### Grunt tasks

* **default** - Download [Fancybox](http://fancyapps.com/fancybox/) and [Font Awesome](http://fontawesome.io/).
* **fontawesome** - Only download [Font Awesome](http://fontawesome.io/).
* **fancybox** - Only download [Fancybox](http://fancyapps.com/fancybox/).
* **clean** - Clean temporarily files and downloaded files.

