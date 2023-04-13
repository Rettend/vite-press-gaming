# Theming

## Theme Resolving

You can enable a custom theme by creating a `.vitepress/theme/index.js` or `.vitepress/theme/index.ts` file (the "theme entry file"):

```
.
├─ docs                # project root
│  ├─ .vitepress
│  │  ├─ theme
│  │  │  └─ index.ts   # theme entry
│  │  └─ config.ts     # config file
│  └─ index.md
└─ package.json
```

VitePress will always use the custom theme instead of the default theme when it detects presence of a theme entry file. You can, however, [extend the default theme](https://vitepress.dev/guide/extending-default-theme) to perform advanced customizations on top of it.

## Customizing CSS

The default theme CSS is customizable by overriding root level CSS variables:

```js
// .vitepress/theme/index.ts
import DefaultTheme from "vitepress/theme";
import "./index.css";

export default DefaultTheme;
```

```css
/* .vitepress/theme/index.css */
:root {
  --vp-c-brand: #646cff;
  --vp-c-brand-light: #747bff;
  --vp-c-brand-lighter: #848cff;
  --vp-c-brand-dark: #545cff;
  --vp-c-brand-darker: #444cff;
}
```

See [default theme CSS variables](https://github.com/vuejs/vitepress/blob/main/src/client/theme-default/styles/vars.css) that can be overridden.
