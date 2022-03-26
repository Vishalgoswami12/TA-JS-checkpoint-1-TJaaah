<!-- 1. Using loops take 10 inputs from user and find the average of all the numbers. -->

let total= 0;
for (let i=1;i<=10;i++){
let input = prompt("Enter a number")
total += Number(input);
}

let average = total / 10;
console.log (average, 'avrg');

<!-- 2. What will be the output of the code below -->

<!-- ```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}fun -->

````print is not defined
<!--
3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10. -->

function getEvenSum (max=10){
  let sum =0;
for (let i=0;i<=max;i++){
  if(i%2 === 0){
    sum=sum+i
  }
}
return sum;
}

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
<!-- function getOddSum (max=10){
  let sum =0;
for (let i=0;i<=max;i++){
  if(i%2 !== 0){
    sum=sum+i
  }
}
return sum;
} -->

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

function getProductOfDigits (num){
  var str = String(num);
  var product = 1;

  for(let i=0; i<str.length; i++) {
    product *= Number(str[i]);
  }
return product;

}

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // output//'Bigger than 5
check(1); // output// 'Smaller than 5'
check(5); // output// 5
````

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") return "You are arya";
  if (name === "John") return "You are john";
  return "Who are you";
}

getOutput("Arya"); // what will be the output
getOutput("John"); // what will be the output
getOutput(); // what will be the output
```

"You are arya"
"You are john"
"Who are you"

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") console.log("You are arya");
  if (name === "John") console.log("You are john");
  return "Who are you";
}

getOutput("Arya"); // what will be the output
getOutput("John"); // what will be the output
getOutput(); // what will be the output
```

It will print "You are arya" but it return "Who are you"
It will print "You are john" but it return "Who are you"
"Who are you"

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
   function userName(name){
   return `Hello ${name} is a good boy`;
   }
10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

The difference between for loop and while loop is that in for loop the number of iterations to be done is already known and is used to obtain a certain result whereas in while loop the command runs until a certain condition is reached and the statement is proved to be false.
for loop ex- function getOddSum (max=10){
let sum =0;
for (let i=0;i<=max;i++){
if(i%2 !== 0){
sum=sum+i
}
}
return sum;
}

while loop ex- let sum =0;
let i=0;
while (i<=max>){
if (i%2===0){
sum=sum+i;
}
i++
}
