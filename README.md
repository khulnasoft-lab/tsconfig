
# KhulnaSoft tsconfig

[![npm](https://img.shields.io/npm/v/@khulnasoft/tsconfig.svg)](https://www.npmjs.com/package/@khulnasoft/tsconfig)
[![downloads](https://img.shields.io/npm/dt/@khulnasoft/tsconfig.svg)](https://www.npmjs.com/package/@khulnasoft/tsconfig)
[![build](https://travis-ci.org/khulnasoft-lab/tsconfig.svg?branch=master)](https://travis-ci.org/khulnasoft-lab/tsconfig)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)

Base tsconfig.json for TypeScript projects at KhulnaSoft.
It only includes compiler options that make TypeScript more strict.
It does not set any project-specific or environmental settings.

## Usage

```
npm install --save-dev @khulnasoft/tsconfig
```

Then add this tsconfig.json:

```json
{
  "extends": "./node_modules/@khulnasoft/tsconfig/tsconfig.json"
}
```

## Making changes

```
npm link
cd <project>
npm link @khulnasoft/tsconfig
npm run lint
```

## Publish a new version

Follow [semver](http://semver.org/).

```
npm version major|minor|patch
git push
git push --tags
npm publish
```

