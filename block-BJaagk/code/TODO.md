1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

percentage(45, 60);
percentage(30, 100);
percentage(43, 45);
percentage(17, 19);
percentage(78, 85);

```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

percentage(23, 30);
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};

percentage(45, 60);
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};

percentage(2, 10);
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};

percentage(4, 30);
```

```js
let percentage = (marks, total) => (marks * 100) / total;

percentage(9, 20);
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

<!-- A function definition counts as an expression because it is fundamentally an equality. Furthermore, the function itself is also an object so it lends itself to being manupulated like one. -->

4. Why is a function call an expression in JavaScript?

<!-- It is because it evaluates to a value eventually, which is exactly what an expression does. -->


5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // VALID
five = add; // INVALID
five = five(10, 11); // INVALID
five = function () {
  return 'Hello';
}; // VALID
```

6. What is the difference between function definition and function call? Explain with an example.

A function definition is the description of the steps involved in the function. A function call is one where the function is put to use, so that it evaluates to a final value.

7. What is the similarities between function definition and function call?

<!-- Both of them are expressions. -->

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // VALID



```

9. What is higher order function explain with an example.

<!-- Higher order functions are functions made of functions. They either take up a function as an argument or they might even end up returning a function. -->

10. Explain what is callback function. Why you can pass a function inside a function?

<!-- A callback function is a function that exists within a function, usually as an argument. -->
