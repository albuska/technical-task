# Технічне завдання від компанії GoIt

---

## Створення персонального бекенду:

- UI-сервіс [mockapi.io](https://mockapi.io/projects).

---

## Застосований стек технологій:

- HTML
- CSS
- JavaScript
- React.js
- Hooks
- Axios
- Figma
- Git Hub
- Vite

---

## Використані бібліотеки

- [Notiflix](https://www.npmjs.com/package/notiflix)
- [Modern-normalize](https://www.npmjs.com/package/modern-normalize)
- [Prop-types](https://www.npmjs.com/package/prop-types)
- [React-icons](https://www.npmjs.com/package/react-icons)
- [React-loader-spinner](https://www.npmjs.com/package/react-loader-spinner)
- [React-router-dom](https://www.npmjs.com/package/react-router-dom)
- [React-select](https://react-select.com/home)
- [React-typewriter-effect](https://blog.logrocket.com/code-block-typewriter-effect-react/)
- [Styled-components](https://styled-components.com/)

---

## Мета: Створити картки твітів та додати інтерактивності при клікові на кнопку.

---
[Посилання на макет](https://www.figma.com/file/zun1oP6NmS2Lmgbcj6e1IG/Test?type=design&node-id=0-1&t=5VDfFa5NoTZg8xoz-0)

---

### Критерії виконання

- Верстка фіксована в рх, семантична та валідна.
- Немає помилок в консолі браузера.
- Робота виконана на нативному JS з використанням зборщиків або на React.
- Інтерактивність працює відповідно до технічного завдання.
- Код відформатований та без коментарів.
- В репозиторії має бути описаний README.md.

---

### Технічне завдання

1. Відповідно до макету потрібно реалізувати картки юзера.
2. При клікові на кнопку Follow - текст змінюється на Following. Також
   змінюється колір кнопки. А до кількості фоловерів додається і ваш. Тобто,
   початкова кількість складає 100,500 фоловерів. При клікові на кнопку буде
   100,501.
3. При оновлені сторінки має фіксуватись кінцевий результат дій юзера. Тобто,
   якщо клікнути по кнопці і оновити сторінку - то кнопка все рівно залишається
   в стані Following із відповідним кольором, а кількість фоловерів НЕ
   зменшується до початкового значення.
4. При повторному клікові на кнопку її текст та колір змінюються до початкового
   стану. Також змінюється і кількість фоловерів. Вона зменшується на 1
   (100,500).
5. В коді цифра 100,500 має бути прописана одним значенням (100500). В UI -
   виведено через кому (100,500).

---

Створи свій персональний бекенд для розробки за допомогою UI-сервісу mockapi.io.
Створи ресурс users. Використай конструктор ресурсу та опиши об'єкт юзера, як
описано нижче.

---

#### Юзер

1. Створюєте юзера в Mockapi з наступними полями: id, user, tweets, followers,
   avatar (див скріншот нижче).
2. Зображення аватарів мають бути прописані окремими url у властивості “avatar”.
   Можете підібрати їх самостійно.
3. Має бути від 12 юзерів з різними значеннями(на ваш розсуд) в базі. Зроби
   пагінацію. На одній сторінці пагінації має відображатися від 3 твітів, решта
   підгружатись при натисканні Load More
4. Решта вимог аналогічні до вищеописаного технічного завдання.

---

### Додаткове завдання

Створи маршрутизацію, використовуючи React Router.

У застосунку повинні бути такі маршрути. Якщо користувач зайшов за неіснуючим
маршрутом, його необхідно перенаправляти на домашню сторінку. '/' – компонент
Home, домашня сторінка. Стилізація та оформлення на ваш розсуд '/tweets' -
компонент tweets, сторінка із відображенням твітів На сторінці tweets має бути
кнопка Back, яка веде на головну сторінку.

#### Завдання із зірочкою

Додай фільтрацію. Це має бути Dropdown із 3 опціями(оформлення на ваш розсуд):
show all, follow, followings show all - показати всі твіти. follow - показати
твіти, у яких стан follow. followings - показати твіти, у яких стан following
