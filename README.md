[![Published on NPM](https://img.shields.io/npm/v/@polymer/paper-radio-group.svg)](https://www.npmjs.com/package/@polymer/paper-radio-group)
[![Build status](https://travis-ci.org/PolymerElements/paper-radio-group.svg?branch=master)](https://travis-ci.org/PolymerElements/paper-radio-group)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://webcomponents.org/element/@polymer/paper-radio-group)

## &lt;paper-radio-group&gt;

`<paper-radio-group>` allows user to select at most one radio button from a set.
Checking one radio button that belongs to a radio group unchecks any previously
checked radio button within the same group. Use `selected` to get or set the
selected radio button.

The `<paper-radio-button>` elements inside the group must have the `name`
attribute set.

See: [Documentation](https://www.webcomponents.org/element/@polymer/paper-radio-group),
  [Demo](https://www.webcomponents.org/element/@polymer/paper-radio-group/demo/demo/index.html).

## Usage

### Installation

```
npm install --save @polymer/paper-radio-group
```

### In an HTML file

```html
<html>
  <head>
    <script type="module">
      import '@polymer/paper-radio-button/paper-radio-button.js';
      import '@polymer/paper-radio-group/paper-radio-group.js';
    </script>
  </head>
  <body>
    <paper-radio-group selected="small">
      <paper-radio-button name="small">Small</paper-radio-button>
      <paper-radio-button name="medium">Medium</paper-radio-button>
      <paper-radio-button name="large">Large</paper-radio-button>
    </paper-radio-group>
  </body>
</html>
```

### In a Polymer 3 element

```js
import {PolymerElement} from '@polymer/polymer/polymer-element.js';
import {html} from '@polymer/polymer/lib/utils/html-tag.js';

import '@polymer/paper-radio-button/paper-radio-button.js';
import '@polymer/paper-radio-group/paper-radio-group.js';

class ExampleElement extends PolymerElement {
  static get template() {
    return html`
      <paper-radio-group selected="small">
        <paper-radio-button name="small">Small</paper-radio-button>
        <paper-radio-button name="medium">Medium</paper-radio-button>
        <paper-radio-button name="large">Large</paper-radio-button>
      </paper-radio-group>
    `;
  }
}

customElements.define('example-element', ExampleElement);
```

## Contributing

If you want to send a PR to this element, here are the instructions for running
the tests and demo locally:

### Installation

```sh
git clone https://github.com/PolymerElements/paper-radio-group
cd paper-radio-group
npm install
npm install -g polymer-cli
```

### Running the demo locally

```sh
polymer serve --npm
open http://127.0.0.1:<port>/demo/
```

### Running the tests

```sh
polymer test --npm
```
