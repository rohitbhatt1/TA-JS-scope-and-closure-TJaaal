1. What does thread of execution means in JavaScript?

<!-- ans -->
Whenever a piece of code is executed line by line in JavaScript, it is known as thread of execution..(i.e. executing second line after first line.).


2. Where the JavaScript code gets executed?
<!-- ans. -->
javaScript code gets executed in JavaScript Engine. As code execution starts, JavaScript creates a Global Execution Context, in which there is a specific memory section.GEC then After execution of function the value is stored and the FEC is deleted and then next line is executed.

3. What does context means in Global Execution Context?
<!-- ans -->
It is a  environment in which any code gets executed.

4. When do you create a global execution context.
<!-- ans -->
As soon as a code snippet is created JavaScript creates a global execution context.

5. Execution context consists of what all things?
<!-- ans -->
Execution context is a concept in the language spec that—in layman's terms—roughly equates to the 'environment' a function executes in; that is, variable scope (and the scope chain, variables in closures from outer scopes), function arguments, and the value of the this object.

6. What are the different types of execution context?
<!-- ans. -->
Global execution context (GEC) and function execution context (FEC).

7. When global and function execution context gets created?
<!-- ans -->
Global execution context is created only once for a program, function execution context is created in global execution context as many times a function is created.

8. Function execution gets created during function execution or while declaring a function.
<!-- ans -->
during the Execution Funtion.

9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);//"Hello Arya";
```


<!-- Put your image here -->

![](./img/image-name.jpg)




```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);//
var percentageProfit = getPercentage(400, 200);//
```

<!-- Put your image here -->

![](.)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)
