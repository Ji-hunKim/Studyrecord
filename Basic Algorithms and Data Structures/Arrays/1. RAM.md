# RAM

## 1. What is a Data Structure?
As the name implies, it's a way of structuring data.   
Ram is basically where all of our variables are gonna be stored.

Let's say we store an array in ram.   
Ram is measured in bytes, and it's common for many computers to have 8GB of Ram 

>1 Giga = 10^9Bytes

>1 Byte = 8bits

>1 Bit = position that can store a digit (only 0,1) -> by the restriction on the digit

So individual bits can form multiple bits which can form bytes which can form RAM and RAM can be used to store advanced data structures.

Integer is commonly represented by 4 bytes.   
So we would actually have 32 bits.


It's gonna be 31 zeros and one 1 if we represent 1 in terms of bytes. 

While Ram can be thought of as a contiguous block of data, it also has two components to it.   

Obviously we're storing values in our RAM but every value is gonna be stored at a distinct location which we call an address.

As we store an array and RAM, we don't always get to choose what location it's gonna be at, but one thing is about arrays is that they're always gonna be contiguous.

Then why are we incrementing the address by four every time? -> Each value takes 4bytes to store.

>ASCII character -> 1byte