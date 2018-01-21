This week I finally learned that currying allows you to wrap functionality into neatly nested pieces of code.  

This is done by passing multiple arguments (a tuple) through a sequence of functions, each with a single argument.  This can be illustrated with a series of additive functions, for example:

We define the function to take in a tuple of arguments (a, b, c) with the result of this function to add the arguments.

`let curryAdd = a => b => c=> => a + b + c;`

And when invoked with three arguments, they are added together to get 9.

`curryAdd(2)(3)(4)` = `9`

An interesting application of this is by creating a partial, that is a function that can be provided a partial amount of arguments and produce deterministic, but perhaps counterintuitive results.

If we reassign curryAdd, giving it an argument of 10:

`let partial = curryAdd(10)`

And invoke the function with a series of 3 arguments

`partial(2)(3)(4)`

The argument of 10 that we provided it in the reassignment with be the actual argument passed in place of all three of the above integers for the result of

`partial(10)(10)(10)` = `30`

