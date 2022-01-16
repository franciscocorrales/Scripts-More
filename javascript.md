
# JavaScript

### References

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference


### Ternary Operator

```js
let drink = (age >= 21) ? "Beer" : "Juice";
```

### Functions

```js
function(x) { return x%2 === 0; }
```

```js
x => x%2 === 0
```

```js
(x1, x2) => { return x%2 === 0; }
```

```js
const square = x => Math.pow(x, 2);
```

Example, you can use them as functions like this:

```js
const squares = array.map(square);
```

```js
const even = numbers.filter(x => x%2 === 0);
```

### Spread Operator

```js
// Concatenating arrays and objects
let arr1 = [1,2,3]; 
let arr2 = [4,5]; 
let newArray = [...arr1,...arr2]; 
console.log(newArray);
// Output: [ 1, 2, 3, 4, 5 ] 

// Copying array elements
let arr = ["a","b","c"]; 
let newArray = [...arr]; 
console.log(newArray);
// Output: ["a", "b", "c"]

// Expanding arrays
let arr = ["a","b"]; 
let newArray = [...arr,"c","d"]; 
console.log(newArray);
// Output: ["a", "b", "c", "d"]

// Merging objects
const userBasic = { 
	name: "Jen", 
	age: 22,
}; 
const userMoreInfo = { 
	country: "Argentina", 
	city: "Córdoba", 
}; 
const user = {... userBasic, ... userMoreInfo};
// Output: {  name: "Jen",  age: 22, country: "Argentina", city: "Córdoba" }
```

### Optional Chaining 

### Nullish Coalescing Operator

### Arrays

Clone Array shallow

```js
let clonedArray = [...array];
```

Clone Array deep

```js
let cloneArray = JSON.parse(JSON.stringify(array));
```

####  Looping Functions

- map: applying a function over every element and then returning the new array.
- reduce: The reduce() method applies a function against an accumulator and each element in the array (from left to right) to reduce it to a single value.
- filter: Filters elements on an array based on a boolean function.
- every: Got an array and want to test if a given condition is met in every element?
- some: Test if at least one element matches our boolean function.

### Edit/Resend Browser Request

In the Network tab. Right click to the sent request. Select "Copy as Node.js fetch". Paste that in your Console and add the following code before running.
```js
  .then(response => response.json())
  .then(data => console.log(data));
```
Example:
```js
fetch('http://example.com/movies.json', {options})
  .then(response => response.json())
  .then(data => console.log(data));
```



