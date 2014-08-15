JavaScript Refactoring Patterns
=======================
A collection of JavaScript refactoring patterns for improving the design of existing JavaScript code.

This work is greatly motivated by, and many patterns are adapted from, Martin Fowlers excellent book Refactoring - Improving the design of existing code.

# Overview of Refactoring Patterns

## General Patterns
- Extract function/method
- Replace temp with query
- Introduce explaining variable
- Split temporary variable
- Remove assignments to parameters

## JavaScript Patterns

### ECMA 3
 - Replace switch with object literal

### ECMA 5
- Replace for loop with forEach
- Replace aggregate property operations with reduce
- Replace direct array access element updates with map
- Replace context variable with bind/call/apply
- Extract module

### ECMA 6
- Replace nested async callbacks with promises

### jQuery
- Replace jQuery selector with querySelector/querySelectorAll
