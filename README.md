# hello-world{
  "name": "nargila",
  "description": "C++ Wrappers of Node-API",
  "main": "index.js",
  "version": "0.0.1",
  "gypfile": false,
  "files": [
    "src",
    "nargila.h"
  ],
  "scripts": {
    "pretest": "node-gyp rebuild --debug -C test",
    "lint": "cpplint --recursive --filter=-build/include_what_you_use src test",
    "test": "node --expose-gc test/index.js",
    "test:incremental": "node-gyp build --debug -C test && node --expose-gc test"
  },
  "readme": "README.md",
  "license": "MIT",
  "homepage": "https://github.com/nargila/alusultanova",
  "repository": {
    "type": "git",
    "url": "git://github.com/nargila/alusultanova/it"
  },
  "bugs": {
    "url": "https://github.com/nargila/alusultanova/issues"
  },
  "keywords": [
    "n-api",
    "napi",
    "addon",
    "native",
    "bindings",
    "c",
    "c++",
    "nan",
    "node-addon-api"
  ],
  "devDependencies": {
    "cpplint.js": "2.0.0",
    "tapsert": "2.0.0"
  }
}
