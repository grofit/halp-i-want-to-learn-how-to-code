# Memory

So we briefly touched on the notion of memory earlier and how the computer needs to store all this guff we give it. 

Much like your brain it takes more effort to store bigger things than smaller things, so if I ask you to remember the number `1` you could easily do that, and if I asked you to remember the number `756320165` you could probably do it, but it would require far more effort.

The same can be said for computers.

## Bits and Bytes

So we have seen a `byte` allows 256 possible values (0-255 with 0 being a value), and under the hood a byte is defined as **8 bits**. Now you may be wondering what a bit is, and why we have 8 of them.

### A bit
A bit is a binary value, which stores a **0** or a **1**, and this is where we take the deep dive into whats actually happening inside the computer when we deal with data types.

So if we have 1 bit, we can store 2 possible values, however if we were to use 2 bits together we can now express 4 possible values **00**, **01**, **10**, **11**.

You may be seeing where im going here, and the numerical sequence may seem familiar to you, as we increase the amount of bits available we also double the available values:

- 1 bit = 2 values
- 2 bits = 4 values
- 3 bits = 8 values
- 4 bits = 16 values
- 5 bits = 32 values
- 6 bits = 64 values
- 7 bits = 128 values
- 8 bits = 256 values

So if we take a step back here, and look back at our **integer** values, we had **int16**, **int32**, **int64**. Those 16,32,64 values indicate how many bits are used to represent that number. So a 16 bit number can store a possible 65,536 values, and a 32 bit one can store far more etc.

Same with a `char`, that is basically (depending on language) a 16 bit value, which gives 65,536 possible letters to use so this again is made up of bits under the hood, and therefore a `string` is just a load of 16 bit values in a sequence.

So the big reveal here is that [ALL your data types are just bits in memory](https://user-images.githubusercontent.com/927201/92087349-49c0d000-edc3-11ea-87f3-656bcdd63580.png). 

> This is how computer memory works, and the contract almost all computer hardware agree upon for processing data. It is all just represented as binary, loads of ones and zeros...

### Bytes

So while under the hood all this stuff its just binary made up of bits it would get quite faffy if we had to always interact with things at the bit level, so we often dont think in terms of bits but in terms of bytes.

So 8 bits makes a byte, and if I ask you how big your computers hard disk is you may tell me its 500 giga**BYTES** or 2 tera**BYTES**, and this is no coincidence.

If we look in terms of bytes, its easier to think about how much memory we are gobbling up, so lets just do a [quick rundown](https://www.reddit.com/r/The_Bogdanoff/comments/5p1dx2/so_heres_the_run_down/) on byte naming conventions.

- 1 kilobyte = 1024 bytes
- 1 megabyte = 1024 kilobytes
- 1 gigabyte = 1024 megabytes
- 1 terabyte = 1024 gigabytes

No point going any higher for now, but as you can see we now have some tangible details on how much memory we are using for our variables now.

### Bytes and Variables

Rewinding back to integer types we have `byte`, `int16` (aka `short`), `int32` (aka `int`), `int64` (aka `long`) so in terms of bytes this is 1 byte, 2 bytes, 4 bytes, 8 bytes.

> Worth noting here that certain older programming languages may use different sizings for some of these types, but these days the above values are pretty standard and also the sizes can potentially change based on if you have a 32 bit or 64 bit application, but lets not worry about that for now.

The same can be said for varying floating point types, as `float` is 4 bytes and a `double` is 8 bytes.

So if we wanted to store someones age, its unlikely that someone is going to live over 255 years of age, so rather than use up 4 bytes and store it as an `int` we could store it as a `byte` and save 3 bytes of memory.

> In the real world its quite common to just use `int` for most use cases, as its easier to do math between variables if they are all the same type, so when you are getting started dont worry about trying to use the most optimal data type for your data, just be in the right ballpark. You can always optimize later on and change your data types to be more specific if needed.