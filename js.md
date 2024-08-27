# 🟨 JavaScript Code Snippets

This file contains a collection of beautiful and reusable JavaScript code snippets. Each snippet is designed to be easy to understand, implement, and enhance your projects.

---

## 📌 Debouncing a Function

```bash
function debounce(func, delay) {
  let debounceTimer;
  return function() {
    const context = this;
    const args = arguments;
    clearTimeout(debounceTimer);
    debounceTimer = setTimeout(() => func.apply(context, args), delay);
  };
}
```

### Explanation:
This snippet creates a debounce function that delays the execution of the passed function until after a specified delay time has elapsed since the last time it was invoked.

---

## 🌟 Shuffling an Array

```bash
function shuffleArray(array) {
  for (let i = array.length - 1; i > 0; i--) {
    const j = Math.floor(Math.random() * (i + 1));
    [array[i], array[j]] = [array[j], array[i]];
  }
  return array;
}
```

### Explanation:
This snippet shuffles the elements of an array in place using the Fisher-Yates (Knuth) shuffle algorithm.

---

## ✨ Deep Clone an Object

```bash
function deepClone(obj) {
  return JSON.parse(JSON.stringify(obj));
}
```

### Explanation:
This snippet creates a deep clone of a given object using `JSON.parse` and `JSON.stringify`. It works well for objects without functions or special data types.

---

## 📏 Throttling a Function

```bash
function throttle(func, limit) {
  let inThrottle;
  return function() {
    const context = this;
    const args = arguments;
    if (!inThrottle) {
      func.apply(context, args);
      inThrottle = true;
      setTimeout(() => (inThrottle = false), limit);
    }
  };
}
```

### Explanation:
This snippet creates a throttle function that ensures the passed function is called at most once in a specified time frame, regardless of how many times it’s triggered.

---

## 🔗 License

All snippets are licensed under the MIT License.
