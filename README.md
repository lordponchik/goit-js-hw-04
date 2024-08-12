<h1 id="home">Homework :clipboard:</h1>

## goit-js-hw-04


* 🇺🇸 [English](#en)
* 🇺🇦 [Ukrainian](#uk)
* 🇷🇺 [Russian](#ru)

--- 

<h3 id="en">📚 EN 📚</h3>

# Acceptance criteria

- Repository created `goit-js-hw-04`
- When submitting homework there is a link to the source files in the repository
- Each task is executed in a separate file named `task-task_number.js`. Use `<script type="module">`
  to close the job code in a separate scope and avoid identifier name conflicts.
- Variable names are clear and descriptive
- Code formatted using Prettier

# Task 1

Add missing `this` to the methods of the `account` object.

```js
const account = {
  owner: 'Mango',
  balance: 24000,
  discount: 0.1,
  orders: ['order-1', 'order-2', 'order-3'],
  changeDiscount(value) {
    discount = value;
  },
  showOrders() {
    return orders;
  },
  addOrder(cost, order) {
    balance -= cost;
    orders.push(order);
  },
};

account.changeDiscount(0.15);
console.log(account.discount); // 0.15

console.table(account.showOrders()); // ['order-1', 'order-2', 'order-3']

account.addOrder(5000, 'order-4');
console.log(account.balance); // 19000
console.table(account.showOrders()); // ['order-1', 'order-2', 'order-3', 'order-4']
```

# Task 2

Correct the errors that appear in the console so that the script will work.

```js
const inventory = {
  items: ['Knife', 'Gas mask'],
  add(itemName) {
    console.log(`Adding ${itemName} to inventory`);

    this.items.push(itemName);
  },
  remove(itemName) {
    console.log(`Removing ${itemName} from inventory`);

    this.items = this.items.filter(item => item !== itemName);
  },
};

const invokeInventoryAction = function (itemName, action) {
  console.log(`Invoking action on ${itemName}`);
  action(itemName);
};

invokeInventoryAction('Medkit', inventory.add);
// Invoking action on Medkit
// Adding Medkit to inventory

console.log(inventory.items); // ['Knife', 'Gas mask', 'Medkit']

invokeInventoryAction('Gas mask', inventory.remove);
// Invoking action on Gas mask
// Removing Gas mask from inventory

console.log(inventory.items); // ['Knife', 'Medkit']
```

---
---

<h3 id="uk">📚 UK 📚 <a href="#home">⬆ Home ⬆</a></h3> 			

# Критерії прийому

- Створено репозиторій `goit-js-hw-04`
- При здачі домашньої роботи є посилання на вихідні файли у репозиторії
- Кожне завдання виконане в окремому файлі з іменем `task-номер_задания.js`. Використовуй
 `<script type="module">` щоб закрити код завдання в окремій області видимості та уникнути
 конфліктів імен ідентифікаторів
- Імена змінних та функцій зрозумілі, описові
- Код відформатовано за допомогою Prettier

# Завдання 1

Розставь відсутні `this` у методах об'єкта `account`.

```js
const account = {
  owner: 'Mango',
  balance: 24000,
  discount: 0.1,
  orders: ['order-1', 'order-2', 'order-3'],
  changeDiscount(value) {
    discount = value;
  },
  showOrders() {
    return orders;
  },
  addOrder(cost, order) {
    balance -= cost;
    orders.push(order);
  },
};

account.changeDiscount(0.15);
console.log(account.discount); // 0.15

console.table(account.showOrders()); // ['order-1', 'order-2', 'order-3']

account.addOrder(5000, 'order-4');
console.log(account.balance); // 19000
console.table(account.showOrders()); // ['order-1', 'order-2', 'order-3', 'order-4']
```

# Завдання 2

Виправте помилки які будуть в консолі, щоб скрипт запрацював.

```js
const inventory = {
  items: ['Knife', 'Gas mask'],
  add(itemName) {
    console.log(`Adding ${itemName} to inventory`);

    this.items.push(itemName);
  },
  remove(itemName) {
    console.log(`Removing ${itemName} from inventory`);

    this.items = this.items.filter(item => item !== itemName);
  },
};

const invokeInventoryAction = function (itemName, action) {
  console.log(`Invoking action on ${itemName}`);
  action(itemName);
};

invokeInventoryAction('Medkit', inventory.add);
// Invoking action on Medkit
// Adding Medkit to inventory

console.log(inventory.items); // ['Knife', 'Gas mask', 'Medkit']

invokeInventoryAction('Gas mask', inventory.remove);
// Invoking action on Gas mask
// Removing Gas mask from inventory

console.log(inventory.items); // ['Knife', 'Medkit']
```

---
---

<h3 id="ru">📚 RU 📚 <a href="#home">⬆ Home ⬆</a></h3> 

# Критерии приема

- Создан репозиторий `goit-js-hw-04`
- При сдаче домашней работы есть ссылка на исходные файлы в репозитории
- Каждое задание выполнено в отдельном файле с именем `task-номер_задания.js`. Используй
  `<script type="module">` чтобы закрыть код задания в отдельной области видимости и избежать
  конфликтов имен идентификаторов.
- Имена переменных и функций понятные, описательные
- Код отформатирован с помощью Prettier

# Задание 1

Расставь отсутствующие `this` в методах объекта `account`.

```js
const account = {
  owner: 'Mango',
  balance: 24000,
  discount: 0.1,
  orders: ['order-1', 'order-2', 'order-3'],
  changeDiscount(value) {
    discount = value;
  },
  showOrders() {
    return orders;
  },
  addOrder(cost, order) {
    balance -= cost;
    orders.push(order);
  },
};

account.changeDiscount(0.15);
console.log(account.discount); // 0.15

console.table(account.showOrders()); // ['order-1', 'order-2', 'order-3']

account.addOrder(5000, 'order-4');
console.log(account.balance); // 19000
console.table(account.showOrders()); // ['order-1', 'order-2', 'order-3', 'order-4']
```

# Задание 2

Исправь ошибки которые будут в консоли, чтобы скрипт заработал.

```js
const inventory = {
  items: ['Knife', 'Gas mask'],
  add(itemName) {
    console.log(`Adding ${itemName} to inventory`);

    this.items.push(itemName);
  },
  remove(itemName) {
    console.log(`Removing ${itemName} from inventory`);

    this.items = this.items.filter(item => item !== itemName);
  },
};

const invokeInventoryAction = function (itemName, action) {
  console.log(`Invoking action on ${itemName}`);
  action(itemName);
};

invokeInventoryAction('Medkit', inventory.add);
// Invoking action on Medkit
// Adding Medkit to inventory

console.log(inventory.items); // ['Knife', 'Gas mask', 'Medkit']

invokeInventoryAction('Gas mask', inventory.remove);
// Invoking action on Gas mask
// Removing Gas mask from inventory

console.log(inventory.items); // ['Knife', 'Medkit']
```
