---
title: Graphics Drivers
description: ''
position: 2
category: Resources
---

Check this [PC Gamer](https://www.pcgamer.com/how-to-update-drivers/) article for more information about installing and updating graphics cards drivers. Below are instructions that should work for any windows system.

## AMD GPU

Add `@nuxtjs/xxx` dependency to your project:

<code-group>
  <code-block label="Yarn" active>

  ```bash
  yarn add @nuxtjs/xxx
  ```

  </code-block>
  <code-block label="NPM">

  ```bash
  npm install @nuxtjs/xxx
  ```

  </code-block>
</code-group>

Then, add `@nuxtjs/xxx` to the `modules` section of `nuxt.config.js`:

```js[nuxt.config.js]
{
  modules: [
    '@nuxtjs/xxx'
  ],
  xxx: {
    // Options
  }
}
```

## Nvidia GPU
