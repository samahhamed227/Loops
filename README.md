# Loops
# Operators
JavaScript has the following types of operators. This section describes the operators and contains information about operator precedence.

* Assignment operators: 
* Comparison operators : Equal (==)	/Not equal (!=)	/Strict equal (===)	Returns true if the operands are equal and of the same type. See also Object.is and sameness in JS/Strict not equal (!==)	/Greater than (>)	/Greater than or equal (>=)	/Less than (<)	/Less than or equal (<=)	
* Arithmetic operators : Remainder (%)	 /Increment (++)	/Decrement (--)	 /Unary negation (-)	/Unary plus (+)	/Exponentiation operator (**)	
* Bitwise operators : Bitwise AND	a & b /Bitwise OR	a | b/ Bitwise XOR	a ^ b/Bitwise NOT	~ a/ Left shift	a << b/Sign-propagating right shift	a >> b/Zero-fill right shift	a >>> b
* Logical operators : Logical AND (&&) /Logical OR (||)/Logical NOT (!)
* String operators : For example :console.log('my ' + 'string')
* Conditional (ternary) operator :The conditional operator is the only JavaScript operator that takes three operands. The operator can have one of two values based on a condition. The syntax is:condition ? val1 : val2
## example : var status = (age >= 18) ? 'adult' : 'minor';

* Comma operator :The comma operator (,) evaluates both of its operands and returns the value of the last operand. This operator is primarily used inside a for loop, to allow multiple variables to be updated each time through the loop. It is regarded bad style to use it elsewhere, when it is not necessary. Often two separate statements can and should be used instead. 

* Unary operators :A unary operation is an operation with only one operand.
* Relational operators :

### Examples
The return value matches the expression to the right of the = sign in the “Meaning” column of the table above. That means that (x = y) returns y, (x += y) returns the resulting sum x + y, (x **= y) returns the resulting power x ** y, and so on.

In the case of logical assignments, (x &&= y), (x ||= y), and (x ??= y), the return value is that of the logical operation without the assignment, so x && y, x || y, and x ?? y, respectively.

# Destructuring
For more complex assignments, the destructuring assignment syntax is a JavaScript expression that makes it possible to extract data from arrays or objects using a syntax that mirrors the construction of array and object literals.
 ### Example :var foo = ['one', 'two', 'three'];
 
 
 # Loop 
 The statements for loops provided in JavaScript are:

1. for statement
2. do...while statement
3. while statement
4. labeled statement
5. break statement
6. continue statement
7. for...in statement
8. for...of statement


# for statement : 
When a for loop executes, the following occurs:

The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. If the value of condition is false, the for loop terminates. (If the condition expression is omitted entirely, the condition is assumed to be true.)
The statement executes. To execute multiple statements, use a block statement ({ ... }) to group those statements.
If present, the update expression incrementExpression is executed.
Control returns to Step 2.

 
 # do...while statement
statement is always executed once before the condition is checked. (To execute multiple statements, use a block statement ({ ... }) to group those statements.)

If condition is true, the statement executes again. At the end of every execution, the condition is checked. When the condition is false, execution stops, and control passes to the statement following do...while.

# while statement
If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.

The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following while.

# labeled statement
A label provides a statement with an identifier that lets you refer to it elsewhere in your program. For example, you can use a label to identify a loop, and then use the break or continue statements to indicate whether a program should interrupt the loop or continue its execution.

# break statement
Use the break statement to terminate a loop, switch, or in conjunction with a labeled statement.

When you use break without a label, it terminates the innermost enclosing while, do-while, for, or switch immediately and transfers control to the following statement.
When you use break with a label, it terminates the specified labeled statement.
# continue statement
The continue statement can be used to restart a while, do-while, for, or label statement.

When you use continue without a label, it terminates the current iteration of the innermost enclosing while, do-while, or for statement and continues execution of the loop with the next iteration. In contrast to the break statement, continue does not terminate the execution of the loop entirely. In a while loop, it jumps back to the condition. In a for loop, it jumps to the increment-expression.
When you use continue with a label, it applies to the looping statement identified with that label.
 
 # for...in statement
The for...in statement iterates a specified variable over all the enumerable properties of an object. For each distinct property, JavaScript executes the specified statements. A for...in statement looks as follows:

for (variable in object)
  statement
  
  # Arrays
Although it may be tempting to use this as a way to iterate over Array elements, the for...in statement will return the name of your user-defined properties in addition to the numeric indexes.

Therefore, it is better to use a traditional for loop with a numeric index when iterating over arrays, because the for...in statement iterates over user-defined properties in addition to the array elements, if you modify the Array object (such as adding custom properties or methods).

# for...of statement
The for...of statement creates a loop Iterating over iterable objects (including Array, Map, Set, arguments object and so on), invoking a custom iteration hook with statements to be executed for the value of each distinct property.

