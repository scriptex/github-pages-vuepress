[![Travis CI](https://travis-ci.com/scriptex/github-pages-vuepress.svg?branch=master)](https://travis-ci.com/scriptex/github-pages-vuepress)
[![Github Build](https://github.com/scriptex/github-pages-vuepress/workflows/Build/badge.svg)](https://github.com/scriptex/github-pages-vuepress/actions?query=workflow%3ABuild)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/34d3d75710534dc6a38c3584a1dcd068)](https://www.codacy.com/gh/scriptex/github-pages-vuepress/dashboard?utm_source=github.com&utm_medium=referral&utm_content=scriptex/github-pages-vuepress&utm_campaign=Badge_Grade)
[![Codebeat Badge](https://codebeat.co/badges/d765a4c8-2c0e-44f2-89c3-fa364fdc14e6)](https://codebeat.co/projects/github-com-scriptex-github-pages-vuepress-master)
[![CodeFactor Badge](https://www.codefactor.io/repository/github/scriptex/github-pages-vuepress/badge)](https://www.codefactor.io/repository/github/scriptex/github-pages-vuepress)
[![DeepScan grade](https://deepscan.io/api/teams/3574/projects/5257/branches/40799/badge/grade.svg)](https://deepscan.io/dashboard#view=project&tid=3574&pid=5257&bid=40799)
[![Analytics](https://ga-beacon-361907.ew.r.appspot.com/UA-83446952-1/github.com/scriptex/github-pages-vuepress/README.md?pixel)](https://github.com/scriptex/github-pages-vuepress/)

# VuePress Github Pages

> Use [VuePress](https://vuepress.vuejs.org/) to built a static website and deploy on [Github Pages](https://pages.github.com/).

## Visitor stats

![GitHub stars](https://img.shields.io/github/stars/scriptex/github-pages-vuepress?style=social)
![GitHub forks](https://img.shields.io/github/forks/scriptex/github-pages-vuepress?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/scriptex/github-pages-vuepress?style=social)
![GitHub followers](https://img.shields.io/github/followers/scriptex?style=social)

## Code stats

![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/scriptex/github-pages-vuepress)
![GitHub repo size](https://img.shields.io/github/repo-size/scriptex/github-pages-vuepress?style=plastic)
![GitHub language count](https://img.shields.io/github/languages/count/scriptex/github-pages-vuepress?style=plastic)
![GitHub top language](https://img.shields.io/github/languages/top/scriptex/github-pages-vuepress?style=plastic)
![GitHub last commit](https://img.shields.io/github/last-commit/scriptex/github-pages-vuepress?style=plastic)

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

## LICENSE

MIT

---

<div align="center">
    Connect with me:
</div>

<br />

<div align="center">
    <a href="https://atanas.info">
        <img src="https://raw.githubusercontent.com/scriptex/socials/master/styled-assets/logo.svg" height="20" alt="">
    </a>
    &nbsp;
    <a href="mailto:hi@atanas.info">
        <img src="https://raw.githubusercontent.com/scriptex/socials/master/styled-assets/email.svg" height="20" alt="">
    </a>
    &nbsp;
    <a href="https://www.linkedin.com/in/scriptex/">
        <img src="https://raw.githubusercontent.com/scriptex/socials/master/styled-assets/linkedin.svg" height="20" alt="">
    </a>
    &nbsp;
    <a href="https://github.com/scriptex">
        <img src="https://raw.githubusercontent.com/scriptex/socials/master/styled-assets/github.svg" height="20" alt="">
    </a>
    &nbsp;
    <a href="https://gitlab.com/scriptex">
        <img src="https://raw.githubusercontent.com/scriptex/socials/master/styled-assets/gitlab.svg" height="20" alt="">
    </a>
    &nbsp;
    <a href="https://twitter.com/scriptexbg">
        <img src="https://raw.githubusercontent.com/scriptex/socials/master/styled-assets/twitter.svg" height="20" alt="">
    </a>
    &nbsp;
    <a href="https://www.npmjs.com/~scriptex">
        <img src="https://raw.githubusercontent.com/scriptex/socials/master/styled-assets/npm.svg" height="20" alt="">
    </a>
    &nbsp;
    <a href="https://www.youtube.com/user/scriptex">
        <img src="https://raw.githubusercontent.com/scriptex/socials/master/styled-assets/youtube.svg" height="20" alt="">
    </a>
    &nbsp;
    <a href="https://stackoverflow.com/users/4140082/atanas-atanasov">
        <img src="https://raw.githubusercontent.com/scriptex/socials/master/styled-assets/stackoverflow.svg" height="20" alt="">
    </a>
    &nbsp;
    <a href="https://codepen.io/scriptex/">
        <img src="https://raw.githubusercontent.com/scriptex/socials/master/styled-assets/codepen.svg" width="20" alt="">
    </a>
    &nbsp;
    <a href="https://profile.codersrank.io/user/scriptex">
        <img src="https://raw.githubusercontent.com/scriptex/socials/master/styled-assets/codersrank.svg" height="20" alt="">
    </a>
    &nbsp;
    <a href="https://linktr.ee/scriptex">
        <img src="https://raw.githubusercontent.com/scriptex/socials/master/styled-assets/linktree.svg" height="20" alt="">
    </a>
</div>

---

<div align="center">
Support and sponsor my work:
<br />
<br />
<a href="https://twitter.com/intent/tweet?text=Checkout%20this%20awesome%20developer%20profile%3A&url=https%3A%2F%2Fgithub.com%2Fscriptex&via=scriptexbg&hashtags=software%2Cgithub%2Ccode%2Cawesome" title="Tweet">
	<img src="https://img.shields.io/badge/Tweet-Share_my_profile-blue.svg?logo=twitter&color=38A1F3" />
</a>
<a href="https://paypal.me/scriptex" title="Donate on Paypal">
	<img src="https://img.shields.io/badge/Donate-Support_me_on_PayPal-blue.svg?logo=paypal&color=222d65" />
</a>
<a href="https://revolut.me/scriptex" title="Donate on Revolut">
	<img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/scriptex/scriptex/master/badges/revolut.json" />
</a>
<a href="https://patreon.com/atanas" title="Become a Patron">
	<img src="https://img.shields.io/badge/Become_Patron-Support_me_on_Patreon-blue.svg?logo=patreon&color=e64413" />
</a>
<a href="https://ko-fi.com/scriptex" title="Buy Me A Coffee">
	<img src="https://img.shields.io/badge/Donate-Buy%20me%20a%20coffee-yellow.svg?logo=ko-fi" />
</a>
<a href="https://liberapay.com/scriptex/donate" title="Donate on Liberapay">
	<img src="https://img.shields.io/liberapay/receives/scriptex?label=Donate%20on%20Liberapay&logo=liberapay" />
</a>

<a href="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/scriptex/scriptex/master/badges/bitcoin.json" title="Donate Bitcoin">
	<img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/scriptex/scriptex/master/badges/bitcoin.json" />
</a>
<a href="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/scriptex/scriptex/master/badges/etherium.json" title="Donate Etherium">
	<img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/scriptex/scriptex/master/badges/etherium.json" />
</a>
<a href="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/scriptex/scriptex/master/badges/shiba-inu.json" title="Donate Shiba Inu">
	<img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/scriptex/scriptex/master/badges/shiba-inu.json" />
</a>
</div>
