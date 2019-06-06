# Lesson 4

## Objects

One important data type we haven't covered yet are objects. Objects are comprised of other elements, that can be accessed by names, called keys. For example,

```js
let myObj = {}
```

Will create an empty object. You will find it the index.js. Let's print it.

```js
console.log(myObj)
```

What did it print?

### Keys and Values

Let's assign some values to the object keys

```js
myObj.key1 = 1
myObj['key2'] = 2.0
myObj["stringkey"] = "stringvalue"
myObj.chicken = {egg:1}
myObj.bool = false
```

Print the contents of this object. Did you notice that objects, like arrays, can hold elements of different types? Did you notice, that the `chicken` key was initialized with an object value?

### Creating objects

Like in the example above, you can create objects using a number of ways
```js
let moObj1 = {}
let myObj2 = new Object()
let myObj3 = {key1:3, name: "John"}
```

In the last example, you will not only create an object, but also will initialize a key `key1` with a value of `3` and a `name` key with a value of "John".

### Retrieving values

Let's print somve object properties (where corresponding keys are property names).

```js
console.log(myObj.key1)
console.log(myObj["key1"])

let key="key1"
console.log(myObj[key])
```

As you can see, the same exact key can be accessed in a number of different ways.

### Removing keys

It is possible to dynamically remove a property by deleting it's key.

```js
delete myObj["key1"]
```

Now print this object out. Which value corresonds to `key1`?

