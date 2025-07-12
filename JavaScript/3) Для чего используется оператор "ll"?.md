
### Объяснение
Оператор `||` в JavaScript — это **логический ИЛИ** (логическое "или").
Он возвращает `true`, если **хотя бы одно** из условий истинно:

```js
true || false    // true
false || true    // true
false || false   // false

console.log('hello' || 'world'); // 'hello' (первое — истинное)
console.log(null || 'fallback'); // 'fallback' (null — ложное)
console.log(0 || false);         // false (оба ложные, вернёт последнее)

```