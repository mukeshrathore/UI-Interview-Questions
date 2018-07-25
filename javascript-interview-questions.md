# JavaScript Interview Questions

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


