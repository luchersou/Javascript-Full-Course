# Objects in JavaScript

This guide explains how **objects** work in JavaScript, with practical examples.

---

## 1. What is an Object
An **object** is a collection of **key–value pairs**.

```javascript
const person = {
  name: "Lucas",
  age: 27,
  active: true
};

console.log(person.name);     // "Lucas"
console.log(person["age"]);   // 27
```

---

## 2. Adding, Updating, and Removing Properties
```javascript
const person = { name: "Lucas" };

person.lastName = "Souza";       // add
person.name = "Lucas Herzinger"; // update
delete person.lastName;          // remove

console.log(person); // { name: "Lucas Herzinger" }
```

---

## 3. Methods (Functions inside Objects)
```javascript
const user = {
  name: "Lucas",
  greet: function() {
    console.log(`Hello, my name is ${this.name}`);
  }
};

user.greet(); // "Hello, my name is Lucas"
```

> `this` refers to the current object.

---

## 4. Nested Objects
```javascript
const car = {
  brand: "Toyota",
  model: "Corolla",
  engine: {
    type: "1.8",
    power: "140hp"
  }
};

console.log(car.engine.power); // "140hp"
```

---

## 5. Iterating Over Objects
```javascript
const product = { name: "Laptop", price: 3500 };

for (let key in product) {
  console.log(`${key}: ${product[key]}`);
}

console.log(Object.keys(product));    // ["name", "price"]
console.log(Object.values(product));  // ["Laptop", 3500]
console.log(Object.entries(product)); // [["name","Laptop"],["price",3500]]
```

---

## 6. Objects Are References
```javascript
const a = { name: "Lucas" };
const b = a;

b.name = "John";
console.log(a.name); // "John"
```

> To create a copy without linking them:

```javascript
const original = { x: 10, y: 20 };
const copy = { ...original };

copy.x = 99;
console.log(original.x); // 10
```

---

## 7. Creating Objects in Other Ways

### 7.1 `new Object()`
```javascript
const person = new Object();
person.name = "Lucas";
```

### 7.2 Constructor Functions
```javascript
function Person(name, age) {
  this.name = name;
  this.age = age;
}

const p1 = new Person("Lucas", 27);
console.log(p1.name); // "Lucas"
```

### 7.3 Classes (ES6)
```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  introduce() {
    console.log(`I'm ${this.name}, I'm ${this.age} years old.`);
  }
}

const p2 = new Person("Lucas", 27);
p2.introduce(); // "I'm Lucas, I'm 27 years old."
```

---

## 8. Practice Exercise
Create an object `BankAccount` with:
- `owner`
- `balance`
- method `deposit(amount)`
- method `withdraw(amount)` (check balance before withdrawing)

```javascript
const bankAccount = {
  owner: "Lucas",
  balance: 1000,
  deposit(amount) {
    this.balance += amount;
    console.log(`Deposited $${amount}. Current balance: $${this.balance}`);
  },
  withdraw(amount) {
    if (amount <= this.balance) {
      this.balance -= amount;
      console.log(`Withdrew $${amount}. Current balance: $${this.balance}`);
    } else {
      console.log("Insufficient funds!");
    }
  }
};

bankAccount.deposit(500);
bankAccount.withdraw(300);
bankAccount.withdraw(1500);
```

---

## 9. Summary
- Object = collection of **properties** and **methods**
- `this` → refers to the current object
- Classes → templates for creating multiple objects
- Copying objects requires care due to **references**

---

© 2025 Quick guide by ChatGPT for Lucas Souza
