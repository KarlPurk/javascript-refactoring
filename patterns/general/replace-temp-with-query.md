Replace temp with query
========================
You’re storing the result of an expression in a temporary variable.

```javascript
var price = items.getPrice() + shipping.getTax();
updateTotalPrice(price);
```

Replace the temporary variable with a query.

```javascript
var getTotalPrice = function(items, shipping) {
    return items.getPrice() + shipping.getTax();
}
updateTotalPrice(getTotalPrice(items, shipping));
```

# More Information
- Martin Fowler, Refactoring - Improving the design of existing code (Addison-Wesley, 2007), p.120.
- http://refactoring.com/catalog/replaceTempWithQuery.html
