# WebAssembly GraphQL parser

[GraphQL](https://graphql.org) parser in [WebAssembly](https://webassembly.org), compiled from [Rust](https://www.rust-lang.org).

## Status: experimental

API/AST structure will probably change.
No semantic validation at the moment, just syntax (e.g. you can declare a field twice).

## Usage via NPM

Published at npm as `graphql-wasm-parser`. Add it as dependency and use it like any other js module:

```js
const { parse } = require('graphql-wasm-parser');

const ast = parse("{foo}");
console.log(JSON.stringify(ast));
```