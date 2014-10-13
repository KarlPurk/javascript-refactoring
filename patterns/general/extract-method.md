Extract method/function
========================

You have a code fragment that can be grouped together.

```javascript
var posts = getPosts();
posts.forEach(function(post) {
    console.log(post);
});
```

Extract the fragment into a new function/method.

```javascript
var logPosts = function(posts) {
    posts.forEach(function(post) {
        console.log(post);
    });
};

var posts = getPosts();
logPosts(posts);
```

# More Information

- Martin Fowler, Refactoring - Improving the design of existing code (Addison-Wesley, 2007), p.110.
- http://refactoring.com/catalog/extractMethod.html
