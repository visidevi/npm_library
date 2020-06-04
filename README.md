# base

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
npx vue-cli-service build --target lib --name buttons src/index.js
```
### Bulid as npm lib
```
npx vue-cli-service build --target lib --name buttons src/index.js
```
### Bulid as npm lib
```
npm publish --access=public

npm install --save @dscns/buttons

```
import Vue from 'vue'
import App from './App.vue'
import '@company_name/components-lib/components-lib.css';
import * as ComponentsLib from '@company_name/components-lib';

Vue.config.productionTip = false

Vue.use({install: ComponentsLib.install});

new Vue({
  render: h => h(App)
}).$mount('#app')

<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <section>
      <button-component buttonText="Ejemplo de botón"/>
      <other-button-component buttonText="Ejemplo de botón"/>
      <button-group-component />
    </section>
  </div>
</template>


```
  "publishConfig": {
    "registry": "https://npm.pkg.github.com"
  },
   npm login --registry=https://npm.pkg.github.com --scope=@company_name
   crea token en github
   crear repo mismo nombre
   npm publish

```

<script>
export default {
  name: 'app'
}
</script>

See [Configuration Reference](https://www.paradigmadigital.com/dev/como-crear-libreria-componentes-vuejs/).
### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
