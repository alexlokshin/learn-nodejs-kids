# Lesson 3

In this lesson we will learn basic Javascript data types, attempt to populate them, and display the data contained in variables of those types.

You need to work in `index.js`. When done, run it with `node index.js` from your terminal. 

We will study the following data types:
* number
* string
* boolean
* array
* undefined
* null

## Declaring a variable
To declare a variable, you can do something like

```js
let myVariable = "Hello World"
```

Notice that semicolon at the end is optional. This could be also written as 

```js
let myVariable = "Hello World";
```

## String

This type has something to do with text. Declare a variable in `index.js` (just like in the example above), and print it:

```js
console.log("myVariable:", myVariable)
```

Run the program `node index.js`. What did it print?

## Number

This data type is used in numeric calculations. Declare a variable:

```js
let myNumber = 3
```

Print it. 

Now let's try the same with a decimal digit number. Change `3` to `3.1`. Run the program again.

Try adding numbers together. Like this

```
myNumber = myNumber + 1.1
```

Print the value. What did it print? We will go over numeric operations in future lessons.


## Boolean

This data type is used in logical calculation, and takes the values of `true` and `false`.

Declare a boolean variable, and print it's value. Lets evaluate some facts.

```
console.log("Is this true 1==1?", 1==1) // == is an equality operator
console.log("Is this true 1==2?", 1==2)
console.log('Is this true "chicken"=="chicken"?', "chicken"=="chicken") // Double and single quotes are interchangeable
console.log('Is this true "chicken"=="fish"?', "chicken"=="fish")
console.log("Is this true true && true?", true && true) // && is a boolean AND operator
console.log("Is this true true || false?", true || false) // || is a boolean OR operator
console.log("Is this true !true?", !true) // ! is a boolean NOT operator
```

## Array

This data type holds a collection of items. Arrays could contain data elements of different types. Like this:

```js
var myArray = ["chicken", "fish", 1.0, true, [1,2,3]]
```

Let's loop through this array and print the values:

```js
for (var i=0; i<myArray.length; i++){
    console.log(myArray[i])
}
```

Run the program. What did it print?

To add items to the array you can do something like

```js
myArray.push("abc")
```

To remove elements from an array, do this
```js
let lastElement = myArray.pop()
```

It will return a last element of the array (if the array is not empty).

## Undefined

Undefined is a special type, it indicates a variable holds no value. For example, declare a new variable

```js
var undefinedVariable
```

And print its value.

## Null

Null is a special type, it indicates a variable is a reference to no object. Assign a vairable like this

```js
let myNullVariable = null   
```

And print its value.