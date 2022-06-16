Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(username); // username is not Defined.
//In above code we are looking for the variable named usename. There is no variable named username in the global scope. The variable is inside the function named hello and we can't access the variable defined inside a function from outside.

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme); // Reference Error username is not defined.
```

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(useranme); // Reference Error username is not defined.
```

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); // useranme is not defined.
```

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); // In above code we are looking for the variable named username. There is a variable named username in the global scope. The variable is also redeclared inside the if condition.

//  Identifier 'username' has already been declared.
```

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(useranme); //In above code we are looking for the variable named username. There is a variable named username in the global scope. The variable is also redeclared inside the if condition which will not be accessed, as it doesn't get inside the condition.

```

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(useranme); // useranme is not define.
```

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output

 0 'First'
 1 'First'
 2 'First'
 3 'First'
 4 'First'
 5 'First'
 6 'First'
 7 'First'
 8 'First'
 9 'First'
 10 'Second'
 
//In above code the for loop will execute first and give the output for increment of numbers from 0 to 9 an per the condition given, then ouside the loop the incremented value of i will be displayed in the second console, as the variable i is declared through a var datatype, which is a globle scope.

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
 0 'First'
 1 'First'
 2 'First'
 3 'First'
 4 'First'
 5 'First'
 6 'First'
 7 'First'
 8 'First'
 9 'First'
}
console.log(i, 'Second'); // ReferenceError: i is not defined
    at <anonymous>:

    // /In above code the for loop will execute first and give the output for increment of numbers from 0 to 9 an per the condition given, then ouside the loop the incremented value of i will be displayed in the second console, as the variable i is declared through a let datatype, which is not a globle scope.
```
