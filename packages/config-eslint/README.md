# `@hakui/eslint-config`

A collection of ESLint configurations for various environments.

## Installation

To install the package, run:

```sh
npm install @hakui/eslint-config --save-dev
```

or

```sh
yarn add @hakui/eslint-config --dev
```

## Usage

### Next.js

```js
import { config } from '@hakui/eslint-config/next-js';

/** @type {import('eslint').Linter.Config} */
export default config;
```

### React

```js
import { config } from '@hakui/eslint-config/react-internal';

/** @type {import("eslint").Linter.Config} */
export default config;
```

### Vite

```js
import { config } from '@hakui/eslint-config/vite';

/** @type {import("eslint").Linter.Config} */
export default config;
```

### Custom

You can also extend the configurations to suit your needs. For example:

```js
import { config as baseConfig } from '@hakui/eslint-config/base';

/** @type {import('eslint').Linter.Config} */
export default [
  ...baseConfig,
  {
    rules: {
      // Add your custom rules here
    },
  },
];
```

