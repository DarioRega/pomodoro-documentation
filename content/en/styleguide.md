---
title: Frontend
description: 'Storybook styleguide for Pomodoro application'
position: 1
---

Styleguide production: [Pomodoro Styleguide](https://styleguide.pomodoro.seelo.ch)  
This styleguide is made with [Storybook](https://storybook.js.org/)

  
##  Installation

  ```bash
  git clone git@gitlab.com:seelo/pomodoro/styleguide.git
  cd ./styleguide
  yarn install
  cp .env.example .env
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
yarn release
```


## Commands

### Compiles and hot-reloads for development

```bash
yarn start
```

### Compiles and minifies for production

```bash 
yarn run build
```

### Lints and fixes files

```bash
yarn run lint
```


