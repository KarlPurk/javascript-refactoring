Replace aggregate property operations with reduce
==================================================
You’re iterating a collection to perform an aggregate query, using a temporary variable to record the results.

```javascript
var result = 0;
[1, 2, 3].forEach(function(item) {
    result += item;
});
console.log(result);
```

Remove the temporary variable and use the ECMAScript 5 reduce method instead.

```javascript
var result = [1, 2, 3].reduce(function(prev, cur) {
    return prev + cur;
}, 0);
console.log(result);
```

# More Information

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce
