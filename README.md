# tfm.js
An TFM parser implementation with TypeScript.

[![NPM](https://nodei.co/npm/tfm-js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/tfm-js)

## Installation
```
npm i tfm-js
```

## Usage
Please see [docs](./docs/index.md) for the detail.

TypeScript:
```ts
import * as tfm from 'tfm-js';

const inputText =
`<center>
Hello $[tada everynyan! 🎉]
</center>`;

// Generate a MFM tree from the full MFM text.
const tfmTree = tfm.parse(inputText);

// Generate a MFM tree from the simple MFM text.
const simpleTfmTree = tfm.parseSimple('I like the hot soup :soup:​');

// Reverse to a MFM text from the MFM tree.
const text = tfm.toString(tfmTree);

```

## Develop
### 1. Clone
```
git clone https://github.com/tanukey-dev/tfm.js
```

### 2. Install packages
```
cd tfm.js
npm i
```

### 3. Build
```
npm run build
```

### Use the interactive CLI parser
full parser:
```
npm run parse
```

simple parser:
```
npm run parse-simple
```

## License
This software is released under the [MIT License](LICENSE).
