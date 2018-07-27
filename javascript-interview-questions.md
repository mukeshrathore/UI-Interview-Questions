# JavaScript Interview Questions

### Refernce Links :
- [learn-javascript-in-one-week](https://coderbyte.com/course/learn-javascript-in-one-week)
- [3-common-javascript-closure-questions](https://www.coderbyte.com/algorithm/3-common-javascript-closure-questions)
- [3-questions-to-watch-out-for-in-a-javascript-interview](https://medium.freecodecamp.org/3-questions-to-watch-out-for-in-a-javascript-interview-725012834ccb)
- [10-common-javascript-interview-questions](https://www.coderbyte.com/algorithm/10-common-javascript-interview-questions)
- [basic-array-manipulation-with-functions-in-javascript](https://www.coderbyte.com/algorithm/basic-array-manipulation-with-functions-in-javascript)

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

### How to check whether given variable is integer or not?

### Sort an integer with using FOR loop but without using Sort Method?

### What are closures in javascript and their uses ?

### How to create Static variable in javascript?

### Is Javascript pass by value or pass by reference?

### Have you used AOP type of programming?

### what is the difference between slice and splice in javascript?

### Find the missing number from unsorted array without using sort method.

### [12,3,10,5,2].getEvenAndSortMethod()

###  difference between var and let keyword. specially in terms of closure.
>Ref link : [let-const-loop-heads](http://exploringjs.com/es6/ch_variables.html#sec_let-const-loop-heads)

### What is Prototype related to Object?

### What is Hoisting in javascript?
In Javascript, You can use variable and function statements before declaring them because Javascript automatically hoist/declare all the variables and function statements.
But Function expressions in Javascript are not hoisted and you can't use function expression before defining or declaring them.

============================

### How would you write a function that can be called only once? (not self envoking, you can call it, whenever you want, but only once) 

 

### Write a function (getEvenAndSort) that can be called on any array, and it returns the subarray of only the even numbers, but sorted.

[12,3,2,1,7,6].getEvenAndSort()

 

### "🤗".length   //what does it return?  => it returns 2, because the smileface is presented by unicode char => two char length.

### What do you get for this? "🤗".length - "🤗".length  

### Implement a react component (it can be simple, can have it's own state) that has a button, which toggles the visibility of a paragraph, which displays some text. "Hello" for example. By default the greeting is hidden and clicking on the button, it gets visible. When clicking on it again, gets hidden.

 

### How do you preserve the cart data for a user in order to show the updated data when she opens a new tab?

 

### There was an image, width='500' height='300', which I had to implement with css.

Markup:
```html
<section>

   <article class='one'>One</article>

   <article class='two>Two</article>

   <article class='three'>Three</article>

   <article class='four'>Four</article>

</section>
```


### How to Flatten an array in JS

### Given an API call and Callback. The requirement is to make a table or a list using these. You can use any framework.

 

### How would you write a function that can be called only once? 


### Design a simple tic tac toe game

### Some questions about React, like where to fetch data in React component

### Some Javascript questions, for example, how to use setTimeout(), how to use Closure, what happened when using new to create an instance

### Some CSS questions

### print ping pong alternatively in JavaScript

### set interval();

 

### Given an array string and numbers

 

### Chess board proto creation: should not edit any of the HTML tags and should not add any classes. Only make use of generic DIV and need to add the CSS to it.

 

### Multi sum functions: Common function accepting closures as well as generic return. Asynch function execution type.

### Need to sort the anagrams from the array: Custom sorting logic needs to be written to support anagrams to appear one after the other.

### React counter application: clicking on "+" should increment the counter and click on "-" should decrease the counter.

### Prototype Programming: add the prototype method to filter out even numbers and sort the same. Should not mutate the input array.

  




