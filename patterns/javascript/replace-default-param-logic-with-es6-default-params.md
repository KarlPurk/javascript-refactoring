# Replace default parameter logic with ES6 default parameters

Your using the `or` operator to provide a default value.

```javascript
function getPrice(price, shippingFee) {
    shippingFee = shippingFee || 9.99;
    return price + shippingFee;
}
```

You're using an `if` statement to provide a default value.

```javascript
function getPrice(price, shippingFee) {
    if (!shippingFee) {
        shippingFee = 9.99;
    }
    return price + shippingFee;
}
```

Use the ES6 default value syntax instead.

```javascript
function getPrice(price, shippingFee = 9.99) {
    return price + shippingFee;
}
```

# More Information

- [https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Functions/default_parameters](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Functions/default_parameters)
