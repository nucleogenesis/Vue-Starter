# oomba-to

> Oomba tournament organizer Vue app.

## Oomba Web Team Vue Projects

### Folder Structure

_api_ - Holds code specifically for making API requests.
_build_ - Houses build-related configurations.
_config_ - Houses environmental configurations.
_dist_ - Your compiled Vue application (what would be served to an actual end-user).
_node_modules_ - Duh.
_src_ - All Vue source files, including CSS and other assets.
_static_ - Holds static assets.
_test_ - Where we keep our testing

#### The `src` Folder In Detail

_assets_ - Keeps our assets, particularly images, which are not otherwise provided by the backend such as logo, icons, etc.

_router_ - Keeps the router file. The `index.js` file here is where we can define our routes and the components that go along with them.

_store_ - This stores all code for Vuex and state management. We expect to manage larger state containers in individual `stores` as modules. Modules are then compiled into the greater global store so that we can have code separation for individual responsibilities. See https://vuex.vuejs.org/en/modules.html and the greater Vuex documentation for more information.

_components_ - Each component is a single `.vue` file. That files houses the `<template>` - an HTML-like template relatively similar to Angular's. There is the `<script>` section, where the JS wizardy ensues. Then there is the `<style>` section, where you add CSS. For components with very large templates, we may consider extracting components into an Angular-esque folder structure in which we house a template (aka `.vue`) file, JS file and CSS file together, but in Vue, this requires that we have our `.vue` file which pulls in the JS and CSS file.

_App.vue_ - This is the root component of our project. This is what we mount into the `index.html` file in the root of the project that makes our Vue project live.

#### index.html in the Root Directory

If you ever need to do something like add things between the `<head>` tags in the actual HTML document, you can do that here.

Otherwise, this file shouldn't be touched much at all.

#### Testing

There is currently _no test framework_ setup in the app. We should discuss what we would like to use for testing on both the e2e side and the unit testing side and what level of test coverage we expect on a component level or beyond. From there, we can decide on our frameworks and detail our team-level expectations.

## Build Setup

```bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```
