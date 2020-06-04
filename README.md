# react-barcode

A React component to generate Barcode.

[![NPM](https://img.shields.io/npm/v/@createnextapp/react-barcode.svg)](https://www.npmjs.com/package/@createnextapp/react-barcode) [![downloads](https://img.shields.io/npm/dm/@createnextapp/react-barcode.svg?style=flat-square)](https://www.npmjs.com/package/@createnextapp/react-barcode) ![npm bundle size](https://img.shields.io/bundlephobia/min/@createnextapp/react-barcode) [![Build Status](https://api.travis-ci.com/Bunlong/@createnextapp/react-barcode.svg?branch=master)](https://travis-ci.com/Bunlong/@createnextapp/react-barcode) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## 🔧 Install

react-barcode is available on npm. It can be installed with the following command:

```
npm install --save @createnextapp/react-barcode
```

react-barcode is available on yarn as well. It can be installed with the following command:

```
yarn add react-hook-qrcode
```

## 💡 Usage

### SVG

```js
import React from 'react';
import { useBarcode } from '@createnextapp/react-barcode';

function App() {
  const [inputRef] = useBarcode({
    value: '1234',
    options: {
      text: 'Hi'
    },
  });
  
  return <svg ref={inputRef} />;
};

export default App;
```

### Canvas

```js
import React from 'react';
import { useBarcode } from '@createnextapp/react-barcode';

function App() {
  const [inputRef] = useBarcode({
    value: '1234',
    options: {
      text: 'Hi'
    },
  });
  
  return <canvas ref={inputRef} />;
};

export default App;
```

### Image

```js
import React from 'react';
import { useBarcode } from '@createnextapp/react-barcode';

function App() {
  const [inputRef] = useBarcode({
    value: '1234',
    options: {
      text: 'Hi'
    },
  });
  
  return <img ref={inputRef} />;
};

export default App;
```

## Options

<table>
  <thead>
    <tr>
      <th>Prop</th>
      <th>Type</th>
      <th>Default</th>
      <th>Require</th>
      <th>Description</th>
    </tr>
  <thead>
  <tbody>
    <tr>
      <td>format</td>
      <td>string?</td>
      <td><code>auto</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>width</td>
      <td>number?</td>
      <td><code>2</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>height</td>
      <td>number?</td>
      <td><code>100</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>displayValue</td>
      <td>boolean?</td>
      <td><code>true</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>text</td>
      <td>string?</td>
      <td><code>undefined</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>fontOptions</td>
      <td>string?</td>
      <td><code>""</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>font</td>
      <td>string?</td>
      <td><code>"monospace"</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>textAlign</td>
      <td>string?</td>
      <td><code>"center"</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>textPosition</td>
      <td>string?</td>
      <td><code>"bottom"</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>textMargin</td>
      <td>number?</td>
      <td><code>2</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>fontSize</td>
      <td>number?</td>
      <td><code>20</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>background</td>
      <td>string?</td>
      <td><code>"#ffffff"</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>lineColor</td>
      <td>string?</td>
      <td><code>"#000000"</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>margin</td>
      <td>number?</td>
      <td><code>10</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>marginTop</td>
      <td>number?</td>
      <td><code>undefined</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>marginBottom</td>
      <td>number?</td>
      <td><code>undefined</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>marginLeft</td>
      <td>number?</td>
      <td><code>undefined</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>marginRight</td>
      <td>number?</td>
      <td><code>undefined</code></td>
      <td>❌</td>
      <td></td>
    </tr>
    <tr>
      <td>flat</td>
      <td>boolean?</td>
      <td><code>false</code></td>
      <td>❌</td>
      <td></td>
    </tr>
  </tbody>
</table>

## 💖 Wrap Up

If you think any of the `react-barcode` can be improved, please do open a PR with any updates and submit any issues. Also, I will continue to improve this, so you might want to watch/star this repository to revisit.

## 🌟 Contribution

We'd love to have your helping hand on contributions to `react-barcode` by forking and sending a pull request!

Your contributions are heartily ♡ welcome, recognized and appreciated. (✿◠‿◠)

How to contribute:

- Open pull request with improvements
- Discuss ideas in issues
- Spread the word
- Reach out with any feedback

## ⚖️ License

The MIT License [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
