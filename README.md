# npmdoc-jsmediatags

#### api documentation for  [jsmediatags (v3.4.0)](https://github.com/aadsm/jsmediatags#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-jsmediatags.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jsmediatags) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jsmediatags.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jsmediatags)

#### Media Tags Reader (ID3, MP4)

[![NPM](https://nodei.co/npm/jsmediatags.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/jsmediatags)

- [https://npmdoc.github.io/node-npmdoc-jsmediatags/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-jsmediatags/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jsmediatags/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jsmediatags/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jsmediatags/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jsmediatags/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "António Afonso"
    },
    "bugs": {
        "url": "https://github.com/aadsm/jsmediatags/issues"
    },
    "contributors": [
        {
            "name": "Jacob Seidelin"
        },
        {
            "name": "Joshua Kifer"
        },
        {
            "name": "Jesse Ditson"
        }
    ],
    "dependencies": {
        "xhr2": "~0.1.3"
    },
    "description": "Media Tags Reader (ID3, MP4)",
    "devDependencies": {
        "babel-cli": "~6.7.7",
        "babel-core": "~6.7.7",
        "babel-jest": "~12.0.2",
        "babel-plugin-transform-class-properties": "~6.6.0",
        "babel-plugin-transform-es2015-block-scoping": "~6.7.1",
        "babel-plugin-transform-es2015-classes": "~6.6.5",
        "babel-plugin-transform-es2015-modules-commonjs": "~6.7.4",
        "babel-plugin-transform-flow-strip-types": "~6.7.0",
        "babelify": "~7.3.0",
        "browserify": "~13.0.0",
        "google-closure-compiler": "20160315.2.0",
        "jest-cli": "~12.0.2",
        "watchify": "~3.7.0"
    },
    "directories": {},
    "dist": {
        "shasum": "5c5975754e8e62c1697dcfcba5804996b6e23ddc",
        "tarball": "https://registry.npmjs.org/jsmediatags/-/jsmediatags-3.4.0.tgz"
    },
    "engines": {
        "node": ">=4.0.0"
    },
    "homepage": "https://github.com/aadsm/jsmediatags#readme",
    "jest": {
        "rootDir": "./src",
        "scriptPreprocessor": "../node_modules/babel-jest"
    },
    "keywords": [
        "ID3",
        "tags",
        "mp3",
        "audio",
        "mp4"
    ],
    "license": "BSD-3-Clause",
    "main": "build2/jsmediatags.js",
    "maintainers": [
        {
            "name": "aadsm"
        }
    ],
    "name": "jsmediatags",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/aadsm/jsmediatags.git"
    },
    "scripts": {
        "build": "babel src --ignore __tests__,__mocks,FlowTypes.js --out-dir build2",
        "dist": "npm run dist-dev && java -jar node_modules/google-closure-compiler/compiler.jar --warning_level QUIET --compilation_level SIMPLE_OPTIMIZATIONS --js dist/jsmediatags.js > dist/jsmediatags.min.js",
        "dist-dev": "mkdir -p dist && browserify src/jsmediatags.js --detect-globals false -i ./src/NodeFileReader.js -o dist/jsmediatags.js -s jsmediatags -t [ babelify --plugins [ transform-flow-strip-types transform-es2015-modules-commonjs transform-class-properties transform-es2015-classes transform-es2015-block-scoping ] ]",
        "dist-watch": "mkdir -p dist && watchify src/jsmediatags.js -v --detect-globals false -i ./src/NodeFileReader.js -o dist/jsmediatags.js -s jsmediatags -t [ babelify --plugins [ transform-flow-strip-types transform-es2015-modules-commonjs transform-class-properties transform-es2015-classes transform-es2015-block-scoping ] ]",
        "test": "jest",
        "watch": "babel --ignore __tests__,__mocks,FlowTypes.js --watch src --out-dir build2"
    },
    "version": "3.4.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
