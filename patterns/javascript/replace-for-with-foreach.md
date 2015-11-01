Replace for with forEach
=========================

You're using the `for` statement to iterate a collection.

```javascript
var i, item, items = [1, 2, 3];
for (i = 0; i < items.length; i++) {
    item = items[i];
    console.log(item);
}
```

Use the ECMAScript 5 `forEach` method instead.

```javascript
[1, 2, 3].forEach(function(item) {
    console.log(item);
});
```

If you depend on the context of `this` then pass in context as the second parameter, or `bind` context to the function

```javascript
{
  honorific: 'Ms.',
  surnames: ['Jones', 'Smith'],
  logNames: function(){
    this.surnames.forEach(function(name){
        console.log(this.honorific+' '+name); // 'Ms. Jones', 'Ms. Smith'
    }, this) // forEach runs in global context by default, 'undefined Jones', 'undefined Smith'; or is undefined in strict mode, causing an error
  }
}
```

# More Information

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach
