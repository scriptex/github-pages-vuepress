[![GitHub stars](https://img.shields.io/github/stars/scriptex/github-pages-vuepress.svg?style=social&label=Stars)](https://github.com/scriptex/github-pages-vuepress)
[![GitHub forks](https://img.shields.io/github/forks/scriptex/github-pages-vuepress.svg?style=social&label=Fork)](https://github.com/scriptex/github-pages-vuepress/network#fork-destination-box)
[![GitHub issues](https://img.shields.io/github/issues/scriptex/github-pages-vuepress.svg)](https://github.com/scriptex/github-pages-vuepress/issues)
[![GitHub last commit](https://img.shields.io/github/last-commit/scriptex/github-pages-vuepress.svg)](https://github.com/scriptex/github-pages-vuepress/commits/master)
[![Build Status](https://travis-ci.org/scriptex/github-pages-vuepress.svg?branch=master)](https://travis-ci.org/scriptex/github-pages-vuepress)
[![license](https://img.shields.io/github/license/scriptex/github-pages-vuepress.svg)](https://github.com/scriptex/github-pages-vuepress)
[![Analytics](https://ga-beacon.appspot.com/UA-83446952-1/github.com/scriptex/github-pages-vuepress/README.md)](https://github.com/scriptex/github-pages-vuepress/)
[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/scriptex/github-pages-vuepress/)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/scriptex/github-pages-vuepress/graphs/commit-activity) [![Greenkeeper badge](https://badges.greenkeeper.io/scriptex/github-pages-vuepress.svg)](https://greenkeeper.io/)

# VuePress Github Pages

Use [VuePress](https://vuepress.vuejs.org/) to built a static website and deploy on [Github Pages](https://pages.github.com/).

## Start

Make sure that you have NodeJS and NPM or Yarn installed.

Start by forking or downloading this repository. If downloaded, extract the contents of the archive in a folder and navigate to that folder in your preferred terminal. Then:

## Install

```console
npm install
```

or

```console
yarn
```

## Develop

```console
npm run start
```

or

```console
yarn start
```

## Build

```console
npm run build
```

or

```console
yarn build
```

## Details

The `README.md` file in the root serves the purpose of `index.html` file.

If you wish to create new pages, you can do so by adding new `.md` files in the root.

If you wish to use a more complicated files/folders structure, make sure that you read and follow the [VuePress usage reference](https://vuepress.vuejs.org/).

VuePress builds your static website in the `/docs` folder which is set to be used by Github Pages in the repository settings.

## Demo

See this page server via Gitlab Pages on https://scriptex.github.io/github-pages-vuepress/

## Bonus: Theming

Vuepress uses [Stylus](http://stylus-lang.com/). It comes with default theme which can be easily overwritten.
Just place your styles in the `override.styl` file in the `.vuepress` folder.

Here are the **default theme** colors:

```stylus
$accentColor = #3eaf7c
$textColor = #2c3e50
$borderColor = #eaecef
$codeBgColor = #282c34
```

Here are the colors and settings for a **Material Light** theme:

```stylus
$accentColor = #009688
$textColor = #212121
$borderColor = #bdbdbd
$codeBgColor = #333
$bgColor = #fff

html,
body,
.navbar,
.sidebar,
.theme-container .navbar,
.theme-container .sidebar
	background-color $bgColor

.theme-container .search-box input
	color $codeBgColor

.theme-container .search-box .suggestion a
	color $accentColor

.theme-container .content code
	color $bgColor
	background-color $codeBgColor
```

Here are the color for a **Material Dark** theme (used in my personal website):

```stylus
$accentColor = #ef4c23
$textColor = #fff
$borderColor = #bdbdbd
$codeBgColor = #000
$bgColor = #263238

html,
body,
.navbar,
.sidebar,
.theme-container .navbar,
.theme-container .sidebar
	background-color $bgColor

.theme-container .search-box input
	color: $codeBgColor

.theme-container .search-box .suggestion a
	color: $accentColor

.theme-container .content code
	background-color $codeBgColor
```

## LICENSE

MIT
