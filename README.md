# test-vue-firebase

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

##作業メモ

>firebase.jsonの編集またはfirebase initのhosting 設定

    "hosting": {
        "public": "dist",///////こ↑こ↓
        "ignore": [
            "firebase.json",
             "**/.*",
             "**/node_modules/**"
        ],
         "rewrites": [
             {
                 "source": "**",
                   "destination": "/index.html"
             }
         ]
     }

コーディング内で"public":"dist"とするかinitでのpublic設定？デプロイ設定？時にdistと打つ