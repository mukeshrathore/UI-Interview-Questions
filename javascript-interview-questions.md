# JavaScript Interview Questions

### Refernce Links :
- [learn-javascript-in-one-week](https://coderbyte.com/course/learn-javascript-in-one-week)
- [3-common-javascript-closure-questions](https://www.coderbyte.com/algorithm/3-common-javascript-closure-questions)
- [3-questions-to-watch-out-for-in-a-javascript-interview](https://medium.freecodecamp.org/3-questions-to-watch-out-for-in-a-javascript-interview-725012834ccb)
- [10-common-javascript-interview-questions](https://www.coderbyte.com/algorithm/10-common-javascript-interview-questions)
- [basic-array-manipulation-with-functions-in-javascript](https://www.coderbyte.com/algorithm/basic-array-manipulation-with-functions-in-javascript)

---
### Write a program that prints the numbers from 1 to 100. But for multiples of three print "Fizz" instead of the number and for the multiples of five print "Buzz". For numbers which are multiples of both three and five print "FizzBuzz"

```js

for(i=1;i<=100;i++){

if(i%3===0 && i%5==0){
    console.log("FizzBuzz")
}
else if(i%5===0){
    console.log("Buzz")
}
else if(i%3===0){
    console.log("Fizz")
}
else {
    console.log(i)
}

}

```

---
### What would be the Output of below Code?

```js

let funcList = [];

for (var i = 0; i < 5; i++) {
    funcList[i] = function(){
        console.log(i);
    };
}

// i === ?
for (var j = 0; j < 5; j++) {
    funcList[j]();
}

```
> it will return 5times 5 in the console.

---
### What would be the Output of below Code?

```js

let funcList = [];

for (let i = 0; i < 5; i++) {
    funcList[i] = function(){
        console.log(i);
    };
}

// i === ?
for (let j = 0; j < 5; j++) {
    funcList[j]();
}

```
> it will return 0 1 2 3 4 in the console. Please note `funcList[j]()` will initiate a single instance and the function 5 times.

---
### How to check whether given variable is integer or not?
use isInteger() to check whether given variable is integer or not.

Using built-in method of Number
```javascript
Number.isInteger(5.2) // false
Number.isInteger(4) //true
```

Different ways of Using custom function to check same condition
```javascript
function checkInteger(x){
    if(Math.floor(x)===x){console.log('Yes. Number is Integer.')}else{console.log('Number is not integer')} // Using if-else. Similarly Math.ceil method could also be used.
}

function checkInteger(x){
    Math.floor(x)===x?console.log('Yes. Number is Integer.'):console.log('Number is not integer') // Using ternary operators
}

// Try using Prototype

```
---
### Sort an Array with using FOR loop but without using Sort Method?

```javascript

function bubbleSort(array) {
  var done = false;
  while (!done) {
    done = true;
    for (var i = 1; i < array.length; i += 1) {
      if (array[i - 1] > array[i]) {
        done = false;
        var tmp = array[i - 1];
        array[i - 1] = array[i];
        array[i] = tmp;
      }
    }
  }

  return array;
}

var number = [1,43,23,6,10,5,9,100,09,2];
bubbleSort(number); 
console.log(numbers); //[1, 2, 5, 6, 9, 9, 10, 23, 43, 100]

```

---
### What are closures in javascript and their uses ?
https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-closure-b2f0d2152b36 

---
### How to create Static variable in javascript?

Static variables are variables, typically used in functions, that maintain their value between function calls. Javascript does not support static variables per se; their is no static keyword in the language. However in javascript all functions are also objects and we can use this fact to simulate static variables. All we have to do is create a variable that is a member of the function, and since it's now part of an object, the value will be retained between calls. While there aren't truly static in the strictest sense of the word, they maintain their value between functions calls, and that usually serves the purpose. 

As an example, consider a completely lame, but very instructive, function that keeps track of the number of times that it has been called. Here's how it might look: 

```javascript

function countMyself() {
    // Check to see if the counter has been initialized
    if ( typeof countMyself.counter == 'undefined' ) {
        // It has not... perform the initilization
        countMyself.counter = 0;
    }

    // Do something stupid to indicate the value
    alert(++countMyself.counter);
}

```

Each time that the countMyself function gets called from the page, the value is shown increasing by one (which means that the value is retained between calls). Using this trick, you can easily simulate static variables in Javascript.

> Ref: [stackoverflow](https://stackoverflow.com/questions/1535631/static-variables-in-javascript)

---
### What are namespace in javascript

---
### Is Javascript pass by value or pass by reference?
Please note variables are pass by value and Objects(arrays,functions parameters) are pass by reference 


---
### what is the difference between slice and splice in javascript?

---
### Find the missing number from unsorted array without using sort method.


---
###  difference between var and let keyword. specially in terms of closure.
>Ref link : [let-const-loop-heads](http://exploringjs.com/es6/ch_variables.html#sec_let-const-loop-heads)

---
### What is Prototype related to Object?

---
### What is Hoisting in javascript?
In Javascript, You can use variable and function statements before declaring them because Javascript automatically hoist/declare all the variables and function statements.
But Function expressions in Javascript are not hoisted and you can't use function expression before defining or declaring them.

============================

---
### How would you write a function that can be called only once? (not self envoking, you can call it, whenever you want, but only once) 

 

---
### Write a function (getEvenAndSort) that can be called on any array, and it returns the subarray of only the even numbers, but sorted. [12,3,2,1,7,6].getEvenAndSort() , [12,3,10,5,2].getEvenAndSortMethod()


 

---
### "🤗".length   //what does it return? 
it returns 2, because the smileface is presented by unicode char => two char length.

---
### What do you get for this? "🤗".length - "🤗".length  
0


 

---
### How do you preserve the cart data for a user in order to show the updated data when she opens a new tab?
Multiple ways : 
1. Save the cart data in local Storage - retrieve it on new tab (browser based solution)
2. Use getters and setters in Service (Using Angular,React, javascript)
3. Pass the details in url. But not effecient way of doing the things.

---
### How to Flatten an array in JS

---
### Given an API call and Callback. The requirement is to make a table or a list using these. You can use any framework.

 

---
### How would you write a function that can be called only once? 


---
### Design a simple tic tac toe game


---
### how to use setTimeout()? 

---
### how to use Closure? 

---
### what happened when using new keyword to create an instance?


---
### print ping pong alternatively in JavaScript

---
### usecase of setInterval();

---
### Multi sum functions: Common function accepting closures as well as generic return. Asynch function execution type.

---
### Need to sort the anagrams from the array: Custom sorting logic needs to be written to support anagrams to appear one after the other.

---
### Prototype Programming: add the prototype method to filter out even numbers and sort the same. Should not mutate the input array.

---
### What are the ways to create an Object?
  
---
### Difference between undefined and undeclared

---
### How do you compare two Objects
Two Object can't be compared with == or ===. You need to check their property one-by-one.

---
### use-case of IIFE

---
### Difference between for in and for of loop?
`for... in` loop: it iterate over key
`for... of` loop: it iterate over value

```javascript
var arr = [3, 5, 7];
for (var i in arr) {
   console.log(i); // logs "0", "1", "2"
}

for (var i of arr) {
   console.log(i); // logs "3", "5", "7"
}

```

above eg. is for Arrays. What about Objects?

---
### Difference between let and var with respect to Closure context


---
### which JavaScript library that matches paths against registered routes ?
route-recognizer.js

---
### Design Patterns in JS ?


--- 
### Filter, map, reduce on Array and Array of Objects

---
### Assign, create, bind on JS Objects

### What is the output of console? How can we make z value print 10 instead of 100 without touching function declaration.
```javascript
var z = 100,
    x = { z : 10 },
function printNum(){
    console.log(this.z);
}
printNum();

Answer: printNum.call(x)
```

---
### Write a function specialCase on "Hello".specialCase() to output H_e_l_l_o

---
### difference between function declaration `function x(){}` and function expression(arrow function) `()=>{}`?

---
### How to know that whether the Object `{x:1, y:2, z:8, b:null, a:[10]}` contains array in it? ...Hint : hasOwnProperty


---
### How do you know at any point in the application that how much size your application has?

---
### Where are timers and variables stored in Javascript?

---
### Compare Javascript Module Systems - commonJS vs AMD vs ES2015

---
## Memory Management in Javascript


### What is garbage?
All variables which can not be reached from root node are considered as Garbage.

### Garbage Collection process?
Garbage collection process takes place in 2 phases:
Phase 1: Find all Garbages
Phase 2: Return memory used by garbage variable to system

---
### Difference between stack and heap memory?
Variables in JavaScript (and most other programming languages) are stored in two places: stack and heap. 
>Ref: [glebbahmutov.com](https://glebbahmutov.com/blog/javascript-stack-size/)

Stack is used for static memory allocation and Heap for dynamic memory allocation, both stored in the computer's RAM. Variables allocated on the stack are stored directly to the memory and access to this memory is very fast, and it's allocation is dealt with when the program is compiled.
>Ref: [net-informations](http://net-informations.com/faq/net/stack-heap.htm)

> Ref: [Memory_Management_in_JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Memory_Management)

---
### what is memory heap and How to determine memory leakage?
Memory leakage can be detected by comparing 3 memory snapshot.

>Ref : [4-types-of-leaks-in-js](https://auth0.com/blog/four-types-of-leaks-in-your-javascript-code-and-how-to-get-rid-of-them/)

There are 2 memory pools : Young Memory pool and Old Memory Pool
- Whenever a new keyword is used to create Object or Array, the memory is allocated from 'Young' memory pool and whenever the young memory pool is totally consumed garbage collector is forced to run and free up Memory.



---
### What challenges you faced while implementing current project?
Implementing Single sign-on feature on Angular UI. As a solution, we used APP_INITIALIZER for angular to complete this task. 

> Ref : [hook-into-angular-initialization-process](https://dormoshe.io/articles/hook-into-angular-initialization-process-8)

---
### What is the difference between Set and Array?
>Ref : [ES6-Set-vs-Array](https://medium.com/front-end-hacking/es6-set-vs-array-what-and-when-efc055655e1a)

---
### Name some common data Structures in Javascript? Do you know some common data structures and algorithms?
>Ref : [Data Structures and Algorithms in JavaScript](https://www.youtube.com/watch?v=t2CEgPsws3U&t=29s) 





