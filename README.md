Class.js
========

[Simple JavaScript Inheritance](http://ejohn.org/blog/simple-javascript-inheritance/) by John Resig, 
extended to include event binding and triggers.

```javascript
var Foo = Class.extend({});

var foo = new Foo();

foo.addEventListener("changed", function(data){
    alert("New color is " + data.color);
});

foo.trigger("changed", {"color": "red"})

```

jQuery-style `.on("event1 event2", callback)` is also supported.