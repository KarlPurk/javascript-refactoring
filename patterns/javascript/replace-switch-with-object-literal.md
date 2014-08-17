Replace switch with object literal
===================================
You’re using a switch statement to conditionally execute a fragment of code.

```javascript
var factory = function(key) {
    var instance;
    switch (key) {
        case 'dog':
            instance = new Dog();
            break;
        case 'cat':
            instance = new Cat();
            break;
        default:
            instance = new Person();
            break;
    }
    return instance;
}
console.log(factory('dog'));
```

Replace the switch statement with an object literal.

```javascript
var factory = function(key) {
    var map = {
        dog: Dog,
        cat: Cat,
        person: Person
    };
    return new map[map.hasOwnProperty(key) ? key : 'person']();
};
console.log(factory('dog'));
```

# More Information

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Values,_variables,_and_literals#Object_literals
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/hasOwnProperty
