# `import {modules} as esm from "nodejs"`

Code for my talk, going over modules and ESM in Node.js.

## Contents

- [**./conditional-exports**](./conditional-exports):
  - Contains a relatively barebones example of using Node.js's [conditional exports](https://nodejs.org/api/esm.html#esm_conditional_exports) with ESM and CommonJS exports from a module (checked in to `node_modules`) and using them, respectively. Uses both implicit ESM and explicit ESM.
- [**./explicit-esm**](./explicit-esm):
  - Demonstrates explicit ESM in Node.js, using `.mjs` extensions for ESM files.
- [**./implicit-esm**](./implicit-esm):
  - Demonstrates implicit ESM in Node.js, using `"type": "module"` in the project's `package.json` and `.js` extensions for ESM files.

## Definitions

- ESM
  - ECMAScript Modules, the moudle system that's built-in to JavaScript and defined by TC39.
- Implicit ESM
  - Implicit ESM is ESM in Node.js that uses `"type": "module"` as a property in `package.json`, which Node.js uses as an indicator to passively read all `.js` files as ESM rather than CommonJS (which Node.js defaults to or can be told to )
- Explicit ESM
  - Explicit ESM is ESM in Node.js that uses `.mjs` as its file extension. Node.js will automatically parse any file with .mjs as its file extension as ESM.