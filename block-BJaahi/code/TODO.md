
// Declaration
var username; //undefined
let brothers; //empty not defined
function sayHello(name) {
  return `Hello ${name}`;
}
let message; // empty i.e not defined
var nextMessage; //undefined

// Execution phase
username = 'Arya';
brothers = ['John', 'Ryan', 'Bran'];
console.log(username, brothers[0]);
message = sayHello(username);
nextMessage = sayHello('Test');
// Declaration Phase
var username = undefined;
let brothers;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

// Execution Phase

username = 'Arya';
brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

message = sayHello(username);
nextMessage = sayHello('Test');
console.log(username, numbers);

var username = 'Arya';
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
// Declaration
var username; //undefined
let number; // not defined
function sayHello(name) { // fn
  return `Hello ${name}`;
}
let message; //not defined
var nextMessage; //undefined

// Execution
console.log(username, numbers);
username = 'Arya';
number = 21;
message = sayHello(username);
nextMessage = sayHello('Test');
console.log(username, numbers);
let username = 'Arya';
let number = 21;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');
// Declaration
let username; // not defined
let number;// not defined
let sayHello;// not defined
let message;// not defined
var nextMessage;// undefined

// Execution
console.log(username, numbers);
username = 'Arya';
number = 21;
sayHello = function (name) {
  return `Hello ${name}`;
};
message = sayHello(username);
nextMessage = sayHello('Test');
let username = 'Arya';
console.log(username, numbers);

let number = 21;
let message = sayHello(username);

let sayHello = function (name) {
  return `Hello ${name}`;
};

var nextMessage = sayHello('Test');
// Declaration
let username; //not defined
let number; // not defined
let message;// not defined
let sayHello;// not defined
var nextMessage;// undefined

// Execution
username = 'Arya';
console.log(username, numbers);
number = 21;
message = sayHello(username);
sayHello = function (name) {
  return `Hello ${name}`;
};
nextMessage = sayHello('Test');
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
// Declaration
var name;
let age;

// Execution
console.log(name);
console.log(age);
name = 'Lydia';
age = 21;
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

sayHi();
// Declaraion
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

// Execution
sayHi();

// Declaration
let name;
var name;
let age;

// Execution
name = 'Lydia';
age = 21;
console.log(name);
console.log(age);
sayHi();
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}
// Declaration
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

// Execution
sayHi();

// Declaration
var name; // not defined
let age; // not defined
// Execution
console.log(name);
console.log(age);
name = 'Lydia';
age = 21;
sayHi();
let sayHi = function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
};
// Declaration
let sayHi; // not defined

// Execution
sayHi(); // ERROR sayHi is not defined. bec of let.

// Declaration function
var name;
let age;
// Execution function
console.log(name);
console.log(age);
name = 'Lydia'
age = 21;
let num1 = 21;
console.log(sum);
var sum = num1 + num2;
let num2 = 30;
// declaration
let num1;
var sum;
let num2;

// execution
console.log(sum);
num1 =21;
sum = num1+num2;
num2 =30;
var num1 = 21;

let sum2 = addAgain(num1, num2, 4, 5, 6);

let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
let num2 = 200;

let sum = add(num1, num2, 4, 5, 6);
// Declaration
var num1;
let sum2;
let add;
function addAgian(a, b) {
  return a + b;
}
let num2;
let sum;

// Execution
num1 = 21;
sum2 = addAgain(num1, num2, 4, 5, 6);

// Function addAgain Decalaration
let a;
let b;
a = num1;
b = num2; // ERROR num2 is not defined. has no value.
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

let add = (a, b) => {
  return a + b;
};
// Declaration
function test(a) {
  let num1 = 21;
  return add(a, num1);
}
let sum; //not defined
let add; //not defined

// Execution
sum = test(100)

// test() declaration
let a;
let num1;
// test() execution
a =100;
num1=21;
add(a,num1)

// add() declartion
// here it'll say add is not defined. because we used let.
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

function add(a, b) {
  return a + b;
}
// Declaration
function test(a) {
  let num1 = 21;
  return add(a, num1);
}
let sum; //not defined
function add(a, b) {
  return a + b;
}

// Execution
sum = test(100)

// test() declaration
let a;
let num1;
// test() execution
add(a,num1)

// add() declaration
let a;
let b;
// add() execution
a = a;
num1 = b;
// 121 returned by add() which is stored in sum variable.
