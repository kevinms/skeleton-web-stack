# yarn2-parcel2-vue3

Minimal project using [Yarn 2](https://yarnpkg.com/), [Parcel 2](https://parceljs.org/) and [Vue 3](https://v3.vuejs.org/).

Benefits:
- `.vue` files - [Single File Components](https://v3.vuejs.org/guide/single-file-component.html)
- Asset bundling
- Tree shaking

Make sure you have both [Node.js](https://nodejs.org/) and [yarn](https://yarnpkg.com/) installed.

Debian/Ubuntu systems:
```sh
sudo apt install nodejs
npm install -g yarn
```

## Usage

Install project dependencies:

```sh
yarn install
```

Run a development server:
```
yarn run start
```

Build production files (output located in `dist/`):
```
yarn run build
```

---

## How this project was created

```sh
mkdir skeleton-web
cd skeleton-web
git init
yarn set version berry # Use Yarn 2
yarn init
yarn add -D parcel@nightly vue@next @babel/core
mkdir src
```


Currently, `parcel@nightly` and `vue@next` are needed to support [SFCs](https://v3.vuejs.org/guide/single-file-component.html) (`.vue` files).

Add script commands to `package.json`:

```
{
  ...

  "scripts": {
    "start": "parcel serve ./src/index.html",
    "build": "parcel build ./src/index.html"
  },

  ...
}
```

Create a basic Vue 3 app in `src/`. An example can be found in the [parcel docs](https://v2.parceljs.org/languages/vue/).

Add a basic .gitignore file:

```
# Vim
*.sw[op]

# Yarn: not using Zero-Installs
.yarn/*
!.yarn/releases
!.yarn/plugins
!.yarn/sdks
!.yarn/versions
.pnp.*

# Parcel
.parcel-cache/
dist/
```