Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme); // output
```

'Username' is what we are looking for, but since it's defined within curly braces and const is a block scope tool, we will the following error: VM21:4 Uncaught ReferenceError: useranme is not defined

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(username); // output
```

Once again, we are looking for `username`, but since it's tucked away within the if condition by 'let' it does not exist in the global scope and cannot be accessed, thereby spitting out a reference error: VM91:4 Uncaught ReferenceError: username is not defined
    at <anonymous>:4:13

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); // Arya
```

We are looking for `username` and since it's defined by the var keyword, it allows it to exist in the global scope, thereby enabling it to be accessed outside the if condition.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(username); // output
```

We are looking for `username` but since it has already been declared at the beginning using the let keyword and there is an attempt to change it's value at line three, the program will encounter an error and publish the following:
Uncaught SyntaxError: Identifier 'username' has already been declared

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // output
```

We are looking for `username` but since it has already been declared at the beginning using the let keyword and there is an attempt to change it's value at line three, the program will encounter an error and publish the following:
Uncaught SyntaxError: Identifier 'username' has already been declared

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // output
```

We are looking for `username` but since it has already been declared at the beginning using the let keyword and there is an attempt to change it's value at line three, the program will encounter an error and publish the following:
Uncaught SyntaxError: Identifier 'username' has already been declared

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // 0 'First'
VM158:2 1 'First'
VM158:2 2 'First'
VM158:2 3 'First'
VM158:2 4 'First'
VM158:2 5 'First'
VM158:2 6 'First'
VM158:2 7 'First'
VM158:2 8 'First'
VM158:2 9 'First'
}
console.log(i, 'Second'); // 10 'Second'
```

Since this is a for statement, var is pegged to be 0 at the beginning and is then taken through the loop till it termiantes at i = 9, after which it moves on to the next line and executes that function with the then value of i, which is 10.


9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```

Since this is a for statement, var is pegged to be 0 at the beginning and is then taken through the loop till it termiantes at i = 9, after which it moves on to the next line and executes that function with the then value of i, which is 10.

