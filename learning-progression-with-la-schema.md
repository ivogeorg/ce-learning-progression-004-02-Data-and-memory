# CPE 1040 - Fall 2020

This is learning progression 004 for the Fall 2020 installment of the course CPE 1040: Introduction to Computer Engineering at MSU Denver.

Table of Contents
=================

* [CPE 1040 \- Fall 2020](#cpe-1040---fall-2020)
  * [Learning Progression 004: External LEDs](#learning-progression-004-external-leds)
    * [Step 2: Data &amp; memory](#step-2-data--memory)
      * [1\. Study](#1-study-1)
        * [Arrays and memory](#arrays-and-memory)
        * [Memory layout](#memory-layout)
        * [Addressing](#addressing)
        * [Random access](#random-access)
      * [2\. Apply](#2-apply-1)
      * [3\. Present](#3-present-1)

## Learning Progression 004: External LEDs

This progression introduces fundamentals of computing, including the binary system of data representation as well as the basics of memory and processing. We introduce assembly language in the context of a minimal instruction set processor. This is where the lowest layer of the software stack and the highest layer of the hardware stack coexist, and where user programs are translated into machine code and executed by the processor one instruction at a time. This is also the level of computing which directly correpsonds to the simplest theoretical models of a computer. We also introduce the input-output capabilities of the micro:bit and build an external circuit to serve as an extension to the built-in 5x5 LED matrix to run our Screensavers program on.

### Step 2: Data & memory  
[[toc](#table-of-contents)]

#### 1. Study
[[toc](#table-of-contents)]

##### Arrays and memory
[[toc](#table-of-contents)]

Arrays have indices. They are the closest analog of computer memory. Memory is organized as a large array with addresses. Each byte (8-bits) has an address, starting from 0x0 up to the highest address depending on the size of the memory.

**TODO: A convincing fundamental motivating definition of memory.**  
```
     -----------------
0x00 | | | | | | | | |
     -----------------
0x01 | | | | | | | | |
     -----------------
0x02 | | | | | | | | |
     -----------------
0x03 | | | | | | | | |
     -----------------
```
##### Memory layout  
[[toc](#table-of-contents)]

Primitive types: integers, floats, booleans.  
Composite types: strings, objects.  
Arrays of any type.  

Functions.  

##### Addressing  
[[toc](#table-of-contents)]

Addresses, references, and pointers.  

##### Random access
[[toc](#table-of-contents)]

Array formula: _base address + index * base type size_. Arrays and memory revisited. Constant access time regardless of address. RAM.  

Array address calculation example with sketch.  

#### 2. Apply
[[toc](#table-of-contents)]

1. `[<lernact-prac>]`The `[<cept>]`_hexadeximal_ number system is frequently used in computing (e.g. the micro:bit HEX files, and to show memory addresses that are too big to show in binary). "Hexadeci-" means 16. Questions and tasks:  
   1. What is the base of hexadecimal?  
   2. What are the symbols of hexadecimal? List them.  
   3. How many bits can represent the same number of different numbers as one `[<cept>]`_hexadigit_?  
   4. Using your answer to the previous question, describe a simple procedure to convert numbers from binary to hexadecimal, and vice versa.  

2. `[<lernact-prac>]`Write a function `bin2Hex(bin : string) : string` which takes a binary integer string and returns the corresponding hexadecimal integer string (e.g. for input `0b00001111`, the output is `0x0F`). Guidelines and hints:
   1. Assume the argument `bin` will have the prefix for binary.  
   2. You might need to `[<cept>]`_pad_ the argument string. What is padding? If I need a string to be of some particular length (or width for binary number strings), say 8 bits, and I have an input like `0b111`, I can pad this string on the left with `0`-s to get the equivalent 8-bit number strging `0b00000111`.  
   3. The output string should have the prefix for hexadecimal.  

3. `[<lernact-prac>]`Write a function `hex2Bin(hex : string) : string` which takes a hexadecimal integer string and returns the corresponding binary integer string (e.g. for input `0x0F`, the output is `0b00001111`). Use prefixes.  

4. `[<lernact-prac>]`**[Optional challenge, max 5 extra step points]**  **TODO** Creating an index to a database:
   1. 2D array.  
   2. Array sorted by first column.  
   3. Create an index array for the second column.  
      <img src="images/index-array-into-record-array-hex.png" alt="Index into Record table" width="600" />  

5. `[<lernact-prac>]`**[Optional super challenge, max 16 extra step points]** **TODO** Array-based malloc simulation ([program draft](https://github.com/ivogeorg/ce-learning-progressions-selected-programs/blob/master/malloc-simulation.js):
   1. Byte-array simulation.
   2. Object memory footprint.  
   3. Memory alignment.  
   4. Calculation of array element addresses.  
      <img src="images/malloc-sim-1.png" alt="Memory management with malloc and free (1 of 2)" width="600" />  
      <img src="images/malloc-sim-2.png" alt="Memory management with malloc and free (2 of 2)" width="600" />  

#### 3. Present
[[toc](#table-of-contents)]

In the [programs](programs) directory:
1. Add your program from 2.2.2 with filename `microbit-program-2-2-2.js`.  
2. Add your program from 2.2.3 with filename `microbit-program-2-2-3.js`.  
3. Add your program from 2.2.4 with filename `microbit-program-2-2-4.js`.  
4. Add your program from 2.2.5 with filename `microbit-program-2-2-5.js`.  

In the [Lab Notebook](README.md):

1. Answer the questions and show your work for 2.2.1 in well-formatted Markdown, including whatever images, tables, or other graphical elements you find necessary. 
2. Link to the program from 2.2.2.  
3. Link to a demo video showing the execution of the program from 2.2.2.  
2. Link to the program from 2.2.3.  
3. Link to a demo video showing the execution of the program from 2.2.3.  
2. Link to the program from 2.2.4.  
3. Link to a demo video showing the execution of the program from 2.2.4.  
2. Link to the program from 2.2.5.  
3. Link to a demo video showing the execution of the program from 2.2.5.  
