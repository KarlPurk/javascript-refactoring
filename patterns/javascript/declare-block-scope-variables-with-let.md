# Declare block scope variables with let

You're using `var` to declare variables within a block:

```javascript

var i, max = 10;

for (i = 0; i < max; i++) {
    var timesLooped = i + 1;
    console.log('Times looped:', timesLooped);
}

```

Use ES6 `let` instead:

```javascript

var i, max = 10;

for (i = 0; i < max; i++) {
    let timesLooped = i + 1;
    console.log('Times looped:', timesLooped);
}

```


# More Information

- https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Statements/let
- https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Statements/var
