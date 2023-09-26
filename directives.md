# Vue.js Directives list
Directive attribute values are expected to be single JavaScript expressions (with the exception of v-for, v-on and v-slot, which will be discussed in their respective sections later)

## 1: v-html
this directive is used to pring raw html. however you cannot use this directive to compose
html partials as vue is not string based templating engine.

## 2: v-bind:attr / :attr (shorthand)
use this to bind attributes to any html element. this is a property

## 3: v-if:
used for conditional rendering the element.reactive

## v-on: / @eventName (shorthand)
used for click handling or other event handling