# parcel-plugin-worker

This Parcel plugin adds support for inlining of Web Workers. Note that the entire source code of your worker module is included in the importing module. As such it is advised to keep your worker module fairly small. 

**🚨 WARNING: THIS IS STILL A WIP**

Things not implemented:

- [ ] Support for imports in Worker module
- [ ] Support for plugin config
- [ ] Test coverage

## Installation

`yarn add parcel-plugin-inline-worker`

## Usage

```js
import MyWorker from './my.worker.js'

const worker = MyWorker.init()

worker.postmessage('hey')
```

## Licence 

MIT