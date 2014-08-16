Replace direct array access element updates with map
=====================================================
You’re iterating over an array and then performing updates on the source array directly.

```javascript
var counts = [5, 7, 13];
counts.forEach(function(value, index) {
    counts[index]++;
});
console.log(counts);
```

Use the ECMAScript 5 map method instead:

```javascript
var counts = [5, 7, 13];
counts = counts.map(function(value, index) {
    return value + 1;
});
console.log(counts);
```

# More Information

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map
