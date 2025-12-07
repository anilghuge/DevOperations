# What is File System, what is the purpose of it?

File system is a technic or a way of storing and organizing the data on the physical storage devices of a computer like:

1. Harddisk
2. Pendrive
3. CD Rom

## How does the actual data get persisted on these storage devices?

The storage devices are electro magnetic or mechanical magnetic devices and they can only carry 0's and 1's. So, the data would be stored in binary format only.

Human data is not binary format - it will be in character/symbol representation. Then how can the symbols be stored in binary format on the physical devices?


### Human data is not binary format - it will be in character/symbol representation. Then how can the symbols be stored in binary format on the physical devices?

### The human characters/symbol representations has to be converted into decimal and a binary equivalent of the decimal should be stored on the physical devices. This technic is called **encoding**. For this there are standard charset encoding techniques available to ensure all the characters are encoded with the same numeric values so that the information can be carried across.

# What are the various charset encoding standards available?

1. ASCII
2. UNICODE
3. UTF-8
4. UTF-32
5. ISO-9001

### Why we need several charset encodings what is the difference between them?

Different charset encodings supports different languages, so we need multiple charset encodings.

### What is ASCII & how many languages it supports?

ASCII supports **english language only** characters with some special symbols. Total it supports **256 characters**. The largest number for representing a character is 255 and requires 8 bits. So to encode and decode the data all the characters from 0-255 are stored in 8 bit length on the storage device.

If every character is not stored with 8 bit size we cannot interpret the data while reading from the physical location since we don't know which character is of what length bits.

### Why can't we have one charset representing all the languages instead of many charset standards?

As we learned from earlier, if a charset supports a lot of languages it needs more bits for representing the character on the physical device. This eventually leads to wastage of memory when we are using only a specific language.

![](image1.png)
