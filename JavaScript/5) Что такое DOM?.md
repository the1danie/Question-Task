
### Объяснение
**DOM (Document Object Model)** — это интерфейс, через который JavaScript взаимодействует с HTML-документом.  
Когда браузер загружает страницу, он парсит HTML и строит дерево узлов — это и есть DOM.

Каждый HTML-элемент становится объектом, и мы можем обращаться к нему через JavaScript, изменять содержимое, структуру и стили страницы.

---
🧠 На практике:

- Используем `querySelector`, `getElementById` и т.д. — для доступа к узлам.
    
- Работаем с событиями (`addEventListener`) для динамичного поведения.
    
- Изменяем DOM: `appendChild`, `remove`, `classList`, `textContent`, `style` и пр.

```js
const button = document.querySelector('button');
button.addEventListener('click', () => {
  document.body.style.backgroundColor = 'lightblue';
});

```