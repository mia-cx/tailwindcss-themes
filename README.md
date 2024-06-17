# @mia-cx/tailwindcss-themes

A Tailwind plugin for theming. Provide media queries and/or multiple selectors, and variants for each theme will be generated!

## Getting Started

```sh
pnpm i -D @mia-cx/tailwindcss-themes
```

```js
// tailwind.config.js
const themes = require('@mia-cx/tailwindcss-themes');

module.exports = {
  // ...
  plugins: [
    // ...
    themes({
      themes: {
        light: {
          selectors: '.light',
        },
        dark: {
          selectors: '.dark',
        },
      },
      baseSelector: ':root',
      fallback: 'dark',
    }),
  ],
  // ...
};
```

## To Do

- [ ] Add auto-generated utilities based on each theme's `theme` definition.
