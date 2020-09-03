# Functions

OK, pat yourself on the back for getting this far. The next bit may seem a bit daunting but once this is out the way we are almost ready to start actually doing some practical code.

## What are functions?

Functions are reusable bits of code that take an input and provide an output.

The inputs are known as **arguments** and the output is known as the **result** and is **returned** from the function. A function can have any amount of **arguments** but in most languages only has one output.

> This isnt to say a function will just return 1 thing, you can have complex scenarios where you want to return lots of contextually relevant data and there are many ways to do that, but we will cover it later.

So lets say you wanted a method that took in 2 numbers and added them togther. Lets have a look at what that function would look like in both C#, JS and Java.

### C# Add function
```c#
int Add(int a, int b)
{ return a + b; }
```
---
### JS Add function
```js
function Add(a, b)
{ return a + b; }
```
---
### Java Add function
```java
int Add(int a, int b)
{ return a + b; }
```

### Similarities

As you can see they are all super similar, the C# and Java functions are idential, and the JS one is syntactically close enough. If we were to have a C++ example that would also be the same as the C# example too.

### Whats actually going on?

So a few new things are at work here, first of all lets focus on the C#/Java/C++ function **signature** which would all be identical.

> The declaration for a function is known as its **signature** which contains what it's input/outputs/name is.

```c#
int Add(int a, int b)
```

So this bit here is saying:

- We want to return an `int` value
- The name of the function is `Add`
- The first argument is an `int` named `a`
- The second argument is an `int` named `b`

So hopefully this seems sensible enough, and if we look at the JS version its doing the same thing just with different syntax.

```js
function Add(a, b)
```

Like the bit above its saying:

- I am declaring a `function`
- The name of the function is `Add`
- The first argument is named `a`
- The second argument is named `b`

Not much different other than we dont have any type information, and this is because C#/Java/C++ and many other languages are known as **statically typed** languages which means you need to explicitly provide typing information and once a variable/argument is created with a type, it is forever that type. However in JS it is known as a **duck/dynamic typed language** and a variable has no explicit type, so you could give a variable an integer value then assign it a string and it would be fine with it, but **statically typed languages** would poop out if you did that.

> This is quite a complex subject, so dont think on it too much for now, at the high level we have shown that 4 different languages all use very similar syntax to achieve the same goal, so keep that in mind and we will discuss static/dynamic typing much more later.

So if we return to the **body** of the function then all of the above examples share the same function body, even JS is the same here.

```c#
{ return a + b; }
```

This is saying:

- Add `a` and `b`
- Return the result

As the type information is contained within the **signature** the body just adheres to that. In JS you could pass in 2 strings and it would add them and return a string, but in C# etc they would not be able to do this as we have explicitly stated it returns an `int`.

## How do we use functions?

GREAT QUESTION! Its really simple and I will show you how to use them in C#, JS and Java.

```c#
var a = Add(10,5);
```

C++ would be ALMOST the same but would look like:

```c++
auto a = Add(10,5);
```
Thats it, all 4 languages are all near identical.

As we have seen before we create a variable called `a` (this is nothing new), and we assign it the result of the function called `Add` giving it a `10` and a `5`.

All languages would end up with `a` being the value `15`.

## Void types

Ok so this may seem a little wacky, and while it is a common type I didn't list it in the previous chapters as its easier to gauge its purpose when looking at it in the context of functions.

So `void` is the absence of a type, so when you have a function like:

```c#
void DoNothing()
{}
```

We are indicating that there will be nothing returned from this function, so when consuming this code we cant assign the value to anything, as there is no value. We are also not giving any arguments, but that has nothing to do with the `void` return type.

> In most languages you can only use the `void` type in the context of function return types, however in certain languages like C++ you can actually use `void` as a variable type which indicates to it that the type is not pre-defined, but this is super advanced and means you are manually managing the way the variables memory should be read.

## WELL DONE CAPTAIN!

You have successfully done a lot of thinking, lets just do a tiny bit more thinking then we can crack on with actually writing some code and learning more stuff.
