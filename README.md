# JS Mentorship

### For vs forEach() vs for/in vs for/of in JavaScript
```javascript 
for (let i = 0; i < arr.length; ++i)
arr.forEach((v, i) => { /* ... */ })
for (let i in arr)
for (const v of arr)
```
The `for`and `for/in` looping constructs give you access to the index in the array, not the actual element.
```javascript 
for (let i = 0; i < arr.length; ++i) {
  console.log(arr[i]);
}

for (let i in arr) {
  console.log(arr[i]);
}
```
With the other two constructs, `forEach()` and `for/of`, you get access to the array element itself. With `forEach()` you can access the array index `i`, with `for/of` you cannot.
```javascript 
arr.forEach((v, i) => console.log(v));

for (const v of arr) {
  console.log(v);
}
```

### Инициализация и объявление переменной. Область видимости. Hoisting(поднятие переменной). var VS let VS const. let VS const.
* Когда в JavaScript создаётся переменная, она инициализируется со значением `undefined`
* В JavaScript есть два типа области видимости — глобальная и локальная (`global scope` и `function scope`)
* Если переменная создаётся внутри объявления функции, то её область видимости определяется как локальная и ограничивается этой функцией.
* переменные, объявлены оператором var, они относятся к функции и доступны вне цикла.
* **создании переменной в JavaScript, она инициализируются со значением undefined. Это и есть «Hoisting»**.