# Replace jQuery selectors with the querySelector/querySelectorAll

You're using jQuery to select elements.

```js
var oneElement = $('.element-one');
var allElements = $('element');
```

Use the Selectors API instead:

```js
  var oneElement = document.querySelector('.element-one');
  var oneElement = document.querySelectorAll('.element');
```

# More Information

- https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector
- https://developer.mozilla.org/en-US/docs/Web/API/document.querySelectorAll
- https://developer.mozilla.org/en-US/docs/Web/API/element.querySelector
- https://developer.mozilla.org/en-US/docs/Web/API/element.querySelectorAll
