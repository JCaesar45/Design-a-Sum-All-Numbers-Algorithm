````markdown
# Sum All Numbers Algorithm

## 📘 Description

This project implements a simple algorithm to **sum all numbers between two given values (inclusive)**. The values are provided as a two-element array. The algorithm ensures proper order regardless of the input sequence.

## ✅ User Story

- The function should be named `sumAll`.
- It must accept **an array of two numbers**.
- It should return the sum of **both numbers and all numbers in between**, regardless of their order.

### Example:
```js
sumAll([4, 1]); // Returns 10 because 1 + 2 + 3 + 4 = 10
```

---

## 🚀 Getting Started

### Prerequisites

* Node.js or any JavaScript runtime
* Code editor (e.g., VSCode)

---

## 💻 Usage

### Code:

```js
function sumAll(arr) {
  const [min, max] = [Math.min(...arr), Math.max(...arr)];
  let sum = 0;
  for (let i = min; i <= max; i++) {
    sum += i;
  }
  return sum;
}
```

### Run the function:

```js
console.log(sumAll([1, 4])); // Output: 10
console.log(sumAll([4, 1])); // Output: 10
console.log(sumAll([5, 5])); // Output: 5
console.log(sumAll([10, 7])); // Output: 34
```

---

## 🧪 Test Cases

| Input     | Expected Output |
| --------- | --------------- |
| `[1, 4]`  | `10`            |
| `[4, 1]`  | `10`            |
| `[5, 5]`  | `5`             |
| `[10, 7]` | `34`            |

---

## 📂 Project Structure

```
sum-all-numbers/
├── README.md
└── sumAll.js
```

---

## 📄 License

This project is open source and free to use.

```
