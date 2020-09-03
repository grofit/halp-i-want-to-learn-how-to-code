# Variables Round 2

As the last chapter mentioned variables are common in almost all languages, and also most of the syntax is. For example here is the same example from the previous chapter in 3 other languages.

---
### Javascript (JS)
```js
var someNumber = 1;
```
---
### CSharp (C#)
```js
var someNumber = 1;
```
---
### Java
```java
int someNumber = 1;
```
---
### C Plus Plus (C++)
```c++
int someNumber = 1;
```
---

## Similarities

So as you can see the above code is almost identical between 4 different mainstream languages. The only real difference is the use of `var` vs `int` to indicate the type of the variable.

Certain languages handle variable allocations differently, so for example in C# you can either provide the variable type yourself or you can use `var` and let the computer infer what the type should be based off the value.

> I'm overly simplifying a bit here, most programming languages are **built** with a **compiler** which takes the code and compiles it into something a computer can understand, and its actually the compiler which does the inferring here.

If you remember back in the previous chapter we mentioned that numeric types are often **integers** or **floats** and in this case the `int` code indicates we want this variable to treat its values as **integers**.

> C++ and Java do actually allow you to infer the type in newer versions but historically they are more rigid on types with variable declarations. To do this we would replace `int` with `var` for Java and `auto` for C++

Other than the data type changes the rest of the syntax is the same, and this is one reason why i'm keen to try and teach how to program with this in mind. As a lot of the time tutorials are **LEARN JAVA IN 30 DAYS** or **LEARN C++ IN 50 YEARS** which is great when you want to just learn a single language, but I feel its better for you to see multiple languages at once and see just how similar everything is between them all.

In the long run this helps you break out from the `"I'm a <insert language> dev"` and instead just be a programmer who can pick up most common languages and hit the ground running.

## String variables

Lets do the same as above but using string data.

---
### Javascript (JS)
```js
var someString = "hello";
```
---
### CSharp (C#)
```js
var someNumber = "hello";
```
---
### Java
```java
String someNumber = "hello";
```
---

As you can see the majority of the code is the same, like before we tell the computer we want to assign a variable (in Java we tell it explicitly what type), then give it a name and assign it a string, but do you notice that we wrap it in quotes. This is because we want this text to be treated as text instead of as code.

For giggles lets take away the quote marks and see what it looks like in JS.

```js
var someString = hello;
```

So now it treats `hello` as code, which in this case would look for a variable called `hello` and try to assign its value to `someString`. In this example we dont have a variable names `hello` so it would blow up and tell you off.

> You may have also noticed I didn't include C++ in the examples here, and thats because in C++ it doesn't really have a built in `String` type without pulling in other **Libraries** or using **Pointers**, which are both waaaaay down the line for now.

Ultimately you can see here that we are always following the same conventions for creating variables.

1. Create a variable
2. Give it a name
3. Give it a value

If its a number we can just put the number in as the value, but if its a string we need to put it in quotations.
