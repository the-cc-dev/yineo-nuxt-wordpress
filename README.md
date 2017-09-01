# Example consumer with Nuxt.js / Vue.js and public wordpress API

This was the consumer for yineo.fr until august 2017. 
yineo.fr will soon using a graphQL API backed by Drupal 8 : https://github.com/nyl-auster/yineo-front
But i keep this repo for interested wordpress people.
Wordpress JSON API is great, I only regret that this is quite slow ( 600ms or > ) for now.
That's why this repo include a simple proxy to cache responses.
You can see cache stats at api/cache and flush going to api/cache/flush

## Build Setup

``` bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, checkout the [Nuxt.js docs](https://github.com/nuxt/nuxt.js).
