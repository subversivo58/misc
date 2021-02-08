## Node Buffer to WEB (browser)

This is freely adaptation of [buffer](https://github.com/feross/buffer) with es6 modules


#### Reason

The implementation suggested in the original package suggests using browserify, but browserify adds a lot of Kbits to make the bundle.

A "non-bundled" (minimized) version is also available ... however it adds `buffer` to the global scope and weighs approximately 50.8kB and is not modular (es6 module syntax).

This adaptation for es6 modules weighs only (with its 2 dependency files) 33.9kB minified with copyright comments.
