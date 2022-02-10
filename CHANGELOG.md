# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project
adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 1.0.0.beta.1 - 2022-02-10

### Added

- add support for svelte `{@const ...}` tag.
- upgrade dependencies
  ```
  @typescript-eslint/eslint-plugin ^5.6.0 → ^5.11.0
  @typescript-eslint/parser ^5.6.0 → ^5.11.0
  eslint ^8.4.1 → ^8.8.0
  eslint-plugin-import ^2.25.3 → ^2.25.4
  eslint-plugin-svelte3 ^3.2.1 → ^3.4.0
  prettier-plugin-svelte ^2.5.1 → ^2.6.0
  typescript ^4.5.3 → ^4.5.5
  ```

### Fixed

- fix svelte3/typescript not being loaded as a peer dependency

## 1.0.0.beta.0 - 2022-01-09

### Changed

- all `dependencies` are now `peerDependencies` which requires installing it in the host package.

### Added

- upgrade dependencies

  ```
  @typescript-eslint/eslint-plugin   ^5.6.0  →   ^5.9.0
  @typescript-eslint/parser          ^5.6.0  →   ^5.9.0
  eslint                             ^8.4.1  →   ^8.6.0
  eslint-plugin-import              ^2.25.3  →  ^2.25.4
  eslint-plugin-svelte3              ^3.2.1  →   ^3.3.0
  typescript                         ^4.5.3  →   ^4.5.4
  ```

  - Typescript **v4.5.4** add support for
    [disabling-import-elision](https://www.typescriptlang.org/docs/handbook/release-notes/typescript-4-5.html#disabling-import-elision)
    which is used by
    [eslint-plugin-svelte3 **v3.3.0**](https://github.com/sveltejs/eslint-plugin-svelte3/blob/master/CHANGELOG.md#330)
    (and also by [@tsconfig/svelte](https://www.npmjs.com/package/@tsconfig/svelte))
  - @typescript-eslint/eslint-plugin v5.9.0 add support for the new
    [inline type specifiers for exports and imports](https://www.typescriptlang.org/docs/handbook/release-notes/typescript-4-5.html#type-modifiers-on-import-names)
    on typescript v4.5.4 avoiding false positives for the eslint rule _consistent-type-imports_.

## 0.1.2

- doc: fix eslint `extends` example

## 0.1.1

- update readme

## 0.1.0

- add svelte support.
- first working typescript setup.
- first commit.
