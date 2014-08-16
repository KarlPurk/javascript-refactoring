Replace for with forEach
=========================

You're using the `for` statement to iterate a collection.

```javascript
var i, item, items = [1, 2, 3];
for (var i = 0; i < items.length; i++) {
    var item = items[i];
    console.log(item);
}
```

Use the ECMAScript 5 `forEach` method instead.

```javascript
[1, 2, 3].forEach(function(item) {
    console.log(item);
});
```

# References

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach
