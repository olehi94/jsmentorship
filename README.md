# JS Mentorship

### For vs forEach() vs for/in vs for/of in JavaScript
```javascript 
* for (let i = 0; i < arr.length; ++i)
* arr.forEach((v, i) => { /* ... */ })
* for (let i in arr)
* for (const v of arr)
```
The `for`and `for/in` looping constructs give you access to the index in the array, not the actual element.