# Lesson 3

## Logical Operators

Now that you're familiar with data types, let's utroduce some operators. We will start with the logical operators:

* OR `||`
* AND `&&`
* NOT `!`

OR works like this:

```js
true || false == true
false || true == true
true || true == true
false || false == false
```

AND works like this:

```js
true && true == true
false && false == false
true && false == false
false && true == false
```

For example, if you want to see if both `var1` and `var2` are true, you can do something like

```js

let var1 = true
let var2 = true

console.log(var1==true && var2==true) // == is the euality operator
```

The last statement can be simplified to 

```js
console.log(var1 && var2)
```

Now, let's see what happens when we want to check if either one variable is set to true

```js
console.log(var1 || var2)
```

Chance var2 to false:

```js
var2 = false
```

And examine both logical expressions.

```js
console.log(var1 && var2)
console.log(var1 || var2)
```

NOT operator works like this:

```js
true == !false
false == !true
```

Let's try it out.

```js
console.log(!var1, !var2)
console.log(!var1 && !var2)
console.log(!var1 || !var2)
```
