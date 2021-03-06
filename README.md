# Boosterfor EZS plugin

This package cannot be used alone. EZS has to be installed.

## Example

```js
#!/usr/bin/env ezs

[use]
plugin = booster

[booster]
file = ./script.ini
```

## Installation

    $ git clone https://github.com/touv/node-booster.git
    $ cd node-booster
    $ npm install -g ezs
    $ npm install
    $ npm link
    $ npm run build 
    $ echo "booster do something !" | ./examples/booster.ezs

## Statements

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### Table of Contents

-   [booster](#booster)
    -   [Parameters](#parameters)

### booster

Takes an `Object` delegate processing to an external pipeline and cache the result

#### Parameters

-   `data`  
-   `feed`  
-   `file` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** the external pipeline is descrbied in a file
-   `script` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** the external pipeline is descrbied in a sting of characters
-   `commands` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** the external pipeline is descrbied in object
-   `key` **[String](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)?** the cache key identifier form the stream, in not provided, the key is computed with the first chunk
-   `hitsByCheck` **[Number](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number)** Number of hits to verify the cache (optional, default `1000`)
-   `maxFiles` **[Number](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number)** Number of hits to verify the cache (optional, default `100`)
-   `maxTotalSize` **[Number](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number)** Size (bytes) maximun of the cash (1 G) (optional, default `1000000000`)
-   `cleanupDelay` **[Number](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number)** Frequency (milliseconds) to cleanup the cahe (10 min) (optional, default `600000`)

Returns **[Object](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object)** 
