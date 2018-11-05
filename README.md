# CALL METHOD
~~~
The call method calls a function with a given this value and arguments provided individually.
Syntax
function.call(thisArg, arg1, arg2, ...)
The call() allows for a function/method belonging to one object to be assigned and called for a different object.
~~~
# APPLY METHOD
~~~
The apply() method calls a function with a given this value, and arguments provided as an array (or an array-like object).

Syntax
function.apply(thisArg, [argsArray])

# Using apply to append an array to another
1 We can use push to append an element to an array.
2 push accepts a variable number of arguments, we can also push multiple elements at once.
EXAMPLE
var array = ['a', 'b'];
var elements = [0, 1, 2];
array.push.apply(array, elements);
console.log(array);

~~~
# BIND METHOD
~~~
The bind method creates a new function that, when called, has its this keyword set to the provided value, with a given sequence of arguments preceding any provided when the new function is called.

Syntax
function.bind(thisArg[, arg1[, arg2[, ...]]])


The bind() function creates a new bound function (BF). A BF is an exotic function object (a term from ECMAScript 2015) that wraps the original function object. Calling a BF generally results in the execution of its wrapped function.
A BF has the following internal properties:

[[BoundTargetFunction]] - the wrapped function object;
[[BoundThis]] - the value that is always passed as this value when calling the wrapped function.
[[BoundArguments]] - a list of values whose elements are used as the first arguments to any call to the wrapped function.
[[Call]] - executes code associated with this object.
 Invoked via a function call expression. 
 The arguments to the internal method are a this value and a list containing the arguments passed to the function by a call expression.
~~~
# QUESTION
~~~
What is the difference between .call and .apply?
ANS  call and .apply are considered a method of function object.
.call
Count the number of arguments with call method. It accepts one or more arguments as objects.
.apply 
To use an array as an argument.
It requires an array as its 2nd argument.
~~~
# QUESTION
~~~
What is the difference between .call/.apply, and .bind?
.call=The call method calls a function with a given this value and arguments provided individually.

.apply=The apply() method calls a function with a given this value, and arguments provided as an array (or an array-like object).

.Bind=A bind function is basically which binds the context of something and then stores it into a variable for execution at a later stage.
~~~

# ASKED QUESTION
bind()
This Binding






