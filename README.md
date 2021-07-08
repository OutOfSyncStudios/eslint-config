# eslint-config-ooss

This is the Out of Sync Studios eslint common configuration for multiple Node development environments.

## Installation
```shell
$ npm install @outofsync/eslint-config-ooss
```
or
```shell
$ yarn add @outofsync/eslint-config-ooss
```

## Usage
This eslint config plugin provides a common environment and one extension for front-end specific rules.

To use this plugin install module as noted above and then edit the `.eslintrc.json` file in the root of your project to look like below.
```json
{
  "extends": "@outofsync/eslint-config-ooss",
  "rules": {
    ...
  }
}
```
This will include the `common` definitions. ***Note***: Any addtional rules that appear in the rules section will override the base settings.

You can also specify to add the front-end extensions as follows:
```json
{
  "extends": [
    "@outofsync/eslint-config-ooss",
    "@outofsync/eslint-config-ooss/frontend-extension"
  ],
  "rules": {
    ...
  }
}
```