# Accordion

The component represents a simple accordion with `transitions` and `max-height`.

Accordions are elements used to expand and collapse content that is broken into logical sections, much like tabs.

This component is based on the blueprint of Veams-Components.

## Version

Latest version is ```v2.0.1```

## Requirements

### JavaScript
- `Veams-JS >= v4.0.0`

### Sass
- `_get-media.scss`

## Usage

### Options:

#### activeClass
`Type: String` | `Default: is-active`

Define the active class for active elements.

#### accordionBtn
`Type: String` | `Default: [data-js-atom="accordion-btn"]`

Define the element for accordion buttons

#### accordionContent
`Type: String` | `Default: [data-js-atom="accordion-content"]`

Define the element for accordion content items.

#### calculatingClass
`Type: String` | `Default: is-calculating`

Define the calculating class for the initial calculation cycle.

#### clickHandler
`Type: String` | `Default: click`

Define a click handler for the buttons.

#### closeClass
`Type: String` | `Default: is-closed`

Define the closing class for accordion content items.

#### dataMaxAttr
`Type: String` | `Default: data-js-height`

Define the attribute in which the calculated height is saved.

#### openAllOnInit
`Type: Boolean` | `Default: false`

If set to true, all panels stays open on render.

#### openByHash
`Type: Boolean` | `Default: false`

If set to true, panel can be opened by url hash referencing the id of the panel

#### openClass
`Type: Boolean` | `Default: is-open`

Define the opening class for accordion content items.

#### openIndex
`Type: Number` | `Default: null`

Index of panel to be opened on init (zero based)

#### openOnViewports
`Type: Array` | `Default: ['desktop', 'tablet-large', 'tablet-small']`

Viewports on which the openIndex panel is opened on init

#### singleOpen
`Type: Boolean` | `Default: false`

If set to true, only one panel can be opened at the same time

#### tabMode
`Type: Boolean` | `Default: false`

If set to true, the accordion behaves like a tab module (click on active button will not close corresponding panel).

#### unresolvedClass
`Type: String` | `Default: is-unresolved`

Define the unresolved class for the whole accordion which will be deleted after `initialize()` and `render()` is finished.