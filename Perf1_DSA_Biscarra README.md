1.JavaScript uses  var ,  let , and  const  to declare variables, but they differ in scope and mutability.   var  has function or global scope, meaning it's accessible throughout its function or globally if declared outside any function.  In contrast,  let  and  const  have block scope, limited to the block of code (within curly braces  {} ) where they're declared.   const  variables must be initialized upon declaration and cannot be reassigned, making them ideal for constants.   let  variables can be reassigned, allowing for value changes after initialization.  Modern JavaScript best practices generally recommend using  let  and  const  over  var  to avoid hoisting issues and to improve code clarity and maintainability due to their more predictable scoping behavior.  Using  const  by default and only resorting to  let  when reassignment is truly necessary is a good guideline.

References:
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var

2.In JavaScript, a falsy value is one that evaluates to  false  in a Boolean context.  This doesn't mean the value is  false , but that it behaves like  false  in conditional statements (e.g.,  if ,  while ).  Understanding falsy values is crucial for writing reliable JavaScript code, as they can lead to unexpected behavior if mishandled.There are six falsy values in JavaScript:  false ,  0  (zero),  -0  (negative zero),  0n  (BigInt zero),  ""  (empty string),  null ,  undefined , and  NaN .  These values, when used in a conditional expression, will cause the conditional block to not execute.
 

Examples:
if (0) { console.log("This won't execute"); }
if (null) { console.log("This won't execute"); }
if ("") { console.log("This won't execute"); }
 
 
Why are these falsy?
 
The reasons for these values being falsy are rooted in JavaScript's design and historical context.   false ,  null , and  undefined  represent the absence or lack of a value.   0  and  ""  represent empty numerical and string quantities, respectively.   NaN  represents an invalid numerical result.

Reference:
https://developer.mozilla.org/en-US/docs/Glossary/Falsy
