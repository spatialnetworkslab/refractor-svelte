# refractor-svelte

Syntax highlighting for svelte code with [refractor](https://github.com/wooorm/refractor/). Simple wrapper around [prism-svelte](https://github.com/pngwn/prism-svelte) by [pngwn](https://github.com/pngwn) so it can be registered as additional syntax in `refractor`. 

## Install

```bash
npm i refractor-svelte
```

## Usage

```js
const refractor = require('refractor');
const svelte = require('refractor-svelte');

refractor.register(svelte)

console.log(refractor.highlight('{#each items as item, i}{item.name}{/each}', 'svelte'))
```