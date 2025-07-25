
### Объяснение
**Замыкание** — это функция, которая **имеет доступ к переменным из своей внешней (замыкающей) области видимости**, даже после того как внешняя функция завершила выполнение.

Если внутренняя функция **«запоминает» переменные** из внешней, и может использовать их **даже после выхода из этой внешней функции**, — это и есть замыкание.

```js
function outer() {
  let counter = 0;

  return function inner() {
    counter++;
    console.log(counter);
  };
}

const increment = outer(); // outer() выполнена, но inner() "помнит" counter

increment(); // 1
increment(); // 2
increment(); // 3

```

