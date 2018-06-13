# VuePress Github Pages

Use [VuePress](https://vuepress.vuejs.org/) to built a static website and deploy on [Github Pages](https://pages.github.com/).

## Install

```javascript
npm install
```

or

```javascript
yarn;
```

## Develop

```javascript
npm run start
```

or

```javascript
yarn start
```

## Build

```javascript
npm run start
```

or

```javascript
yarn start
```

## Details

The `README.md` file in the root server the purpose of `index.html` file.

If you wish to create new pages, you can do so by adding new `.md` files in the root.

If you wish to use a more complicated files/folders structure, make sure that you read and follow the reference in https://vuepress.vuejs.org/

## Demo

See this page server via Gitlab Pages on ...

## Deployment Info

1. Create a new personal access token from https://github.com/settings/tokens/new

    * set the name of the token
    * select `public_repo` checkbox

2. On the Travis settings for the repository https://travis-ci.org/<me>/<myrepo>/settings create an environment variable:

```
GITHUB_API_KEY=<token>
```

**!Important**

Mark _Display value in build log_ as _Off_

3. Add the following to your `.travis.yml` file

```
after_success: |
  if [ -n "$GITHUB_API_KEY" ]; then
    cd "$TRAVIS_BUILD_DIR"
    # This generates a `web` directory containing the website.
    make web
    cd web
    git init
    git checkout -b gh-pages
    git add .
    git -c user.name='travis' -c user.email='travis' commit -m init
    # Make sure to make the output quiet, or else the API token will leak!
    # This works because the API key can replace your password.
    git push -f -q https://<me>:$GITHUB_API_KEY@github.com/<me>/<myrepo>-gh-pages gh-pages &2>/dev/null
    cd "$TRAVIS_BUILD_DIR"
  fi
```

## LICENSE

MIT
