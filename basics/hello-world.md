# Hello World

So its a huge tradition in programming to always make a "hello world" application in a language when you are first learning it. Ultimately it is an applicaiton which just prints "Hello World" on the screen/console/browser/whatever and you can then build off that and make it say other things.

## Most Basic Example

So lets look at a simple example in Javascript. ([Demo Here](https://code.sololearn.com/c55Mhx54oGmM))

```js
console.log("hello world");
```

If you go to the demo and click run you will see the resulting "hello world" being printed onto the screen. Go change it to say anything between the two quotation marks and it will output it.

> We have picked JS here as we dont need any application setup guff around it, we can literally just execute functions right away, which saves time in just getting something simple on the screen.

### WTF Is `console.log`?

If you asked this question well done, if not then no problem maybe you are already ahead here.

We have not covered the notion of **classes** or objects/instances yet, and won't really be going in depth on them just yet, but to summarise an object wraps multiple variables/functions giving you a group way to access similar functionality.

So `console` is an object that contains lots of functionality relating to putting stuff on the console or taking data from it. In this case we are using the `log` function which will output whatever *data* we give it onto the console.

Almost all programming languages have some basic console input/output library which handles outputting or retrieving data from a console, and for example the same logic in other languages would look like this:

#### C# Example
```c#
Console.WriteLine("hello world");
```

#### C++ Example
```c++
cout << "hello world";
```

#### Java Example
```java
System.out.println("hello world");
```

As you can see the mechanisms for accessing the console are slightly different, but ultimately all do the same thing.

> You may look at C++ and wonder what the hell is going on there, and C++ is quite an odd language in a lot of ways. Behind the scenes `cout` is an object with an overloaded operator (don't worry we will cover them later) that internally runs a function when the `<<` operator is used with it.

## Detour

So at this point we have done "Hello World" in JS, and while we have provided examples of how to write to the console in other languages, making an **application** in those languages requires a lot more than it does in JS, so we need to go on a little detour to discuss compiled vs interpreted languages before we revisit our hello world applications.