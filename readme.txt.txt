Difference between var and let:

Scope:
var is function-scoped, which means if you declare it inside a function, it can only be accessed within that function. But if declared outside any function, it's globally scoped.
let is block-scoped. This means it can only be accessed within the block (e.g., inside { } like loops or conditionals) where it was defined.
Hoisting:
Both var and let declarations are hoisted to the top of their containing function or block, but while var is initialized with undefined, let is not initialized, leading to a ReferenceError if you try to access it before its declaration.
Re-declaration:
In the same scope, var can be re-declared without any issues, while let cannot.
Difference between var and const:

Scope: Same difference as between var and let.
Mutability:
Variables declared with var are mutable.
Variables declared with const are immutable in the sense that their assignment cannot be changed. However, if the const variable holds an object, the properties of that object can still be modified.
Hoisting: Similar to let, const declarations are also hoisted to the top but are not initialized.
Re-declaration: var can be re-declared in the same scope, but const cannot. Additionally, const requires an initial value at the time of declaration.
Difference between let and const:

Mutability:
let allows re-assignment to the variable.
const does not allow re-assignment after initialization.
Initial Value: const requires an initial value when declared, while let does not.
What is hoisting?

Hoisting is a JavaScript mechanism where variable and function declarations are moved to the top of their containing scope during the compilation phase. However, while the declarations are hoisted, initializations are not. This means that a variable declared and initialized at the bottom of the code can be used at the top because of hoisting, but it will be undefined until the line where it was initialized is executed.

