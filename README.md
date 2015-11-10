JavaScript Refactoring Patterns
=======================
A collection of refactoring patterns for improving the design of existing JavaScript code.

This work is greatly motivated by, and many patterns are adapted from, Martin Fowler's excellent book Refactoring - Improving the design of existing code.

# Overview of Refactoring Patterns

## General Patterns
These refactorings are ported to JavaScript from Martin Fowler's book Refactoring - Improving the design of existing code.  Although they are not JavaScript specific they are still great refactorings which can help to improve the design of JavaScript code.

### Composing Methods
- [Extract function/method](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/general/extract-method.md)
- [Replace temp with query](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/general/replace-temp-with-query.md)
- [Introduce explaining variable](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/general/introduce-explaining-variable.md)
- Split temporary variable
- Remove assignments to parameters

## JavaScript Patterns
These refactorings are JavaScript specific and should help to improve the design of your code.  The refactorings are grouped by the ECMAScript version that implements the functionality that they depend on.  

### ECMAScript 3
- [Replace switch with object literal](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/javascript/replace-switch-with-object-literal.md)
- [Extract module](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/javascript/extract-module.md)

### ECMAScript 5
- [Replace for with forEach](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/javascript/replace-for-with-foreach.md)
- [Replace aggregate property operations with reduce](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/javascript/replace-aggregate-property-operations-with-reduce.md)
- [Replace direct array access element updates with map](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/javascript/replace-direct-array-access-element-updates-with-map.md)
- [Replace context variable with bind/call/apply](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/javascript/replace-context-variable-with-bind-call-apply.md)

### ECMAScript 6
- [Declare block scope variables with let](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/javascript/declare-block-scope-variables-with-let.md)
- [Replace default param logic with ES6 default params](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/javascript/replace-default-param-logic-with-es6-default-params.md)
- Replace nested async callbacks with promises

### jQuery
- [Replace jQuery selector with querySelector/querySelectorAll](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/javascript/replace-jquery-selector-with-query-selector.md)
