The statement "use strict"; instructs the browser to use the Strict mode, which is a reduced and safer feature set of JavaScript.

**List of features (non-exhaustive)**

Disallows global variables. `(Catches missing var declarations and typos in variable names)`

Silent failing assignments will throw error in strict mode `(assigning NaN = 5;)`

Attempts to delete undeletable properties will throw `(delete Object.prototype)`

Requires all property names in an object literal to be unique `(var x = {x1: "1", x1: "2"})`

Function parameter names must be unique `(function sum (x, x) {...})`

Forbids octal syntax `(var x = 023; some devs assume wrongly that a preceding zero does nothing to change the number.)`

Forbids the with keyword

eval in strict mode does not introduce new variables

Forbids deleting plain names `(delete x;)`

Forbids binding or assignment of the names eval and arguments in any form

Strict mode does not alias properties of the arguments object with the formal parameters. `(i.e. in function sum (a,b) { return arguments[0] + b;} This works because arguments[0] is bound to a and so on. )`

arguments.callee is not supported
