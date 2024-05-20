# Vue Js crash course

## Directives

A way to connect to elements in the html with the Vue Js JavaScript
They are used as html attributes but prepended by a `v-` to differentiate them from regular html attributes.
Examples are:

1. `v-model` : Allows for two-way data binding.
2. `v-if`: Conditional statements. Takes in a boolean variable
3. `v-show`: Sets styling to display="none"
4. `v-cloak`: Hides anything from rendering until the page/application is ready.

## Events and Methods

To create custom functions, the `methods` object is used to house and register the methods to Vue JS.

Accessing custom variables within the methods, the `this` kkeyword is used as Vue Js registeres all defined varibles though it in its instance.

There are also event modifiers in Vue js. For example `@click.prevent` or `@keyup.enter`

`v-on`: specific directive used for events. Short-hand is `@` symbol and then the event name e.g. `@.click`

## Vue components

Has the same structure as the default template.

Must be defined before the mounting of the app.

Data defined within a custom component can only be used within its template.
