## Usage

### Include: Page

``` hbs
{{! @INSERT :: START @id: accordion, @tag: component-partial }}
{{#with accordion-bp.variations.simple}}
    {{! WrapWith START: Accordion }}
    {{#wrapWith "accordion" settings=this.settings}}
    {{! WrapWith START: Item }}
        {{#each content.items}}
            {{#wrapWith "accordion__item" accItemId=this.itemId accButton=itemBtnText}}
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ab aliquid assumenda, ducimus facilis inventore iste labore laborum libero nam necessitatibus neque nulla numquam perspiciatis rem, repudiandae sed soluta veniam vero.
            {{/wrapWith}}
        {{/each}}
    {{! WrapWith END: Item }}
    {{/wrapWith}}
    {{! WrapWith END: Accordion }}
{{/with}}
{{! @INSERT :: END }}
```

### Include: JavaScript

#### Initializing in Veams V5

``` js
// @INSERT :: START @tag: js-init-v5 //
	// Init Accordion
	Veams.modules.add({ namespace: 'accordion', module: Accordion });
// @INSERT :: END //
```

#### Custom Events

``` js
// @INSERT :: START @tag: js-events //
/**
 * Events Accordion
 */
EVENTS.accordion = {
	openAll: 'accordion:openAll',
	closeAll: 'accordion:closeAll'
};
// @INSERT :: END //
```