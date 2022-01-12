# eslint-config-monosvelte

```bash
npm install @cubostuff/eslint-config-monosvelte
```

## Usage

Create a file `.eslintrc.js` and add the following.

> should be **.eslintrc.cjs** if your package.json has `"type": "module"`.

```js
module.exports = {
  root: true,
  // add this if you're in a monorepo and don't want a specific member to inherit eslint rules from
  // other configs that exists higher on the file system's tree.

  extends: '@cubostuff/eslint-config-monosvelte',
  parserOptions: {
    tsconfigRootDir: __dirname,
  },
};
```

## Release

```bash
npm version minor
# options (major, minor, or patch)
# - increments the version your package.json based on the type of the change
# - commits this version bump
# - creates a tag for the current release
npm publish
git push
git push --tags
```