Find the output of the code snippets below:

```js
console.log(numA + numB); //NaN
var numA = 21,
  numB = 30;
```

Find the output of the code snippets below:

```js
console.log(numA + numB); //RefrenceError: numA is not defined at <anonymous>,
let numA = 21,
  numB = 30;
```

Find the output of the code snippets below:

```js
let numA = 21,
  numB = 30;
console.log(numA + numB); //51
```

Find the output of the code snippets below:

```js
console.log(sayHello()); // Hello
function sayHello() {
  console.log("Hey");
}
function sayHello() {
  console.log("Hello");
}
```

Find the output of the code snippets below:

```js
let username = "Tyrion";
sayHello(); // Tyrion.
function sayHello() {
  console.log(username);
}
```

Find the output of the code snippets below:

```js
sayHello(); //  ReferenceError: can't access lexical declaration 'username' before initialization
let username = "Tyrion";
function sayHello() {
  console.log(username);
}
```

Find the output of the code snippets below:

```js
let username = "Tyrion";
sayHello(); // RefrenceError: sayHello is not defined.
let sayHello = () => {
  console.log(username);
};
```

Find the output of the code snippets below:

```js
sayHello(); // RefrenceError: sayHello is a not defined.
let username = "Tyrion";
let sayHello = () => {
  console.log(username);
};
```

Find the output of the code snippets below:

  ```js
  sayHello(); // : Identifier 'username' has already been declared.
  var username = "Tyrion";
  let sayHello = () => {
    console.log(username);
};
```

Find the output of the code snippets below:

```js
var username = "Tyrion";
sayHello(); // sayHello is not defined.
let sayHello = () => {
  console.log(username);
};
```

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
  var username = "John";
};
sayHello(); //  Uncaught SyntaxError: Identifier 'username' has already been declared
// undefined 
```

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  var username = "John";
  console.log(username);
};
sayHello(); // Uncaught SyntaxError: Identifier 'username' has already been declared
// john
```

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
  let username = "John";
};
sayHello(); // syntaxError:  Identifier 'username' has already been declared.
```