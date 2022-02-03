1. What does thread of execution means in JavaScript?

<!-- Thread of execution refers to the sequence folllowec by the JavaScript engine to run through a program. -->

2. Where the JavaScript code gets executed?

<!-- It gets executed in the JavaScript engine. -->

3. What does context means in Global Execution Context?

<!-- It refers to the base on top of which the rest of the program is executed. -->

4. When do you create a global execution context.

<!-- It is created at the beginning of a program and is created only once. -->

5. Execution context consists of what all things?

<!-- There are two kinds of execution context: global and functional. Each of them have an execution path and a memory container. -->

6. What are the different types of execution context?

<!-- Global execution context and functional execution context. -->

7. When global and function execution context gets created?

<!-- Global execution context gets created at the beginning of a program while the function execution context gets created every time a function is invoked. -->

8. Function execution gets created during function execution or while declaring a function.

<!-- This happens during the function execution. -->


9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



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