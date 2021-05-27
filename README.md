[![GitHub issues](https://img.shields.io/github/issues/scriptex/github-pages-vuepress.svg)](https://github.com/scriptex/github-pages-vuepress/issues)
[![GitHub last commit](https://img.shields.io/github/last-commit/scriptex/github-pages-vuepress.svg)](https://github.com/scriptex/github-pages-vuepress/commits/master)
[![Build Status](https://travis-ci.com/scriptex/github-pages-vuepress.svg?branch=master)](https://travis-ci.com/scriptex/github-pages-vuepress)
[![Analytics](https://ga-beacon.appspot.com/UA-83446952-1/github.com/scriptex/github-pages-vuepress/README.md)](https://github.com/scriptex/github-pages-vuepress/)

# VuePress Github Pages

Use [VuePress](https://vuepress.vuejs.org/) to built a static website and deploy on [Github Pages](https://pages.github.com/).

## Start

Make sure that you have NodeJS and NPM or Yarn installed.

Start by forking or downloading this repository. If downloaded, extract the contents of the archive in a folder and navigate to that folder in your preferred terminal. Then:

## Install

```sh
npm install
```

or

```sh
yarn
```

## Develop

```sh
npm run start
```

or

```sh
yarn start
```

## Build

```sh
npm run build
```

or

```sh
yarn build
```

## Details

The `README.md` file in the root serves the purpose of `index.html` file.

If you wish to create new pages, you can do so by adding new `.md` files in the root.

If you wish to use a more complicated files/folders structure, make sure that you read and follow the [official docs](https://vuepress.vuejs.org/guide/directory-structure.html#default-page-routing) or just checkout how I did it in the [demo branch](https://github.com/scriptex/github-pages-vuepress/tree/demo)

VuePress builds your static website in the `/docs` folder which is set to be used by Github Pages in the repository settings.

**Important**

You can control the base dir of your site in the `.vuepress/config.js` file's `base` property.

## Demo

See this page served via Gitlab Pages on https://scriptex.js.org/github-pages-vuepress/

## Bonus: Theming

Vuepress uses [Stylus](http://stylus-lang.com/). It comes with default theme which can be easily overwritten.
Just place your styles in the `.vuepress/styles` folder.

Here are the **default theme** colors. Variables should go in the `palette.styl` file:

```stylus
$accentColor = #3eaf7c
$textColor = #2c3e50
$borderColor = #eaecef
$codeBgColor = #282c34
```

Here are the colors and settings for a **Material Light** theme:

Variables should go in the `palette.styl` file:

```stylus
$accentColor = #009688
$textColor = #212121
$borderColor = #bdbdbd
$codeBgColor = #333
$bgColor = #fff
```

The rest of the styles should go in the `index.styl` file:

```stylus
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
/* .vuepress/styles/palette.styl */
$accentColor = #ef4c23
$textColor = #fff
$borderColor = #bdbdbd
$codeBgColor = #000
$bgColor = #263238

/* .vuepress/styles/index.styl */
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

## Support this project

[![Tweet](https://img.shields.io/badge/Tweet-Share_this_repository-blue.svg?style=flat-square&logo=twitter&color=38A1F3)](https://twitter.com/intent/tweet?text=Checkout%20this%20awesome%20software%20project%3A&url=https%3A%2F%2Fgithub.com%2Fscriptex%2Fgithub-pages-vuepress&via=scriptexbg&hashtags=software%2Cgithub%2Ccode%2Cawesome)
[![Donate](https://img.shields.io/badge/Donate-Support_me_on_PayPal-blue.svg?style=flat-square&logo=paypal&color=222d65)](https://www.paypal.me/scriptex)
[![Become a Patron](https://img.shields.io/badge/Become_Patron-Support_me_on_Patreon-blue.svg?style=flat-square&logo=patreon&color=e64413)](https://www.patreon.com/atanas)

## LICENSE

MIT
