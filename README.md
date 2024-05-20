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

## Component Props

For a component to be referenced within another component, the child comonent must be registered within the parent component.

This is done within the components object defined in the parent component through _props_.

The _props_ can also accept, apart from prop names, a special value called `modelValue` that comes from the parent.

The `v-model` on a child prop also includes, under the hood, another directive called `modelValue`

`v-bind`: Turns a regularly defined attribute to a parsable javascript for Vue Js. Usually used in passing props between parent and child components. Shortcut is to use just `:`

Receiving props in the child component is done by registering them on the _props_ object in the child component definition.

_Computed_: It is an object defined within a component that has as keys variable names and as values of associated keys as getters and setters that deal with fetching data and handling changes made.

_$emit()_: Allows one to emit events that other components are alble to listen to. Its takes two arguments; type of event being emitted and the value of the argument being passed through.

`v-model` also listens for an update in the subsequent child prop for the particular value. It automatically updates the associated value if a change occur.

