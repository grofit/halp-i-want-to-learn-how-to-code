# D A T A -  T Y P E S - A G A I N

I apologise for constantly retracing the same ground but digging a bit deeper, but hopefully later on you will thank me as you will be super grounded in what im waffling about.

So if we rewind we have so far spoken about `int`, `float`, `string` variable types. These are super common and you will be using these a lot, but there are also other data types which are more niche, so lets cover all common types.

> Not all languages will support all these types, but most do. For example C#, Java, C/C++ and many others all have the notion of these variable types.

## Boolean

This data type has 2 possible values, true or false. So if I were to ask you "Do you like peas?" you would ask your brain and it would tell you "yes" or "no", same sort of thing here (using C# for example).

```c#
bool doesPersonLikePeas = true;
```

## Byte

This is where we start getting into the deep stuff, a byte is a numeric value which can only store values between 0-255.

Day to day you wont really use a byte much by itself, as it tends to be used like a string where a collection of bytes make up a data stream of sorts.

> Bytes actually are very important from a technical perspective as you can actually look at almost all other types as many bytes glued together, and we will talk about that more later.

## Int

We have already discussed integers at a high level but there are actually a few different types of integers which are available depending on how big your values need to be.

### Int16 / Short

This is the 2nd smallest int as a byte is technically a type of integer. It is known as `int16` or `short` (they both mean same thing) and it can store a value between -32,768 to 32,767.

### Int32 / Int

This is the most common int, and if you were to just use `int` this is the type of integer you would be provided. It can store a value between -2,147,483,648 to 2,147,483,647.

### Int64 / Long

This is the biggest common integer and can store numbers between -2,147,483,648 to 2,147,483,647.

> You may be wondering why we have this many int types, and we are about to see there are lots of float types too, but we will address the **WHY** shortly

## Float

Like `int` we have already discussed `float` but there are a few different flavours.

### Float / Single

A float can also be known as a `single` and is the default `float` provided to you, it can store 6-9 digits accurately. So unlike an integer type which stores a value between a min and max a float is more geared for accuracy so you could have 6-9 (depending on language) digits and have the decimal place anywhere, be it 1.23456789 or 123456.789. If you try to store more digits it just truncates it.

### Double

This name makes more sense if you think of a `float` as a `single`, but this is the same sort of thing, just allows more accuracy giving 15-17 (again depending on language) precision.


== MORE TO COME ==












