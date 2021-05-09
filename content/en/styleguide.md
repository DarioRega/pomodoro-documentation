---
title: Styleguide
description: 'Storybook styleguide for Pomodoro application'
position: 1
---

This styleguide is made with [Storybook ](https://storybook.js.org/)

  
##  Installation

  ```bash
  git clone git@gitlab.com:seelo/pomodoro/styleguide.git
  cd ./styleguide
  npm install
  ```

## Release

To release we use the package
[release-it](https://github.com/release-it/release-it)
This package is going read the commit history and write in the changelog
using the conventions of Eslint

### Release config
You can find the configuration file here: `.release-it.json`

### Release command
```bash
npm run release
```


## Commands

### Compiles and hot-reloads for development

```bash
npm start
```

### Compiles and minifies for production

```bash 
npm run build
```

### Lints and fixes files

```bash
npm run lint
```


