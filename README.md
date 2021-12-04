# eslint-config-monosvelte

```bash
npm install eslint-config-monosvelte
```

## Usage

Create a file `.eslintrc.js` and add the following.

> should be **.eslintrc.cjs** if your package.json has `"type": "module"`.

```js
module.exports = {
  root: true,
  // add `root: true` if for example you're in a monorepo and don't want
  // a specific module to inherit eslint rules from other configs higher on
  // the file system tree.

  extends: 'monosvelte',
  parserOptions: {
    tsconfigRootDir: __dirname,
  },
};
```
