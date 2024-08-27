# ⚛️ React Code Snippets

This file contains a collection of beautiful and reusable React code snippets. Each snippet is designed to be easy to understand, implement, and enhance your projects.

---

## 📌 Functional Component with State

```bash
import React, { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}

export default Counter;
```

### Explanation:
This snippet demonstrates a simple functional component in React that uses the `useState` hook to manage state. The component renders a counter that increments every time the button is clicked.

---

## 🌟 useEffect Hook Example

```bash
import React, { useState, useEffect } from 'react';

function DataFetcher() {
  const [data, setData] = useState(null);

  useEffect(() => {
    fetch('https://api.example.com/data')
      .then(response => response.json())
      .then(data => setData(data));
  }, []);

  return (
    <div>
      {data ? <p>Data: {JSON.stringify(data)}</p> : <p>Loading...</p>}
    </div>
  );
}

export default DataFetcher;
```

### Explanation:
This snippet shows how to use the `useEffect` hook to fetch data from an API when the component mounts. It demonstrates the power of `useEffect` for handling side effects in React.

---

## ✨ Conditional Rendering

```bash
import React from 'react';

function Greeting({ isLoggedIn }) {
  return (
    <div>
      {isLoggedIn ? <h1>Welcome back!</h1> : <h1>Please sign in.</h1>}
    </div>
  );
}

export default Greeting;
```

### Explanation:
This snippet illustrates conditional rendering in React, where the component displays different content based on the `isLoggedIn` prop.

---

## 📏 Mapping Over an Array of Items

```bash
import React from 'react';

function ItemList({ items }) {
  return (
    <ul>
      {items.map(item => (
        <li key={item.id}>{item.name}</li>
      ))}
    </ul>
  );
}

export default ItemList;
```

### Explanation:
This snippet demonstrates how to render a list of items by mapping over an array and returning a list item for each element. The `key` prop is important for helping React identify which items have changed.

---

## 🎨 Styling with Inline Styles

```bash
import React from 'react';

function StyledButton() {
  return (
    <button style={{ backgroundColor: 'blue', color: 'white', padding: '10px 20px', borderRadius: '5px' }}>
      Styled Button
    </button>
  );
}

export default StyledButton;
```

### Explanation:
This snippet shows how to apply inline styles directly to a React component. Inline styles are useful for applying unique styles that aren't repeated elsewhere.

---

## 🔗 License

All snippets are licensed under the MIT License.
