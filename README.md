# vue-component-package-demo

## Use in browser
```
<script src="https://unpkg.com/vue-component-package-demo/dist/vue-component-package-demo.umd.js"></script>
```

## Project create
```
vue create .
vue add vuetify
```

vue.config.js： `css: { extract: false } // 强制CSS内联`

'src/index.js'

package.json
```
{
  "name": "vue-component-package-demo",
  "version": "0.1.0",
  "description": "vue component package demo",
  // The files hosted by NPM
  "files": [
    "dist/*",
    "src/*",
    "*.json"
  ],
  "main": "dist/vue-component-package-demo.common.js",
  "scripts": {
    "serve": "vue-cli-service serve",
    "build-package": "vue-cli-service build --target lib --inline-vue --name vue-component-demo ./src/index.js",
    "build": "vue-cli-service build",
    "lint": "vue-cli-service lint"
  },
}
```

## Publish to NPM

npm login
npm publish

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

### Build package
```
npm run build-package
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
