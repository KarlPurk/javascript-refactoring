Replace context variable with bind/call/apply
=============================================
You're using a temporary variable to store a reference to an object so that you can maintain scope in an inner function.

```javascript
Post.prototype.getDateTime = function() {
    var self = this,
        concatDateTime = function() {
            return self.date + ‘ ‘ + self.time;
        };
    return concatDateTime();
};
```

Remove the temporary variable and use ECMAScript 5 bind instead.

```javascript
Post.prototype.getDateTime = function() {
    var concatDateTime = function() {
        return this.date + ‘ ‘ + this.time;
    }.bind(this);
    return concatDateTime();
};
```

Remove the temporary variable and use the ECMAScript 3 call/apply instead.

```javascript
Post.prototype.getDateTime = function() {
    var concatDateTime = function() {
        return this.date + ‘ ‘ + this.time;
    };
    return concatDateTime.call(this);
};
```

# More Information
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/bind
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/call
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/apply
