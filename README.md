[![Build status](https://travis-ci.org/PolymerElements/paper-radio-group.svg?branch=master)](https://travis-ci.org/PolymerElements/paper-radio-group)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/PolymerElements/paper-radio-group)

## &lt;paper-radio-group&gt;

Material design: [Radio button](https://www.google.com/design/spec/components/selection-controls.html#selection-controls-radio-button)

`paper-radio-group` allows user to select at most one radio button from a set.
Checking one radio button that belongs to a radio group unchecks any
previously checked radio button within the same group. Use
`selected` to get or set the selected radio button.

The <paper-radio-buttons> inside the group must have the `name` attribute
set.

Example:

```html
<paper-radio-group selected="small">
  <paper-radio-button name="small">Small</paper-radio-button>
  <paper-radio-button name="medium">Medium</paper-radio-button>
  <paper-radio-button name="large">Large</paper-radio-button>
</paper-radio-group>
```

Radio-button-groups can be made optional, and allow zero buttons to be selected:

```html
<paper-radio-group selected="small" allow-empty-selection>
  <paper-radio-button name="small">Small</paper-radio-button>
  <paper-radio-button name="medium">Medium</paper-radio-button>
  <paper-radio-button name="large">Large</paper-radio-button>
</paper-radio-group>
```

See <a href="paper-radio-button">paper-radio-button</a> for more
information about `paper-radio-button`.

| Custom property | Description | Default |
| --- | --- | --- |
| `--paper-radio-group-item-padding` | The padding of the item | `12px` |

### Notable breaking changes between 1.x and 2.x (hybrid):

IronSelectableBehavior and IronMultiSelectableBehavior, which are used by
paper-radio-group, introduce multiple breaking changes. Please see the README
for those behaviors for more detail.
