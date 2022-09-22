# Class 07 Reading Notes *(9/../22)*

[*back*](../README.md)

## Functions

A function

``` JS
function myFunction(p1, p2) {
  return p1 * p2;   // The function returns the product of p1 and p2
}
```

``` Js
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```

The code inside the function will execute when "something" invokes (calls) the function:

- When an event occurs (when a user clicks a button)
- When it is invoked (called) from JavaScript code
- Automatically (self invoked)

return

- When JavaScript reaches a return statement, the function will stop executing. If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement. Functions often compute a return value. The return value is "returned" back to the "caller"

## Variables

- Local Var

``` JS
// code here can NOT use carName

function myFunction() {
  let carName = "Volvo";
  // code here CAN use carName
}

// code here can NOT use carName
```

- Public var

``` Js
  let carName = "Volvo";
// code here CAN use carName

function myFunction() {
  // code here CAN use carName
}

// code here CAN use carName
```

[Operators](https://www.w3schools.com/js/js_operators.asp)

[More Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)