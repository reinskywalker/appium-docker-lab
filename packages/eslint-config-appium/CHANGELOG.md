# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## [8.0.5](https://github.com/appium/appium/compare/@appium/eslint-config-appium@8.0.4...@appium/eslint-config-appium@8.0.5) (2023-10-18)

**Note:** Version bump only for package @appium/eslint-config-appium





## [8.0.4](https://github.com/appium/appium/compare/@appium/eslint-config-appium@8.0.3...@appium/eslint-config-appium@8.0.4) (2023-07-03)


### Bug Fixes

* **eslint-config-appium:** remove prototype assignment warning ([679865e](https://github.com/appium/appium/commit/679865ed2f1df59baef8c4d884b0a63a9222940e))



## [8.0.3](https://github.com/appium/appium/compare/@appium/eslint-config-appium@8.0.2...@appium/eslint-config-appium@8.0.3) (2023-04-03)

**Note:** Version bump only for package @appium/eslint-config-appium





## [8.0.2](https://github.com/appium/appium/compare/@appium/eslint-config-appium@8.0.1...@appium/eslint-config-appium@8.0.2) (2023-03-28)


### Bug Fixes

* **eslint-config-appium:** disable import/no-unresolved for tsd tests ([020473a](https://github.com/appium/appium/commit/020473afc43e68215a576cb3d723b2de2de8e8ad))





## [8.0.1](https://github.com/appium/appium/compare/@appium/eslint-config-appium@8.0.0...@appium/eslint-config-appium@8.0.1) (2023-03-08)

**Note:** Version bump only for package @appium/eslint-config-appium





# [8.0.0](https://github.com/appium/appium/compare/@appium/eslint-config-appium@7.0.0...@appium/eslint-config-appium@8.0.0) (2022-12-14)

- chore!: set engines to minimum Node.js v14.17.0 ([a1dbe6c](https://github.com/appium/appium/commit/a1dbe6c43efe76604943a607d402f4c8b864d652))

### BREAKING CHANGES

- Appium now supports version range `^14.17.0 || ^16.13.0 || >=18.0.0`

# [7.0.0](https://github.com/appium/appium/compare/@appium/eslint-config-appium@6.0.4...@appium/eslint-config-appium@7.0.0) (2022-09-07)

### chore

- **eslint-config-appium:** upgrade to ESLint v8 ([887cb44](https://github.com/appium/appium/commit/887cb449e61be585c084af2f6422d2e02be5028b))

### BREAKING CHANGES

- **eslint-config-appium:** This change upgrades to ESLint v8 and removes `@babel/eslint-parser`, which is only necessary if we're using mid-stage TC39 proposals (which we aren't). I think `@babel/core` was a peer dep of `@babel/eslint-parser`, so I removed that too. And removed cruft from the main configuration.

ESLint rules _very likely_ had breaking changes, but I didn't experience any on our codebase. However, this version of ESLint seems to be incompatible with `gulp-eslint`, so `@appium/gulp-plugins` should be held back from upgrading.

In addition:

- Updated `README.md`
- Updated some fields in `package.json`
- Loosened `peerDependencies`, as they're supposed to be loose.

## [6.0.4](https://github.com/appium/appium/compare/@appium/eslint-config-appium@6.0.3...@appium/eslint-config-appium@6.0.4) (2022-08-03)

### Bug Fixes

- **appium,base-driver,base-plugin,doctor,docutils,eslint-config-appium,execute-driver-plugin,fake-driver,fake-plugin,gulp-plugins,images-plugin,opencv,relaxed-caps-plugin,schema,support,test-support,types,universal-xml-plugin:** update engines ([d8d2382](https://github.com/appium/appium/commit/d8d2382327ba7b7db8a4d1cad987c0e60184c92d))

## [6.0.3](https://github.com/appium/appium/compare/@appium/eslint-config-appium@6.0.2...@appium/eslint-config-appium@6.0.3) (2022-07-28)

**Note:** Version bump only for package @appium/eslint-config-appium

## [6.0.2](https://github.com/appium/appium/compare/@appium/eslint-config-appium@6.0.1...@appium/eslint-config-appium@6.0.2) (2022-05-31)

**Note:** Version bump only for package @appium/eslint-config-appium

## [6.0.1](https://github.com/appium/appium/compare/@appium/eslint-config-appium@6.0.0...@appium/eslint-config-appium@6.0.1) (2022-05-31)

**Note:** Version bump only for package @appium/eslint-config-appium

# [6.0.0](https://github.com/appium/appium/compare/@appium/eslint-config-appium@5.1.1...@appium/eslint-config-appium@6.0.0) (2022-05-03)

### Features

- **eslint-config-appium,gulp-plugins:** add prettier ([878bb6a](https://github.com/appium/appium/commit/878bb6a44f85fd43e0f3678b95cddb8d7cbba69a))

### BREAKING CHANGES

- **eslint-config-appium,gulp-plugins:** `@appium/eslint-config-appium` now requires peer dependency `eslint-config-prettier`. Because `@appium/gulp-plugins` always uses the latest development version of `@appium/eslint-config-appium`, the dependency needs to be added there, too.

In addition, this disables some rules, so _may_ cause code which previously passed lint checks _not_ to pass lint checks.

## [5.1.1](https://github.com/appium/appium/compare/@appium/eslint-config-appium@5.1.0...@appium/eslint-config-appium@5.1.1) (2022-05-03)

### Bug Fixes

- **eslint-config-appium:** remove custom indenting rules ([d89203f](https://github.com/appium/appium/commit/d89203f96c7d45e8cda5e447c808d1485449c284))
- **eslint-config-appium:** revert prettier-related change ([93e05a8](https://github.com/appium/appium/commit/93e05a82696514be04d9792c90eb3fe7e3fa0143))

# [5.1.0](https://github.com/appium/appium/compare/@appium/eslint-config-appium@5.0.6...@appium/eslint-config-appium@5.1.0) (2022-05-02)

### Bug Fixes

- **eslint-config-appium:** disable space-before-function-paren ([88a6655](https://github.com/appium/appium/commit/88a6655253a4879041478d64254471efebe4cbfe))

### Features

- **eslint-config-appium:** adds a warning if code attempts to assign to an object prototype ([5bdc476](https://github.com/appium/appium/commit/5bdc476c626caa301c7cb4ffc01c296f437deb06)), closes [#16829](https://github.com/appium/appium/issues/16829)

## [5.0.6](https://github.com/appium/appium/compare/@appium/eslint-config-appium@5.0.5...@appium/eslint-config-appium@5.0.6) (2022-04-20)

**Note:** Version bump only for package @appium/eslint-config-appium

## [5.0.5](https://github.com/appium/appium/compare/@appium/eslint-config-appium@5.0.4...@appium/eslint-config-appium@5.0.5) (2022-04-20)

**Note:** Version bump only for package @appium/eslint-config-appium

## [5.0.4](https://github.com/appium/appium/compare/@appium/eslint-config-appium@5.0.3...@appium/eslint-config-appium@5.0.4) (2022-04-12)

**Note:** Version bump only for package @appium/eslint-config-appium

## [5.0.3](https://github.com/appium/appium/compare/@appium/eslint-config-appium@5.0.2...@appium/eslint-config-appium@5.0.3) (2022-04-07)

**Note:** Version bump only for package @appium/eslint-config-appium

## [5.0.2](https://github.com/appium/appium/compare/@appium/eslint-config-appium@5.0.1...@appium/eslint-config-appium@5.0.2) (2022-03-22)

**Note:** Version bump only for package @appium/eslint-config-appium

## [5.0.1](https://github.com/appium/appium/compare/@appium/eslint-config-appium@5.0.0...@appium/eslint-config-appium@5.0.1) (2022-01-11)

**Note:** Version bump only for package @appium/eslint-config-appium

# [5.0.0](https://github.com/appium/appium/compare/@appium/eslint-config-appium@4.7.4...@appium/eslint-config-appium@5.0.0) (2021-11-19)

### Bug Fixes

- **eslint-config-appium:** switch to peerdeps ([7fb1667](https://github.com/appium/appium/commit/7fb1667a3b702a22ec365b6fc8e88c88e4e24573))

### BREAKING CHANGES

- **eslint-config-appium:** ESLint expects configs or plugins which require other configs or plugins to have _peer dependencies_ of those things _and_ of ESLint itself. All deps have been changed to peer deps, and this module now requires the installation of the following _if_ using npm older than v7:

```
    "@babel/core": "7.16.0",
    "@babel/eslint-parser": "7.16.3",
    "eslint": "7.32.0",
    "eslint-plugin-import": "2.25.3",
    "eslint-plugin-mocha": "9.0.0",
    "eslint-plugin-promise": "5.1.1"
```

npm@7 will install these automatically if they do not exist.

## [4.7.4](https://github.com/appium/appium/compare/@appium/eslint-config-appium@4.7.3...@appium/eslint-config-appium@4.7.4) (2021-11-15)

**Note:** Version bump only for package @appium/eslint-config-appium

## [4.7.3](https://github.com/appium/appium/compare/@appium/eslint-config-appium@4.7.2...@appium/eslint-config-appium@4.7.3) (2021-11-09)

**Note:** Version bump only for package @appium/eslint-config-appium

## [4.7.2](https://github.com/appium/appium/compare/@appium/eslint-config-appium@4.7.1...@appium/eslint-config-appium@4.7.2) (2021-09-14)

**Note:** Version bump only for package @appium/eslint-config-appium

## [4.7.1](https://github.com/appium/appium/compare/@appium/eslint-config-appium@4.7.0...@appium/eslint-config-appium@4.7.1) (2021-08-16)

# 2.0.0-beta (2021-08-13)

**Note:** Version bump only for package @appium/eslint-config-appium
