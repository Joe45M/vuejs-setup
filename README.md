# Install Vue CLI

If not installed already:

> npm install -g @vue/cli

OR

> yarn global add @vue/cli

To use vue Router:

> vue add router

## Global SCSS Injection

Useful for global styles, Bootstrap CSS for example. **NOTE** : Preprocessors must be enabled. 

> npm i node-sass sass-loader

OR

> yarn add node-sass sass-loader

Then, create a `vue.config.js` file at project root, containing:

```javascript
module.exports = {
  css: {
    loaderOptions: {
      sass: {
        prependData: `@import "@/styles/_variables.scss";`
      }
    }
  }
};
```

NOTE: `@` is an alias to the assets directory.

More on global injection: https://css-tricks.com/how-to-import-a-sass-file-into-every-vue-component-in-an-app/


## Useful VueJS tools

VueJS carousel    - https://ssense.github.io/vue-carousel/

VueJS Lottie Wrap - https://www.npmjs.com/package/lottie-vuejs
