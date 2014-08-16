Replace switch with object literal
===================================
You’re using a switch statement to conditionally execute a fragment of code.

```javascript
var instance, something = 'dog';
switch (something) {
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
console.log(instance);
```

Replace the switch statement with an object literal.

```javascript
var something = 'dog', 
    factory = {
        dog: Dog,
        cat: Cat,
        person: Person
    },
    instance = new factory[something || 'person']();
console.log(instance);
```

# More Information

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Values,_variables,_and_literals#Object_literals
