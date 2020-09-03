# Variables

So lets not beat around the bush, lets take a look at possibly the simplest part of programming, which is data types and variables. 

Here is an example of a variable in Javascript.

```js
var someNumber = 1;
```

## What is a variable?

So before we disect the above code, lets just make sure we are all on the same page as to what a variable is.

Let's say I ask you what your name is. You would be able to recall that information from your brainicles and tell me what it is right?

That is all a **variable** is, its a bit of data that you want to store in the computers memory and retrieve at a later point in time. So just as your brain can store information for short/long periods of time so can a computer, although in the computer world this is known as the **scope** of a variable.

> We will dive more into scopes later, as we need to lay some more groundwork first, but all these fancy buzz words will be explained later on so dont worry if you have no idea what im talking about

## Data Types

Another important point to cover is the notion of data types, which is super simple, but the **types** available in each programming language can differ, but at the end of the day they all allow you to express the same intent.

So lets go back to the scenario where we use your `name` as a variable, and lets also think of your `age` as a variable and express this in Javascript.

> Dont worry about the syntax below, we have not covered that yet, but we will do shortly, so keep reading don't be scared by `var` or `;` etc

```js
var name = "John Doe";
var age = 22;
```

So what is the difference between these 2 variables other than they would have different names?

I am hoping you would have said *"One is a number, one contains text"* or something similar (feel free to pretend you did think of this even if you didnt, well done etc). 

If we look at these 2 data types we can start to get a better handle on what data types are and how they effect you (and variables).

### Numeric Data

Numeric data is one of the most common sorts of data types, but it kind of gets a bit more complex than all numbers being the same in terms of data type.

So if we look at the number `120` and `1.20` they are both valid numbers, but they are often treated differently (depending on the language).

The former number `120` is known as an **Integer** and these types of numbers express numbers without decimal points, the latter number is known as a **Float** (floating point) and is used to store numbers which contain decimal places (although they dont HAVE to).

Luckily computers are clever enough for you to do silly things like store `1.20` as an integer, but like an executioner it just cuts off the decimal place and rounds the number up or down, if you are moving from an **integer** to a **float** then it doesnt care.

> Certain languages have more numeric data types, some have less but im not going to bore you with the details on that just yet, we will get into it later

### Textual Data

The other kind of data we were looking at was `name` which contained text, and in the computer world this is known as a **String**. 

Although we look at a **String** as a block of text, its actually just a collection of **Characters** (fancy name for letters), so the `name` John Doe is actually 8 characters `J`, `O`, `H`, `N`, ` `, `D`, `O`, `E`.

> This is why they are called strings, because they are a string of characters.

You don't really need to care too much about characters specifically at the moment. I just want to make clear that at a high level there are **numbers** and **strings** before we continue.

### Variable Syntax

Great job if you got this far! You had to wade through a lot of waffle, and boring stuff, but huzzah lets look at variables a bit more closely, by going back to the first example:

```js
var someNumber = 1;
```

So what the heck is ACTUALLY going on here? Lets break the Javascript **syntax** down so we know whats going on here.

> We tend to read code from left to right in most languages, so each bit of code is generally contextually dependent on the previous bit of code, so if we took one bit of the above code away it would all fall apart as some context would be missing.

#### `var`

This tells JS (cba typing Javascript everywhere) that we are creating a variable, so behind the scenes it needs to go allocate some memory on the computer. Much like if I asked you remember the number 5142 your brain would do something magical and store the info away for you.

#### `someNumber`

This is the name of the variable we want to store. This is super important as without the name of the variable we cannot access it, like if I ask you for your age you know what im talking about and where to think to retrieve that data. Same thing here, its a handle for the computer to know where to rummage around to get the data back for you.

> It is worth noting here that in majority of languages your variable names MUST START WITH LETTERS, they can contain numbers but you will get errors if you start a variable name with a number or symbol. It is recommended to always use text wherever you can, certain language have conventions for naming variables but more on that later.

#### `=`

This is the equals sign, im sure you have used this before in basic maths etc. This is telling JS that we want to set the value for the variable we have created.

#### `1`

This is the value we are assigning to the variable we created.


#### `;`

This little gem is one of my favourite things, its a **Semi-colon** and it represents grace and beauty... as well as indicating that you have finished the current line of code, so it can be evaluated. 

> Some programming languages don't like semi colins (such as **Python**) and that makes me very sad, and can keep me awake at night...

### Congrats!

If this was a game you would earn an achievement here, something cleverly named (I can't think of anything though).


