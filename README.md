# Fusebox

[![Build Status](https://travis-ci.org/fuse-box/fuse-box.svg?branch=master)](https://travis-ci.org/fuse-box/fuse-box)
[![Fusebox-bundler](https://img.shields.io/badge/gitter-join%20chat%20%E2%86%92-brightgreen.svg)](https://gitter.im/fusebox-bundler/Lobby)

[![NPM](https://nodei.co/npm/fuse-box.png?downloads=true)](https://nodei.co/npm/fuse-box/)

http://fuse-box.org/

FuseBox is a bundler/module loader that combines the power of webpack, JSPM and SystemJS. 

It is blazing fast (it takes 50-100ms to re-bundle) which makes it extremely convenient for developers. It requires zero configuration to bundle such monsters like `babel-core`.

FuseBox loves __typescript__, and does not require any additional configuration. It will compile and bundle your code within a fraction of a second, yet offering a comprehensive loader API. 

It is packed with features, and unfolds limitless possibilities of extending the API.

[Offical documentation](http://fuse-box.org/) / Submit an [issue](https://github.com/fuse-box/fuse-box/issues/new) / Make [documentation](https://github.com/fuse-box/fuse-box/tree/master/docs) better / Join [gitter channel](https://gitter.im/fusebox-bundler/Lobby) we are active!


## Installation

```bash
npm install fuse-box --save-dev
```

FuseBox has many plugins in place to help you get started. All you need to do is install `fuse-box` from npm.

## Try it now!

Check a [marvellous TODO app](https://fuse-box.github.io/angular2-example/) built on the latest [ng2+sass](https://github.com/fuse-box/angular2-example). Fuse it in a fraction of second! (50-80ms)
[react-example](https://github.com/fuse-box/react-example) 50ms!

Check this [benchmark](https://github.com/fuse-box/benchmark):
__1200 files to bundle__

|         |            |
| ------------- |:-------------:| 
| FuseBox      | __0.234s__ |
| Webpack      | 1.376s |


__1000 files to bundle / 10 times__

|         |            |
| ------------- |:-------------:| 
| FuseBox      | __2.257s__ |
| Webpack      | 13.591s |

## All your need to compile and bundle typescript

```
FuseBox.init({
    homeDir: "src/",
    sourceMap: {
         bundleReference: "./sourcemaps.js.map",
         outFile: "sourcemaps.js.map",
    },
    outFile: "./out.js"
}).bundle(">index.ts");
```
