codecolon
=========

**`]:42` Extra space renders in second-to-last line:**

```JavaScript
var obj = {
   // __proto__
   __proto__: theProtoObj,
   // Shorthand for ‘handler: handler’
   handler,
   // Methods
   toString() {
     // Super calls
     return "d " + super.toString();
   },
   // Computed (dynamic) property names
   [ 'prop_' + (() => 42)() ]:42
};
```

**`]:` Space still there, but last line doesn't show at all:**

```JavaScript
var obj = {
   // __proto__
   __proto__: theProtoObj,
   // Shorthand for ‘handler: handler’
   handler,
   // Methods
   toString() {
     // Super calls
     return "d " + super.toString();
   },
   // Computed (dynamic) property names
   [ 'prop_' + (() => 42)() ]:
};
```
