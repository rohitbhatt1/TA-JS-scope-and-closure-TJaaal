1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// answer

let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};

let percentage = (marks, total)  => {
  return (marks * 100) / total;
};



2. Write Function Declaration or Function Expression next to the function.


function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer

// Function Declaration
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
}


// Function Expression

let percentage = function (marks, total) {
  return (marks * 100) / total;
}

// function arrow

let percentage = (marks, total) => {
  return (marks * 100) / total;
}

// Function Expression.


let percentage = (marks, total) => (marks * 100) / total;

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

 //ans.  A function expression is very similar to and has almost the same syntax as a function declaration.The main difference between a function expression and a function declaration is the function name, which can be omitted in function expressions to create anonymous functions.

Example: (Function Expression) let percentage = function (marks, total) { return (marks * 100) / total; };


4. Why is a function call an expression in JavaScript?
// ans.When we call any function, it will return any value or undefined which is also a value, so it is called an expression.


5. Write VALID and INVALID next to each example below with the reason.

function add(a, b) {
  return a + b;
}

let five = add(2, 3); //  it is a valid piece of code.
five = add; // it is also valid piece of code. beacuse it is function refrence.
five = five(10, 11); // it is a valid piece of code.and this is function declearation.
five = function () {
  return 'Hello';
}; // Valid it is a function expression.


6. What is the difference between function definition and function call? Explain with an example.4

ans. the difference between function call and function defination is. =>"function definition" we define that how function will perform an in "function call" we call it to perform certain action.


// function defination.
function multiply(a,b){
    return a * b ;
};
// function call.
multiply(20,5).


7. What is the similarities between function definition and function call?
ans. function defination is a define a function and function call is the code used to pass control to a function.


8. Is the code below valid or invalid. Explain with reason.
ans.
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid.  Because function is an object, it can have any key.

9. What is higher order function explain with an example.
ans.
let number = [1, 2, 3, 4, 5, 6,8,9,10,11,12,1,3,14];
let isEven = (num) => {
  return num % 2 === 0;
}
let isOdd = (num) => {
  return num % 2 !== 0;
}
function filter (arr, cb) {
  let array = [];
  for (let i of arr) {
    if (cb(i)) {
      array.push(i);
    }
  }
  return array;
}
console.log(filter(number, isOdd));
console.log(filter(number, isEven));


10. Explain what is callback function. Why you can pass a function inside a function?
ans.
A function that is passed a parameter to a higher order function is known as a callback function. As function is an object in JavaScript and object is an expression, thus, a function can be passed inside a function.
