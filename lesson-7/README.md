# Lesson 7

## String operators and operations

This section is rather short, but it is followed by a test.

### String operators

String concatenation is performed by using the `+` operators on two strings. If one of the arguments is not a string, it will be converted to it. For example, identical results will be printed for both statements:

```js
console.log("chicken"+"1")
```

and

```js
console.log("chicken"+1)
```

Task:

Declare an array and a string variable

```js
let myString = "chicken"
let myArray = [1,2,3]
```

Concatenate the two, and explain what you see.


### Operations

There are a couple of useful operations you can invoke on a piece of text. For example, you can calculate it's length.

```js
let len = "chicken".length
```

Or check the position of one sting within the other:

```js
let pos = "chicken".indexOf("ck")
```

You can get a portion of text, using start and end positions:

```js
let subString = "chicken".slice(2,4)
```

Notice, that indices are zero-based, i.e. the very first character is in position 0. This method will return `ic`. Explain, why. Hint: How many characters will `chicken.slice(0,1)` return?

Another useful method is `replace`. It will replace all occurences of a substing within a string. Like this:

```js
"chicken".replace("c","www")
```

Print this value, what do you see?

There's a way to remove a substring, by replacing it with a blank value. Remember, all occurrences will be replaced.

```js
"chicken".replace("ch","")
```

As a resultant of any such call is a string, you can chain funciton calls.

```js
"chicken".replace("ch","").replace("ck","").indexOf("c")
```

Finally, a very useful function that splits the string into an array of strings: `split`. It works like this:

```js
"chicken|beef|pork|fish".split("|")
```

This expression is equivalent to the value of this array

```js
["chicken,beef,pork,fish"]
```

## Quiz

Empty out index.js, and write a simple program, that
* Converts `My name is Jerry Seinfeld` to `His name is George Costanza`
* Removes `His name is ` from the resultant
* Prints the length of the final string
* Prints the number of words in the final string