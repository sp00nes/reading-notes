# Class 08 Reading Notes *(9/22/22)*

[*back*](../README.md)

## Expressions and Operators

At a high level, an expression is a valid unit of code that resolves to a value. There are two types of expressions: those that have side effects (such as assigning values) and those that purely evaluate.

- Assignment operators
  - An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = f() is an assignment expression that assigns the value of f() to x.

  [Assignment Ops EX](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

- Comparison operators
  - A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values. Strings are compared based on standard lexicographical ordering, using Unicode values. In most cases, if the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type for the comparison. This behavior generally results in comparing the operands numerically. The sole exceptions to type conversion within comparisons involve the === and !== operators, which perform strict equality and inequality comparisons. These operators do not attempt to convert the operands to compatible types before checking equality. The following table describes the comparison operators in terms of this sample code:

  [Comparison Ops EX](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

## Loops

### For Loops

``` JS
for (let step = 0; step < 5; step++) {
  // Runs 5 times, with values of step 0 through 4.
  console.log('Walking east one step');
}
```

Syntax

``` JS
for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement
```

When a for loop executes, the following occurs:

- The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
- The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. Otherwise, the for loop terminates. (If the conditionExpression expression is omitted entirely, the condition is assumed to be true.)
- The statement executes. To execute multiple statements, use a block statement ({ }) to group those statements.
- If present, the update expression incrementExpression is executed.
- Control returns to Step 2.

### While loops

A while statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:

``` JS
while (condition)
  statement
```

``` JS
let n = 0;
let x = 0;
while (n < 3) {
  n++; //adds one to n
  x += n; //adds the value and assigns the new value to var x
}
```

[Comparison Ops EX](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)
