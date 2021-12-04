# eslint-config-monosvelte

```bash
npm install eslint-config-monosvelte
```

## Usage

Create a file `.eslintrc.js` and add the following.

> should be **.eslintrc.cjs** if your package.json has `"type": "module"`.

```js
module.exports = {
  extends: 'monosvelte',
  parserOptions: {
    tsconfigRootDir: __dirname,
  },
};
```
