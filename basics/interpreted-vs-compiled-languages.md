# Interpreted vs Compiled Languages

I wont lie to you, this is a bit of an advanced thing to cover so early on, but given we are learning programming agnostic of languages its worth pointing out why certain languages may seem *easier* to use than others.

> We wont be going SUPER DEEP DIVE into this subject so while it's a more advanced topic, really we just need to cover some basics that will solidify future chapters easier for you.

## Compiled Languages

It's easier to start with compiled languages, and they are basically a language which has to run through a compiler to be run on a computer. This means it takes EVERYTHING you have written in code and converts it into a singular output for execution.

So a typical flow for a compiled language would be:

1. Write the code
2. Compile the code (known as **building/compiling**)
3. Run resulting application (on windows an **exe**)

The reason for this is that the language you have written your code in is not the same as what the computer will be executing the code in. In most cases your code will be converted to machine code or some intermediate language/code for execution.

> This goes down a big rabbit hole, and we don't really want to bog you down too much here, but machine code is like super low level instructions a computer understands and can execute, whereas intermediate languages are often higher level and are run through other layers to generate machine code.

Examples of code that runs through a compiler would be C#, Java, C/C++, Rust and many others, but simply speaking all we need to know here is that a compile language takes ALL your code and kinda runs it all together as a single output.

### What About Errors?

If there are any errors in your code, the entire thing wont compile and it poops out with an error, so in this case you can only run your code when there are no errors.

## Interpreted Languages

Simply speaking interpreted languages (also known as scripting languages) are not run as a whole thing but are instead processed line by line.

So in the example of Javascript where we just have a `.js` file and put a line of code there and run it through the browser or node.js it just processes each line and works out what to do. 

Some examples of interpreted languages are Javascript, Python and Ruby. There are loads of others too but for the moment let's just focus on mainstream languages.

### What About Errors?

In this case its quite interesting, as it processes line by line, it will keep running code until it finds an error then poop out on you.

This is a bit of a problem in some scenarios as lets say you were wanting to create a user for a website and you made the user and stored them in the database but then needed to send an email, and there was an error in your code... You have made a user but no email would ever get sent, so they would keep trying again filling up your database.

## This Sounds Great, Why Does It Matter?

The reason we are learning about this now is because in the *Hello World* JS example, we were using an interpreted language, so it made it look super simple to do hello world.

However if we were to show you how to do *Hello World* in C++ or C# we would need to do things differently, because they are not interpreted languages and have no idea where your **entry point** is in the code.

## What's An Entrypoint?

GREAT QUESTION! So an entry point is basically a function hook in your source code that tells a **compiled language** where to start running, and in most cases this is known as **the main function**.

> With interpreted languages you provide a file and it will run (in most cases) top to bottom evaluating as it goes, so you don't need an explicit entry point, but in compiled languages you need the entry point to indicate where to begin.

This is why we have gone down this rabbit hole so that when we revisit *Hello World* with compiled languages you will not be freaked out by code like:

```c#
static void Main(string[] args) { ... }
```

So let's get more into that in the next section and cover entry points and *Hello World* in other languages.

> Although this chapter makes out like its one or the other for languages, some are both. For example Python can be compiled or interpreted and so can others, so it's useful to know that there is a difference but in some cases you can choose how to run your code.