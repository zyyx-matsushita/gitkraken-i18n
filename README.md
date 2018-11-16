# gitkraken-i18n
Unofficial GitKraken i18n project

[![Build status](https://ci.appveyor.com/api/projects/status/1xs1l6w9qjxfjmrf?svg=true)](https://ci.appveyor.com/project/megos/gitkraken-i18n) [![CircleCI](https://circleci.com/gh/megos/gitkraken-i18n.svg?style=svg)](https://circleci.com/gh/megos/gitkraken-i18n) [![TravisCI](https://api.travis-ci.org/megos/gitkraken-i18n.svg)](https://travis-ci.org/megos/gitkraken-i18n)

## Contents
- [Japanese](README-ja.md)

## Requirement
- git

## Patch
- Construction


## Translate

### Requirement
- node
- npm
- asar

### Setting

1. Copy GitKraken's `app.asar` to project dir and rename to `app.asar.original`.
1. Copy GitKraken's `app.asar.unpacked` to project dir and rename to `app.asar.original.unpacked`.
1. Extract `app.asar` to `app.extract`.
Copy `en-us.json` to your locale json file.
   - `npm run extract`
1. Translate json file.
1. Copy your locale json file to `app.extract/src/string/en-us.json`
1. Pack `app.asar`
   - `npm run pack`
1. Overwrite created `app.asar` to GitKraken's `app.asar`.
1. Restart GitKraken and check translate.
