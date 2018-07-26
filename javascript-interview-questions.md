# JavaScript Interview Questions

### Refernce Links :
- [learn-javascript-in-one-week](https://coderbyte.com/course/learn-javascript-in-one-week)
- [3-common-javascript-closure-questions](https://www.coderbyte.com/algorithm/3-common-javascript-closure-questions)
- [3-questions-to-watch-out-for-in-a-javascript-interview](https://medium.freecodecamp.org/3-questions-to-watch-out-for-in-a-javascript-interview-725012834ccb)
- [10-common-javascript-interview-questions](https://www.coderbyte.com/algorithm/10-common-javascript-interview-questions)


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




