---
title: Graphics Drivers
description: ''
position: 2
category: Resources
---

Check this [PC Gamer](https://www.pcgamer.com/how-to-update-drivers/) article for more information about installing and updating graphics cards drivers. Below are instructions that should work for any Windows system.

## AMD GPU

Visit AMD's [driver page](https://www.amd.com/en/support), select your graphics card, and update your drivers to the latest version. This may allow you to use the _Vulkan_ engine, which some report has better performance on AMD graphics cards than *OpenGL*.

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

Visit Nvidia's [driver page](https://www.nvidia.com/Download/index.aspx), select your graphics card, and update your drivers to the latest version.

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