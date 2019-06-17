# Lesson 8

## Functions

Javascript functions are helpful when code needs to be re-used or broken up into smaller pieces. For example, let's define a function that calculates the sum of two operands.

```js
function sum(a1, a2){
    return a1+a2
}
```

Here's a great case for reuse:

```js
console.log(sum(1,2))
console.log(sum(1,3))
console.log(sum(5,8))
```

However, since types are not enforced, you can do this:

```js
console.log(sum("chicken","fish"))
```

What did it print?

To fix this side effect, let's make sure the arguments passed into the function are numbers. This can be done using a built-in function called `isNaN()`. It stands of `is not a number`. We just need to negate it's output to check for numbers.

```js
function sum(a1, a2){
    if (!isNaN(a1) && !isNaN(a2)){
        return a1+a2
    } else {
        return 0
    }
}
```

Let's re-run the code. What did this print?

```js
console.log(sum("chicken","fish"))
```

* Quiz: explain this.

```js
console.log(sum(5.1,8.2))
```

Functions do not have to return anything. Like this one:

```js
function noReturn(){
    console.log("Doesn't return anything!")
}
```

Another interesting fact about functions, is that they are objects themselves.

```js
var noReturn = function(){
    console.log("Doesn't return anything!")
}
// Let's call it
noReturn()
noReturn()
```