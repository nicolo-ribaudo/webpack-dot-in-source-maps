1. Run `npm ci` to install dependencies
1. Run `rm -rf node_modules/@jridgewell/trace-mapping` to be 100% sure that it's not used
1. Run `npm run build`
1. Check the `"sources"` field in `dist/bundle.js.map`: it contains `"webpack://sourcemap-test/./src/index.ts"` and not `"webpack://sourcemap-test/src/index.ts"`
