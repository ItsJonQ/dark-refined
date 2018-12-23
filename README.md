# 🔸 Dark Refined

[![Version](https://vsmarketplacebadge.apphb.com/version/itsjonq.dark-refined.svg)](https://marketplace.visualstudio.com/items?itemName=itsjonq.dark-refined)

> A series of VSCode themes based on Dark+

## Preview

![Default](https://raw.githubusercontent.com/ItsJonQ/dark-refined/master/images/refined-default.jpg)

## Generate

This is the magic sauce for Refined's themes!

### Setup

This project only has a couple of dependencies, which it uses to generate the VS Code `theme.json` files.

To install the dependencies, run:

```
npm install
```

To build the theme file(s), run:

```
npm start
```

### Theme files

A theme only really requires a single shade, which makes up the background.

**Example**

```js
// themes/palenight.js
const colors = require("../colors/default");

const config = {
  name: "Dark (Palenight)",
  type: "dark"
};

const shades = {
  background: "#292d3e"
};

module.exports = {
  config,
  shades,
  colors
};
```

The theme is generated into `/themes/`, with it's details added to `package.json` - ready for publishing!
