## 1.Why do we use functions in JavaScript?
Ans-We can reuse code: Define the code once, and use it many times.

We can use the same code many times with different arguments, to produce different result
## 2.What is Function Invocation?
Ans- The code inside a function is not executed when the function is defined. The code inside a function is executed when the function is invoked. It is common to use the term "call a function" instead of "invoke a function". It is also common to say "call upon a function", "start a function", or "execute a function".
example->
```js
function myFunction(a, b) {
  return a * b;
}
myFunction(10, 2);
```

## 3.Does a function behave like an object in Javascript? Prove it by an example.
Ans- Yes, In JS the function can behave as an object as they are first-class objects. So one can assign functions to variables, array elements and other objects.
example->
```js
let circle = {
  radius: 10,
  area: function () {
    return Math.PI * this.radius * this.radius;
  },
};

console.log(circle.area());
console.log(typeof circle.area); 
```
## 4.What are Events in Javascript?
Ans- JavaScript's interaction with HTML is handled through events that occur when the user or the browser manipulates a page.

When the page loads, it is called an event. When the user clicks a button, that click too is an event. Other examples include events like pressing any key, closing a window, resizing a window, etc
example-
```js
<button onclick="document.getElementById('demo').innerHTML = Date()">The time is?</button>
```
## 5.What is a string?
Ans- JavaScript strings are for storing and manipulating text.

A JavaScript string is zero or more characters written inside quotes.
example-
```js
let text = "We are the so-called "Vikings" from the north.";
```
## 6.What is an array? Is it static or dynamic in Javascript?
Ans- The array object in js is used to store multiple values in a single variable. They are zero-indexed.

Arrays in JS are dynamic by nature meaning, they can be modified even after definition, and can increase or decrease in size.
## 7. Difference between Map and Set?
Ans- Map is a collection of keyed data items, just like an Object. But the main difference is that Map allows keys of any type.

Methods and properties are:

new Map() – creates the map.
map.set(key, value) – stores the value by the key.
map.get(key) – returns the value by the key, undefined if key doesn’t exist in map.
map.has(key) – returns true if the key exists, false otherwise.
map.delete(key) – removes the value by the key.
map.clear() – removes everything from the map.
map.size – returns the current element count.

A Set is a special type of collection, where each value may occur only once.
Methods and Properties of Set:

new Set(iterable): creates the set and if an iterable object, copies values from it into the set.
set.add(val) and set.delete(val): The add method adds a value and returns the set. The delete method will remove the value and will return true if the value existed at the moment the function was called.
set.has(val): Returns true if the Set has the value.

## 8.Difference between Array and Map?
Ans-The array object in js is used to store multiple values in a single variable
example-
```js
let arr = [];
// Or
let arr2 = new Array();
```
map:-
A map is a collection of keyed data items, just like an Object. But map allows keys of any type.
example-
```js
let map = new Map();
map.set(1, "Nathan");
map.set("Lorem", "Ipsum");
```
### 9.What are array methods? List a few names?
Ans-rrays provide a lot of methods. To make things easier, in this chapter they are split into groups.

Add/remove items
We already know methods that add and remove items from the beginning or the end:

arr.push(...items) – adds items to the end,
arr.pop() – extracts an item from the end,
arr.shift() – extracts an item from the beginning,
arr.unshift(...items) – adds items to the beginning.

## 10.
Ans-There are many ways in which we can iterate over an array
for Loop
2.foreach()
3.whileloop
4.map()

## Programs->
1. Reverse an array
```js
let arr = [1,2,3,4,5];
arr = arr.reverse();
console.log(arr);
```
2.Join array
```js

<script> 
   function func() { 
      var a = [ 1, 2, 3, 4, 5, 6 ]; 
      document.write(a.join('|')); 
   } 
   func(); 
< /script> 
output:
1|2|3|4|5|6
```

3.
```html
<h1>JavaScript Arrays</h1>
<h2>The forEach() Method</h2>

<p>forEach() calls a function for each element in an array:</p>

<p id="demo"></p>
```
```js
let text = "";
const fruits = ["apple", "orange", "cherry"];
fruits.forEach(myFunction);

document.getElementById("demo").innerHTML = text;
 
function myFunction(item, index) {
  text += index + ": " + item + "<br>"; 
}
```
4.Merge to sets in javascript
```js
let setA = new Set([1, 2, 3, 4]);
let setB = new Set([2, 3]);
console.log(Set.union(setA, setB));
output:
Set { 1, 2, 3, 4 }
```
