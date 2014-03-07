node-addon-example
==================

Sample starter application for a Node C++ addon packaged with node-pre-gyp.

## Depends

- Node.js 0.10.x or 0.8.x

## Install

Install from binary:

    npm install

Install from source:

    npm install --build-from-source

## Developing

To recompile only the C++ files that have changed, first put `node-gyp` and `node-pre-gyp` on your PATH:

    export PATH=`npm explore npm -g -- pwd`/bin/node-gyp-bin:./node_modules/.bin:${PATH}

Then simply run:

    node-pre-gyp build

### Packaging

    node-pre-gyp build package

### Publishing

    npm install aws-sdk
    node-pre-gyp publish
