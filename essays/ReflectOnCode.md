---
layout: essay
type: essay
title: "Reflect on coding standards with ESLint"
# All dates must be YYYY-MM-DD format!
date: 2020-02-13
labels:
  - JavaScript
  - ES6
  - Learning
---
  ESLint is an open source JavaScript linting tool made to help JavaScript programmer's write clean code that adheres to some strict coding standards. For the past week we have been using ESLint in IntelliJ to check our code for errors. This tool has been helpful in making the code we write look presentable to whoever might want to read it. Having real time error reporting With ESLint has helped me improve my code overall because I can immediately see that I have messy code by professional standards and can take action in changing my bad habits.


Example of messy code:
---
```js
function numEvenNums(array){
  let i;
  let x;
  let total=0;
  for(i=0;i<array.length;i++){
    if((array[i]%2)===0){

      total++;
    }
  }

  return total;
}
```
As you can see, this code above is kind of hard to read because the code is so smashed together. This code example even includes a variable that has not even been used. This will all show up with ESLint as red under-lines as if you missed spelled something.

Example of cleaned code with ESLint:
---
```js
function numEvenNums(array) {
  let i;
  let total = 0;
  for (i = 0; i < array.length; i++) {
    if ((array[i] % 2) === 0) {
      total++;
    }
  }
  return total;
}
```
This is the same code written with ESLint enabled. The code is much more readable and there are no unnecessary lines, spaces, or variables anywhere in the code. besides the lack of comments above the function, this is efficient clean code.

Conclusion:
---
I believe ESLint is a very effective tool for JavaScript beginners because it starts you off learning the correct way to do things by the standards of the industry professionals
