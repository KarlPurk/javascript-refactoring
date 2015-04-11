Introduce Explaining Variable
==============================

You have a complicated expression that can be simplified.

```javascript
  if (device.platform.toUpperCase() === 'IOS' && 
      device.platform.version < 7 && 
      device.browser.toUpperCase() === 'CHROME') {
```

Simplify the expression by introducing variables that clearly explain each condition:

```javascript
  var isTargetPlatform = device.platform.toUpperCase() === 'IOS';
  var isTargetVersion = device.platform.version < 7
  var isTargetBrowser = device.browser.toUpperCase() === 'CHROME';
  
  if (isTargetPlatform && isTargetVersion && isTargetBrowser) {
```

# More Information

- http://refactoring.com/catalog/extractVariable.html
- https://sourcemaking.com/refactoring/introduce-explaining-variable
