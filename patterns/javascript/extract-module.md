Extract module
===============
You have a collection of related functions that can be utilised through a simple interface.

```javascript
var getPostsFromDataSource = function() {
    // Fetch posts from data source
};
var logPosts = function(posts) {
    // Log each post to console
};
var mapPosts = function(posts) {
    // Map each post to a model
};
var getPosts = function() {
    var posts = getPostsFromDataSource();
    posts = mapPosts(posts);
    logPosts(posts);
    return posts;
};
var posts = getPosts();
```

Encapsulate the functions in a new function and return a fine-grained interface for clients.

```javascript
var postsModule = function() {
  var getPostsFromDataSource = function() {
      // Fetch posts from data source
  };
  var logPosts = function(posts) {
      // Log each post to console
  };
  var mapPosts = function(posts) {
      // Map each post to a model
  };
  var getPosts = function() {
      var posts = getPostsFromDataSource();
      posts = mapPosts(posts);
      logPosts(posts);
      return posts;
  };
  return {
  	getPosts: getPosts
  };
}();
var posts = postsModule.getPosts();
```

# More Information
- http://addyosmani.com/largescalejavascript/#modpattern
