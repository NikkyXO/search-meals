# Vue 3 + Vite

This template should help get you started developing with Vue 3 in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

## Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).



## Tutorial 1: https://www.youtube.com/watch?v=cfiN8lCA3RM

### To initialize vue project
npm  create vite@latest


Reference: [tailwindcss.com/docs/guides/vite#vue](https://tailwindcss.com/docs/guides/vite#vue)

### To install tailwind css
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p


### Install vue Router latest version

npm install vue-router@next

### install vuex
npm install vuex@4 -S

### install tailwindcss forms
Reference: https://github.com/tailwindlabs/tailwindcss-forms
npm install -D @tailwindcss/forms

Then add the plugin to your tailwind.config.js file:

// tailwind.config.js
module.exports = {
  theme: {
    // ...
  },
  plugins: [
    require('@tailwindcss/forms'),
    // ...
  ],
}

### install axios for makin api calls
npm i -S axios

### source api to use (themealdb.com/api.php)
www.themealdb.com/api/json/v1/1/list.php?c=list
www.themealdb.com/api/json/v1/1/list.php?a=list
www.themealdb.com/api/json/v1/1/list.php?i=list