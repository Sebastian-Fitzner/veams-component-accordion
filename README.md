<p align='right'>
    <a href="https://badge.fury.io/js/@veams/component-accordion"><img src="https://badge.fury.io/js/@veams/component-accordion.svg" alt="npm version" height="18"></a>
    <a href='https://gitter.im/Sebastian-Fitzner/Veams?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge'><img src='https://badges.gitter.im/Sebastian-Fitzner/Veams.svg' alt='Gitter Chat' /></a>
</p>

# Accordion

## Description

The component represents a simple accordion with `transitions` and `max-height`. 

Accordions are elements used to expand and collapse content that is broken into logical sections, much like tabs.

The accordion is based on the blueprint of Veams-Components and is a wrap-with component to support flexible content with predefined surrounded markup.

The accordion is jQuery-free (we use Veams-Query) and contains some accessiblity functionality.

-----------

## Requirements
- [@veams/core](https://github.com/Veams/core) - Veams Core Framework.
- [@veams/query](https://github.com/Veams/query) or `jquery` - Veams Query or jQuery.
- [@veams/component](https://github.com/Veams/component) - Veams Component.
- [@veams/helpers](https://github.com/Veams/helpers) - Veams Detection Helpers.

-----------

## Installation 

### Installation with Veams

``` bash
veams install component accordion
```
``` bash
veams -i c accordion
```

----------- 

## Fields

### `accordion-usage.hbs`

The partial is a `{{#wrapWith}}` helper. Documentation for [wrapWith](https://github.com/Sebastian-Fitzner/mangony-hbs-helper-wrap-with) helper.


### `accordion.hbs`

#### Settings

| Parameter | Type | Value | Description |
|:--- | :---: |:---: | :--- |
| settings.accContextClass | String | `default` | Context class of component. |
| settings.accClasses | String | | Modifier classes for component. |
| settings.accJsOptions | Object | | JavaScript options which gets stringified. |

### `accordion__item.hbs`

#### Settings

| Parameter | Type | Description |
|:--- | :---: | :--- |
| settings.accNoWrapper | Boolean | Hide wrapper div `.accordion__item`. |

<!-- Further Parameters  -->
| Parameter | Type | Description |
|:--- | :---: | :--- |
| accItemId | String | Id of the accordion item. |
| accButton | String | Button text for accordion item. |

-------------

## JavaScript Options

The module gives you the possibility to override default options: 

| Option | Type | Default | Description |
|:--- | :---: |:---: |:--- |
| activeClass | String | `'is-active'` | Define the active class for active elements. |
| accordionBtn | String | `'[data-js-item='accordion-btn']'` | Define the element for accordion buttons. |
| accordionContent | String | `'[data-js-item="accordion-content"]'` | Define the element for accordion content items. |
| calculatingClass | String | `'is-calculating'` | Define the calculating class for the initial calculation cycle. |
| clickHandler | String | `'click'` | Define a click handler for the buttons. |
| closeClass | String | `'is-closed'` | Define the closing class for accordion content items. |
| dataMaxAttr | String | `'data-js-height'` | Define the attribute in which the calculated height is saved. |
| openAllOnInit | Boolean | `false` | If set to true, all panels stays open on render. |
| openByHash | Boolean | `false` | If set to true, panel can be opened by url hash referencing the id of the panel. |
| openClass | Boolean | `'is-open'` | Define the opening class for accordion content items. |
| openIndex | Number | `null` | Index of panel to be opened on init (zero based). |
| openOnViewports | Array | `['tablet-s', 'tablet-l', 'desktop-s', 'desktop-m', 'desktop-l']` | Viewports on which the openIndex panel is opened on init. |
| removeStyles | Boolean | `false` | If set to true, |
| singleOpen | Boolean | `false` | If set to true, only one panel can be opened at the same time. |
| tabMode | Boolean | `false` | If set to true, the accordion behaves like a tab module (clicking on active button will not close the corresponding panel). |
| unresolvedClass | String | `'is-unresolved'` | Define the unresolved class for the whole accordion which will be deleted after `didMount()` and `render()` is finished. |

------------

## Sass Options

There are multiple global variables which you can change: 

| Variable | Value | Description |
|:--- | :---: |:--- |
| $accordion-toggle-duration: | `300ms !default` | Speed of toggling. |
| $accordion-transition-method: | `ease !default` | Transition method of toggle effect. |
| $accordion-icon-color: | `#666 !default` | + icon color. |
| $accordion-icon-width: | `15px !default` | + icon width. |
| $accordion-icon-height: | `2px !default` | + icon height. |
| $accordion-btn-color: | `$accordion-icon-color !default` | Accordion button color. |
| $accordion-btn-bg-color: | `rgba(255, 255, 255, .5) !default` | Background color of the accordion button. |
| $accordion-padding: | `1rem !default` | Default padding which will be used in the accordion. |
