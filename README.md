<h1 align="center">skeleton-web-stack</h1>

<h3 align="center">Pick a web stack. Start your project.</h4>
<br>

This repository contains multiple branches. Each one contains a minimal project for a given web stack. The idea is to provide a good skeleton on which you can build your own projects.

The `main` branch only contains this `README.md` with a description of other branches.

## How it works

Simply checkout the branch that contains the web stack you are insterested in. Each branch should have its own `README.md` that describes how to use the specific web stack but also how to create it from scratch.

When switching branches make sure to reset and clean your working directory. This will remove project specific caches like `.yarn/`, `node_modules`, etc. ensuring you start fresh each time.

```sh
git checkout <branch>
git reset --hard
git clean -fdx
```

# Pick a stack

* `yarn2-parcel2-vue3` - Minimal project using [Yarn 2](https://yarnpkg.com/), [Parcel 2](https://parceljs.org/) and [Vue 3](https://v3.vuejs.org/). Benefits include asset bundling, tree shaking and .vue files - [Single File Components](https://v3.vuejs.org/guide/single-file-component.html) with very little configuration.
