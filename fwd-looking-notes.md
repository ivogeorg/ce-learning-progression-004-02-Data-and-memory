# Forward-looking notes

**[For staff use]**

Originally in Step 004-02

#### 2. Apply
1. `[<lernact-prac>]`**[Optional challenge, max ? extra step points]** Caching task (e.g. function-result cache to avoid pre-computing; amortized computation with backing store, say array). Resources:    
   1. [Memoization in JS](https://scotch.io/tutorials/understanding-memoization-in-javascript) from [Web dev tutorials](https://scotch.io/).  
      1. Objects:
         1. [Working with objects (MDN)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects).  
         2. [TypeScript Object Types](https://www.typescriptlang.org/docs/handbook/2/objects.html).  
         3. [MakeCode Langauges](https://makecode.com/language).  
   2. [Closures in TS](https://basarat.gitbook.io/typescript/recap/closure) (from [TypeScript Deep Dive](https://basarat.gitbook.io/typescript/)).    
   3. Fibonacci numbers:  
      1. ViHart videos:  
         1. [Video 1](https://www.youtube.com/watch?v=ahXIMUkSXX0) 
         2. [Video 2](https://www.youtube.com/watch?v=lOIP_Z_-0Hs)  
         3. [Video 3](https://www.youtube.com/watch?v=14-NdQwKz9w&t=305s)  
      2. [Wikipedia](https://en.wikipedia.org/wiki/Fibonacci_number).  
   4. How to use this to efficiently arrive at a large result without maxing out the memory of the micro:bit?     
   5. Example with closures for computing binary numbers?  
7. `[<lernact-prac>]`**[Optional challenge, max 5 extra step points]** **TODO** Fibonacci with memoisation/caching using a [`Buffer`](https://makecode.microbit.org/types/buffer).  
   1. [`Int32LE`](https://makecode.microbit.org/types/buffer/number-format):  
      - `-1` for none  
      - buffer of depth 47 for offsets in range [0, [46](http://www.maths.surrey.ac.uk/hosted-sites/R.Knott/Fibonacci/fibtable.html)], to stay in range  
   2. **TODO:** How does `Buffer` work?
      - How big is it?  
      - Are gaps handled gracefully?  
      - Is there automatic expansion?  
      - Can positions be `undefined`?  

## Resources

1. [Rapid tables](https://www.rapidtables.com/).  
