# Destructuring_All_About


# **Destructuring in JavaScript/TypeScript**

## **What is Destructuring?** 🤔  
Destructuring is a **shortcut** in JavaScript/TypeScript that allows you to **extract values from arrays or objects** easily. It makes the code **shorter and more readable**.

---

## **1️⃣ Array Destructuring**
Array destructuring allows us to **extract specific values based on index**.

### 🔹 **Without Destructuring:**
```js
const numbers = [10, 20, 30];

const first = numbers[0];
const second = numbers[1];

console.log(first, second); // 10 20
```

### 🔹 **With Destructuring:**
```js
const numbers = [10, 20, 30];

const [first, second] = numbers; // Extracting first two values

console.log(first, second); // 10 20
```

✅ **Benefit:** Short and clean syntax

---

## **2️⃣ Object Destructuring**
Object destructuring allows us to **extract properties easily**.

### 🔹 **Without Destructuring:**
```js
const user = {
  name: "Amit",
  age: 25,
  city: "Delhi"
};

const name = user.name;
const age = user.age;

console.log(name, age); // Amit 25
```

### 🔹 **With Destructuring:**
```js
const user = {
  name: "Amit",
  age: 25,
  city: "Delhi"
};

const { name, age } = user; // Extracting name and age

console.log(name, age); // Amit 25
```

✅ **Benefit:** Code becomes short and more readable

---

## **3️⃣ Default Values**
If a **value is undefined**, we can set a default value.

```js
const user = { name: "Rahul" };

const { name, age = 30 } = user;

console.log(name, age); // Rahul 30
```

---

## **4️⃣ Destructuring in Function Parameters**
Destructuring can also be used **inside function parameters**.

### 🔹 **Without Destructuring:**
```js
function printUser(user) {
  console.log(user.name, user.age);
}

printUser({ name: "Sara", age: 28 });
```

### 🔹 **With Destructuring:**
```js
function printUser({ name, age }) {
  console.log(name, age);
}

printUser({ name: "Sara", age: 28 });
```

✅ **Benefit:** Direct access to properties inside the function without extra code.

---

## **Why Use Destructuring?** 🤷‍♂️  
✅ **Shorter and more readable code**  
✅ **Faster execution** as properties are extracted directly  
✅ **Default values can be set**  
✅ **Easier access to function parameters**  

---

💡 **Did you understand? Let me know if you need more examples!** 🚀

