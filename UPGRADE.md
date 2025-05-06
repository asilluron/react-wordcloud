# React Wordcloud Plus - v2.0.0

This is a fork of [react-wordcloud](https://github.com/chrisrzhou/react-wordcloud) with significant updates to make the library compatible with React 18 and modern ESM syntax.

## Major Changes

### React 18 Compatibility
- Updated peer dependencies to support React 16.13.0, 17.x, and 18.x
- Updated event handling to use the new React 18 pattern
- Fixed TypeScript definitions to be compatible with React 18

### ESM Support
- Added proper ESM module exports
- Updated build configuration to output ESM and CJS formats
- Added `"type": "module"` to package.json

### Dependency Updates
- Updated all D3 dependencies to latest versions
- Updated other dependencies to latest compatible versions
- Replaced direct ResizeObserver polyfill with conditional usage

### Build System
- Updated microbundle to latest version
- Added modern output format

## Breaking Changes

1. The library now uses ESM syntax by default
2. D3 event handling has been updated to the latest pattern
3. The package now requires React 16.13.0 or higher

## Migration Guide

### For ESM/Modern Projects

```js
// Import the component
import ReactWordcloud from 'react-wordcloud-plus';

// Import the tooltip styles if needed
import 'tippy.js/dist/tippy.css';
import 'tippy.js/animations/scale.css';
```

### For CommonJS Projects

```js
// Import the component
const ReactWordcloud = require('react-wordcloud-plus').default;

// Import the tooltip styles if needed
require('tippy.js/dist/tippy.css');
require('tippy.js/animations/scale.css');
```

## TypeScript Support

TypeScript definitions have been updated to be compatible with React 18. The library continues to export the same types as before:

```ts
import ReactWordcloud, { Word, Options, Callbacks } from 'react-wordcloud-plus';
```
