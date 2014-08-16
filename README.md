JavaScript Refactoring Patterns
=======================
A collection of refactoring patterns for improving the design of existing JavaScript code.

This work is greatly motivated by, and many patterns are adapted from, Martin Fowler's excellent book Refactoring - Improving the design of existing code.

# Overview of Refactoring Patterns

## General Patterns
- [Extract function/method](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/general/extract-method.md)
- Replace temp with query
- Introduce explaining variable
- Split temporary variable
- Remove assignments to parameters

## JavaScript Patterns

### ECMAScript 3
 - [Replace switch with object literal](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/javascript/replace-switch-with-object-literal.md)

### ECMAScript 5
- [Replace for with forEach](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/javascript/replace-for-with-foreach.md)
- [Replace aggregate property operations with reduce](https://github.com/KarlPurk/javascript-refactoring/blob/master/patterns/javascript/replace-aggregate-property-operations-with-reduce.md)
- Replace direct array access element updates with map
- Replace context variable with bind/call/apply
- Extract module

### ECMAScript 6
- Replace nested async callbacks with promises

### jQuery
- Replace jQuery selector with querySelector/querySelectorAll
