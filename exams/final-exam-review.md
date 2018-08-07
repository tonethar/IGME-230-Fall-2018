# Final Exam Review

The exam is cumulative, so everything we have covered this semester is fair game. 

## I. Topics covered since midterm

### I-A. Intro to Web Apps
Most of this is new: https://github.com/tonethar/IGME-230-GDD-2017-Fall/blob/master/notes/web-apps-0.md

All of the content above is fair game. Be sure to look over the review questions and assignments for chapters 1-10


### I-B. Intro to PixiJS
https://github.com/tonethar/IGME-230-GDD-2017-Fall/blob/master/notes/pixi-js-0.md

**Major topics:**
- Factoids about PixiJS
- ES6 classes, constructors, inheritance, `this`
- CORS
- Sprite Hierarchy


### I-C. Weekly Notes
Week 8+ in [weekly](../weekly/) covers the newer material. 



## II. Concepts that may be tested

### CSS Selectors
Be able to write CSS rules using these selectors:
- universal,type,class,id
- descendant
- attribute
- selectors for button states

### The DOM & DOM Methods
- which DOM method have we been using to get a reference to a single element on a web page?
- which DOM method have we been using to get references to multiple elements on a web page?
- how do you set and get the attribute values of DOM elements?
- which method is used to add elements to the DOM tree?
- which method is used to remove elements from the DOM tree?

### Variables & Types
- is JavaScript a dynamically typed or statically typed language? What is the major difference between these types of languages?
- what does `"use strict"` do?
- how do you create a *block* in JavaScript?
- define what variable *scope* is.
- how are variables *scoped* when declared with `let` and `const`?
- how are variables *scoped* when declared with `var`?
- in regards to `let` and `const` declared variables, what is a "temporal dead zone" and how is it caused?
- are function *declarations* **hoisted** in JavaScript?
- are function *expressions* **hoisted** in JavaScript?
- give examples of JS reference types and JS value types.
- how does the behavior of `const` vary when dealing with (primitive) value types, as opposed to reference types?
- what is a *falsy* value?
- list JavaScript's 7 falsy values.

### Functions
- write a function named *addThem* that takes two arguments and returns their sum. Be sure you can write this both as a standard function, and as an ES6 arrow function.
- write a function (arrow or standard) named *addThem2* that takes two arguments and returns their sum. If either parameter is not passed in,  they will have default values of `0`.
- write a function that takes another function as an argument, and then calls that passed in function.

### Arrays
- <s>write a *testing function* for use with `array.filter()` that puts objects with a `.y` of less than -10 in the returned array</s>
- <s>write a *comparator function* for use with `array.sort()` that puts objects with a `.alive` value of `true` at the beginning of the array</s>
- give 3 ways to loop through an array
- how are JS *typed arrays* different from the standard JS `Array`

### Events
- compare and contrast *event handlers* and *event listeners*
- why will this line of code - `window.onload=init();` - fail? (assume that the `init()` function is correctly defined elsewhere)
- why will this line of code - `window.addEventListener("onload",init);` - fail? (assume that the `init()` function is correctly defined elsewhere)

### Classes & Objects
- create an object literal with at least 2 properties, and at least one method that acts upon those properties
- create an ES6 `class` with at least 2 properties, and at least one method that acts upon those properties
- what is the keyword used when a JS class inherits from another JS class?
- which `Object` static method is used to prevent an object from having new properties added to it?
- which `Object` static method is used to prevents an object from having new properties added to it, and also prevents the values of those properties from changing?
- which JS methods are used to *serialize* and *deserialize* objects?

### Web Services (these are in the notes, and in Wikipedia)
- define *Ajax*
- define *web service*
- define *API Key*
- define *Query String*

### Acronym Soup
What do the following stand for?
- HTML, CSS, FTP, HTTP, DOM
- Ecma (trick question)
- CRUD
- DRY
- JSON
- CDN

### Other Concepts
- Separation of Concern
- Method Chaining
- Fluent Interfaces
- Subclass Sandbox
- Rendering Engine
- Display List


## III. Sample Questions (not exhaustive of what could be asked)

### A - CSS/HTML
*To answer these questions you need to know how CSS selectors work - here are some resources:*
- https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors
- https://www.w3.org/TR/2018/CR-selectors-3-20180130/

1. Write a CSS rule that will select an element that has an id value of "content", and give it a background color of green.

2. Write a CSS rule that will select all elements of class "important", and give them a font size color of 16 points.

3. Write a CSS rule that will select only those links on the page that have an `href` value equal to `http://www.google.com`

4. Write a CSS rule that will select only those links on the page that have an `href` value that contains the text `google`

5. Write a CSS rule that will select all &lt;b> elements that are *descendants* of &lt;p> elements

6. Write a CSS rule that will select all &lt;b> elements that are *children* of &lt;p> elements

7. Write a CSS rule that causes a link to turn green when the mouse is pressed down over it

8. Write a CSS rule that selects &lt;h1>, &lt;h2> and &lt;h3> tags and gives them a color of red

9. Write a CSS rule that selects all of the elements on a page and gives them a font size of 10 pixels

10. Re-write this HTML so that the &lt;p> element below belongs to both the `hoser` and `takeoff` classes:

`<p><i>Strange Brew</i> is my favorite movie!</p>` 

### B - JavaScript & DOM
*To answer these questions you need to know how CSS selectors work, as well as `querySelector()` and `querySelectorAll()`*

1. Write JS that selects **all** of the &lt;img> tags on a HTML page and stores them in an array, loops through the array, and gives each a `title` atttribute with the value of "I am an image"!"

1. Write JS that loops through the `colors` array, and creates an unordered list of the contents of the array. When you are done creating the array, don't forget to add it to the page.

`let colors = ["red","green","blue"];`

### C - JS Objects

*To answer these questions, you will need to read up on [Object Literals](./web-apps-7.md) and [ES6 classes](./pixi-js-2.md)*

1. Create an ES6 *class* called `Person`. Its constructor will take two arguments `name` and `height`, and assign those passed in values as properties of the `Person object`. `Person` will have a `grow()` method that causes that instance's height to increase by 1.

2. Create a JS *object literal* named `rover` that has 2 properties `breed` and `age`. The object will also have a method named `getOlder()` which will increase age by 1.

3. What is the output of this statement? Will it produce an error message?

```js
"use strict";
let car = {"cylinders":4};
console.log(car.color);
```

4. What is the output of this statement? Will it produce an error message?

```js
"use strict";
let car = {"cylinders":4};
car.color = "red";
console.log(car.color);
```

5. What is the output of this statement? Will it produce an error message?

```js
"use strict";
let car = {"cylinders":4};
Object.seal(car);
car.color = "red";
console.log(car.color);
```

6. What is the output of this statement? Will it produce an error message?

```js
"use strict";
let car = {"cylinders":4};
Object.freeze(car);
car.cylinders = 8;
console.log(car.cylinders);
```



### D - Truthy/Falsy Values
*To answer these questions you need to know JavaScript's 6 (or 8 depending on how you count) **falsy** values. In a JavaScript boolean context (like an `if` statement), if a value doesn't evaluate to one of these 8 falsy values, it is **true***

- See [web-apps-2.md](web-apps-2.md#section10)

1. What will be logged for this line of code? Why?

```js
if(""){
  console.log("Guns!");
}else{
  console.log("Butter!");
}
```

2. What will be logged for this line of code? Why?

```js
if("false"){
  console.log("Guns!");
}else{
  console.log("Butter!");
}
```

3. What will be logged for this line of code? Why?

```js
if([]){
  console.log("Guns!");
}else{
  console.log("Butter!");
}
```

4. What will be logged for this line of code? Why?

```js
if([].length){
  console.log("Guns!");
}else{
  console.log("Butter!");
}
```

5. What will be logged for this line of code? Why?

```js
if([null,undefined,true,false][0]){
  console.log("Guns!");
}else{
  console.log("Butter!");
}
```

### E - Variable Scope
*To answer these questions, you have to understand how [var](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var), [let](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let), and [const](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const) work*

1. What will be logged below? Why?

```js
let x = 0;
x++;
console.log(x);
y++;
let y = 0;
console.log(y);
```

2. What will be logged below? Why?

```js
let x = 1;
let y;
if(x==1){
	x++;
	let y = 1;
	y++;
	let z = 1;
 }
 console.log(x);
 console.log(y);
 console.log(z);
```

3. What will be logged below? Why?

```js
doStuff()
console.log(x);

function doStuff(){
	console.log("doStuff!");
	x = 1;
}
```

4. What will be logged below? Why?

```js
"use strict";
doStuff()
console.log(x);

function doStuff(){
	console.log("doStuff!");
	x = 1;
}
```

5. What will be logged below? Why?

```js
doStuff()
console.log(x);

function doStuff(){
	console.log("doStuff!");
	var x = 1;
}
```

6. What will be logged below? Why?

```js
doStuff()

function doStuff(){
  if(true){
    if(!false){
      for(let i=0;i<10;i++){
	var x = 1;
        let y = 2;
        const z = 3;
      }
    }
  }
   console.log(x);
   console.log(y);
   console.log(z);
}
```

### F - Value Types v. Reference Types
*To answer these questions, you need to know the difference between JavaScript **value** types and **reference** types*

- Info here: [web-apps-7.md](./web-apps-7.md#section7)

1. What will be logged below? Why?

```js
  let x = "1";
  let y = x;
  x = "2";
  console.log(x);
  console.log(y);
```

2. What will be logged below? Why?

```js
  let x = [1,2,3];
  let y = x;
  x.push(4);
  y.push(5);
  console.log(x);
  console.log(y);
```

### G - Variable Immutability

*To answer these questions, you need to know how `const` immutability works in JavaScript*

- Info here: [web-apps-7.md](web-apps-7.md#section8)

1. What will be logged below? Why?

```js
const x = {};
x.name = "fred";
console.log(x);
```

2. What will be logged below? Why?

```js
const y = 1;
y++;
console.log(y);
```

3. What will be logged below? Why?

```js
const z = {};
z = {"name":"mary"};
console.log(z);
```
