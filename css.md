# 🎨 CSS Code Snippets

This file contains a collection of beautiful and reusable CSS code snippets. Each snippet is designed to be easy to understand, implement, and enhance your projects.

---

## 📌 Centering an Element

```bash
/* Flexbox centering */
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
```

### Explanation:
This snippet uses Flexbox to center an element both horizontally and vertically within its container.

---

## 🌟 Responsive Grid Layout

```bash
/* Simple responsive grid layout */
.grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 20px;
}
```

### Explanation:
A grid layout that automatically adjusts the number of columns based on the container's width, making it fully responsive.

---

## ✨ Smooth Hover Transition

```bash
/* Smooth transition effect on hover */
.button {
  background-color: #4CAF50;
  color: white;
  padding: 10px 20px;
  text-align: center;
  border: none;
  transition: background-color 0.3s ease;
}

.button:hover {
  background-color: #45a049;
}
```

### Explanation:
A button with a smooth transition effect on hover, changing its background color with a subtle animation.

---

## 📏 Equal Height Columns

```bash
/* Ensuring equal height columns */
.columns {
  display: flex;
}

.column {
  flex: 1;
  padding: 10px;
}
```

### Explanation:
Using Flexbox to create columns that automatically adjust to have equal height, regardless of their content.

---

## 🔗 License

All snippets are licensed under the MIT License.
