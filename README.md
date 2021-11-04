# 🛢 Auroraswap UIkit

<!-- [![Version](https://img.shields.io/npm/v/@auroraswap-libs/uikit)](https://www.npmjs.com/package/@auroraswap-libs/uikit) [![Size](https://img.shields.io/bundlephobia/min/@auroraswap-libs/uikit)](https://www.npmjs.com/package/@auroraswap-libs/uikit) -->

Auroraswap UIkit is a set of React components and hooks used to build pages on Auroraswap's apps. It also contains a theme file for dark and light mode.

## Install

`npm i auroraswap-uikit`

## Setup

### Theme

Before using Auroraswap UIkit, you need to provide the theme file to styled-component.

```
import { ThemeProvider } from 'styled-components'
import { light, dark } from 'auroraswap-uikit'
...
<ThemeProvider theme={isDark}>...</ThemeProvider>
```

### Reset

A reset CSS is available as a global styled component.

```
import { ResetCSS } from 'auroraswap-uikit'
...
<ResetCSS />
```

### Types

This project is built with Typescript and export all the relevant types.

## How to use the UIkit

If you want to use components from the UIkit, check the [Storybook documentation](https://auroraswap.github.io/pancake-uikit/)

## How to Customize UIkit

First clone this repo to local and then start editing the components, theme, etc.

When is finished the Customization of the UIkit build it using:

`npm run build`

Commit everything to the git repo and if you are using a diferent repo just change it in package.json.

If you have a commit error due to husky you can try:

`git commit -am 'commit' --no-verify`

That should solve the problem, then push to remote repo.

After this you need to [publish the npm packege](https://zellwk.com/blog/publish-to-npm/)

Be aware of the versions, If you make an update change the version in package.json so when you publish this's not gonna throw you an error.

Go to the npm package you create an you are ready to use it.
