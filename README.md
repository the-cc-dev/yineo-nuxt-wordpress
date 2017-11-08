# Example consumer with Nuxt.js / Vue.js and public wordpress API

This is the consumer for https://yineo.fr, using wordpress.com public API.
Wordpress public JSON API is great but is quite slow ( 600ms or > ) for now.
That's why this repo include a simple proxy to cache responses.
You can see cache stats at api/cache

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
