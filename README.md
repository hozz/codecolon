codecolon
=========

### `]:42` in second-to-last line of code.

Extra space renders in second-to-last line:

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

### `]:` in second-to-last line of code

Extra space still there. Last code line doesn't show at all:

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

### Just `:` or `]` in second-to-last line of code

Renders fine:

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
   [ 'prop_' + (() => 42)() :
};
```

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
   [ 'prop_' + (() => 42)() ]
};
```
