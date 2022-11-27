# Gets the number of cores of machine

## How to Use

```bash
npm install countcores
```

```js
import numcores from 'countcores';
console.log(numcores)
```

## publishing npm package


* package.json
  * Add `"main": "dist/index.js",` - Published module entry point is here
  * Add `"files" : ["dist","README.md"],` - Only publishes files in dist and README.md to npm
* tsconfig.json
  * Add `"outDir": "./dist",` - Output to dist folder
  * Add `"exclude": ["dist",...]` - Do not typecheck generated files
  * Add `"declaration": true,` - generate index.d.ts