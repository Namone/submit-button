# submit-button

This README outlines the details of collaborating on this Ember addon.

This Ember component was developed by Nate Schroader and converted/published to an addon by Alex Nordhausen.

## Installation

* `npm install submit-button`

##Usage

* Place `{{#submit-button action="yourActionHere"}}Button Text{{/submit-button}}` into your page templates. 

There are a couple settings one is able to set for each button, including the `loadingIcon` and the `locked` properties.

* **tagName:** `button`,
* **attributeBindings:** `[ 'type' ]`,
* **type:** `submit`,
* **loadingIcon:** `<i class="fa fa-cog fa-spin"></i>`,
* **locked:** `false`,

The settings are pretty self explanatory. One can alter each of these via inserting them into the component itself:

`{#submit-button class="btn btn-default btn-block" locked=formLocked action="login"}}Submit{{/submit-button}}`

`loadingIcon` can be used to set a default icon for when the button is in the submission process.

`locked` can be used to set if the forms associated with the submission button are 'locked'; as in they cannot be altered
until the form is properly submitted (and returns either success or error.)
    
## Running

* `ember serve`
* Visit your app at [http://localhost:4200](http://localhost:4200).

## Running Tests

* `npm test` (Runs `ember try:each` to test your addon against multiple Ember versions)
* `ember test`
* `ember test --server`

## Building

* `ember build`

For more information on using ember-cli, visit [https://ember-cli.com/](https://ember-cli.com/).
