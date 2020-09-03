# Operators

Believe it or not you have already seen one operator from our initial example. They are basically symbols that let us perform operations on data. They assume you have something on the left and something of the right of the operator and then you get a result from the operation.

Most of them you are already familiar with assuming you have learnt basic algebra, but here is a list of the common ones with some C# examples.

## `=` Assignment Operator

You have seen this one already, and this is how we assign a value to something, the right hand side of the operator being the value to assign and the left being the place to assign it.

```c#
var a = 10;
```

So as you can see the operator takes the value of 10 and assigns it to the variable `a`.

## `+` Addition Operator

This adds two things together, in most languages these days it's clever enough to know *how* you want those things added.

```c#
var a = 10 + 5;
```

So here we are using 2 operators, but we can ignore the assignment as we know what thats doing, the latter operator is taking 5 and adding it to 10 resulting in `a` being assigned the value 15.

However what if we were to do the same with strings.

```c#
var b = "He" + "llo";
```

You cant really add these together like numbers, so you ideally want them to concatenate (join them together), which would result in the variable `b` being assigned the string value of `Hello`.

> Not all languages support this at the operator level, but most modern ones do, so if you get an error trying to add 2 strings this way it may be that you need to do it via a function (we will cover them shortly).

## `+=` Addition Assignment Operator

This is basically combining the two above operators into one, so I could write the above examples as:

```c#
var a = 10;
a += 5;

var b = "He";
b += "llo";
```

Its a bit convoluted as we need a value already in `a` and `b` to add to it, but this does the same as the above example. Its common to use this when you are wanting to add lots of stuff to an existing variable.

## `==` Equality Operator

This checks to see if two things are equal and returns a **truthy** result (a boolean with `true` or `false`).

```C#
var a = 10 == 8;
var b = 5 == 5;
var c = "Hi" == "Hi";
```

As we can see above a would be a boolean value of `false` because 10 does not equal 8, and `b` would have a value of `true` and finally `c` would be `true` as the contents of both strings are the same.

> Its worth noting here that string comparison with equality operator is not always supported in all languages, as it may have different behaviour. In C# it is case sensitive, so "Hi" and "HI" would not be equal.

Some languages (like JS) also have an `===` operator, which is a more strict equality check, as in the JS world it doesnt treat types as strictly as in other languages (we will cover that topic more later). So in JS you could do:

```js
var a = 1 == "1";
var b = 1 === "1";
```

In this example `a` would be true, as in JS the equality operator checks just if the value can be considered equal, so it's happy to say the integer 1 is the same as a string containing the character 1. However when we use the stricter `===` operator the `b` variable would be false as the types are not the same so it cannot evaluate the values the same way.

> As mentioned not all languages have `===` and some languages treat `==` stricter than others, but for the most part you can assume that any equality operator like above is going to be used for comparing two values and giving a boolean result.

## `!=` NOT Equal operator

This does the opposite of the equality operator and checks to see if two values are NOT equal.

```c#
var a = 10 != 5;
var b = 10 != 10;
```

So here we check if 10 is not equal to 5, and the result for `a` is `true` as they are not equal, however when we compare 10 to 10 the result is equal so it would return a `false` value for `b`.

> In some languages like SQL the Not Equal operator can be `<>` but its more often than not the `!=` symbol.

## `!` Not Operator

This acts as an inverter of sorts for things, so we could have a truthy value and use the `!` operator to invert it, like so:

```c#
var a = !true;
```

So here the boolean `a` has the value of `false` as it's inverted the `true` value. 

## `>` Greater than Operator

This one checks if the left side is greater than the right side and returns a truthy result.

```c#
var a = 10 > 5;
var b = 5 > 10;
```

So `a` is a boolean with the value of `false` and `b` has `true`.

## `<` Less than operator

This one checks to see if the left side is less than the right side and returns a truthy result.

```c#
var a = 10 < 5;
var b = 5 < 10;
```

So `a` is `false` and `b` is `true` here.

## `>=` and `<=` Greater/Less than or Equals operator

So these combine the Greater than and Less than operators with the equality operator so you can also account for values which equal the value you are comparing.

```c#
var a = 10 >= 10;
var b = 10 <= 10;
```

Both would be `true` here as 10 is not greater or less than 10, but it is equal to 10.

## Other operators

There are LOTS of other operators, but rather than bore you with them all now, lets just focus on these simple ones and dive a bit deeper into the more complex and situational ones later.