## Node Buffer to WEB (browser)

This is freely adaptation of [buffer](https://github.com/feross/buffer) with es6 modules


#### Reason

The implementation suggested in the original package suggests using browserify, but browserify adds a lot of Kbits to make the bundle.

A "non-bundled" (minimized) version is also available ... however it adds `buffer` to the global scope and weighs approximately 50.8kB and is not modular (es6 module syntax).

This adaptation for es6 modules weighs only (with its 2 dependency files) 33.9kB minified with copyright comments.

### How to use:

```javascript
// in your module
import {
    Buffer,
    SlowBuffer,
    INSPECT_MAX_BYTES,
    kMaxLength
} from 'your-path/to/buffer/buffer.min.mjs'

const buff = Buffer.from("I'm a string", "utf-8")
console.log(buff
```

This excerpt show:

```console
Uint8Array(13) [73, 39, 109, 32, 97, 32, 115, 116, 114, 105, 110, 103, 33]
0: 73
1: 39
2: 109
3: 32
4: 97
5: 32
6: 115
7: 116
8: 114
9: 105
10: 110
11: 103
12: 33
offset: (...)
parent: (...)
buffer: (...)
byteLength: (...)
byteOffset: (...)
length: (...)
Symbol(Symbol.toStringTag): (...)
__proto__: Uint8Array
```

### API:

Go to https://nodejs.org/api/buffer.html for full buffer method's
