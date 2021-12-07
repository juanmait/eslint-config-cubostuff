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
  // add this if you're in a monorepo and don't want a specific member to inherit eslint rules from
  // other configs that exists higher on the file system tree.

  extends: 'monosvelte',
  parserOptions: {
    tsconfigRootDir: __dirname,
  },
};
```
