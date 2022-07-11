1. Write a function that accepts a callback function and return another function. But the function should only be called once.

```js
function once(cb) {
  let isCalled =false;
  return function() {
    if(!isCalled){
      cb();
      isCalled
    }else {
        return(`Can't we Twice`);
    }  
  }
  
}

// TEST
function sayHello() {
  alert('Call me once!');
}
let log = once(sayHello);
log(); // alert message "You can only call me once!"
log(); // return undefinde (can't be called twice)
```

2. Change the above function in such a way that the function accepts two parameter a callback function and parameter for the callback function. When calling the function pass the parameters.

```js
function once(cb,params) {
  // your code goes here
  let isCalled = false;
  return function (params) {
    if (!isCalled) {
      cb(params);
      isCalled = true;
    }else{
      return  ("can't be called twice");
    }
  }

}

// TEST
let log = once(console.log, 'Hello Console');
log(); // log message "Hello Console"
log(); // return undefinde (can't be called twice)
```

3. Change the above function in such a way that it can accept `n` number of parameters for the callback function.

**For handling `n` number of parameter use `rest` parameters `...` or predefined arguments variable present in every function declaration.**

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/rest_parameters

```js
function once(cb ,...rest) {
  // your code goes here
    let isCalled = false;
    return function (){
        if(!isCalled){
            cb(...rest);
      isCalled = true;
        }else{
        alert('you can call this  Functions again');
              }
    }
}

// TEST
let log = once(console.log, 'Message one', 'Message Two');

undefined
log();
//output Message one Message Two
```

4. Create a new function `nTimes` whose 1st parameter is a callback function, 2nd parameter is the number of times the function should be called and 3rd ... nth parameter should be passed to the callback function.

```js
function nTimes(cb, times, ...rest) {
  // your code goes here
    let numberOfTimesCalled = 0;
    return function (){
        if( numberOfTimesCalled >= times){
            alert(`You Can't call this function more than ${times} times!`)} else{
            cb(...rest);
            numberOfTimesCalled = numberOfTimesCalled + 1;
        }
    }
}
let log = (msg) => console.log(msg);
let logThreeTimes = nTimes(log, 3, 'Hello Arya');
logThreeTimes(); // log message "Hello Arya" (1)
logThreeTimes(); // log message "Hello Arya" (2)

//outputg
// VM2136:12 Hello Arya
// VM2136:12 Hello Arya

// TEST
let log = (msg) => console.log(msg);
let logThreeTimes = nTimes(log, 3, 'Hello Arya');
logThreeTimes(); // log message "Hello Arya" (1)
logThreeTimes(); // log message "Hello Arya" (2)
logThreeTimes(); // log message "Hello Arya" (3)
log(); // return undefinde (can't be called)
```
