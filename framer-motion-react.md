# 🎥 Framer Motion in React Code Snippets

This file contains a collection of beautiful and reusable Framer Motion code snippets for React. Each snippet is designed to be easy to understand, implement, and enhance your projects.

---

## 📌 Basic Motion Component

```bash
import { motion } from 'framer-motion';

function BasicMotion() {
  return (
    <motion.div
      animate={{ x: 100 }}
      transition={{ duration: 0.5 }}
      style={{ width: 100, height: 100, backgroundColor: 'blue' }}
    />
  );
}

export default BasicMotion;
```

### Explanation:
This snippet demonstrates a basic `motion.div` component that moves 100 pixels along the x-axis over 0.5 seconds. Framer Motion makes it easy to animate React components with a declarative syntax.

---

## 🌟 Hover and Tap Animations

```bash
import { motion } from 'framer-motion';

function HoverTapButton() {
  return (
    <motion.button
      whileHover={{ scale: 1.2 }}
      whileTap={{ scale: 0.8 }}
      style={{ padding: '10px 20px', fontSize: '16px' }}
    >
      Press Me
    </motion.button>
  );
}

export default HoverTapButton;
```

### Explanation:
This snippet shows how to use Framer Motion to create a button that scales up when hovered and scales down when tapped or clicked.

---

## ✨ Staggered List Animation

```bash
import { motion } from 'framer-motion';

const container = {
  hidden: { opacity: 0 },
  show: {
    opacity: 1,
    transition: {
      staggerChildren: 0.2,
    },
  },
};

const item = {
  hidden: { opacity: 0, y: -20 },
  show: { opacity: 1, y: 0 },
};

function StaggeredList() {
  return (
    <motion.ul variants={container} initial="hidden" animate="show">
      <motion.li variants={item}>Item 1</motion.li>
      <motion.li variants={item}>Item 2</motion.li>
      <motion.li variants={item}>Item 3</motion.li>
    </motion.ul>
  );
}

export default StaggeredList;
```

### Explanation:
This snippet demonstrates how to create staggered animations for a list of items using Framer Motion. Each list item fades in and moves up with a slight delay between each item.

---

## 📏 Animate Presence for Conditional Rendering

```bash
import { motion, AnimatePresence } from 'framer-motion';
import { useState } from 'react';

function ToggleComponent() {
  const [isVisible, setIsVisible] = useState(true);

  return (
    <>
      <button onClick={() => setIsVisible(!isVisible)}>Toggle</button>
      <AnimatePresence>
        {isVisible && (
          <motion.div
            initial={{ opacity: 0 }}
            animate={{ opacity: 1 }}
            exit={{ opacity: 0 }}
            style={{ width: 100, height: 100, backgroundColor: 'red' }}
          />
        )}
      </AnimatePresence>
    </>
  );
}

export default ToggleComponent;
```

### Explanation:
This snippet shows how to use `AnimatePresence` to animate components that are conditionally rendered. The `motion.div` will fade in when it appears and fade out when it exits.

---

## 🎨 Drag and Drop

```bash
import { motion } from 'framer-motion';

function DraggableBox() {
  return (
    <motion.div
      drag
      dragConstraints={{ left: -100, right: 100, top: -100, bottom: 100 }}
      style={{ width: 100, height: 100, backgroundColor: 'green', borderRadius: '10px' }}
    />
  );
}

export default DraggableBox;
```

### Explanation:
This snippet demonstrates how to create a draggable component using Framer Motion. The box can be dragged within a defined area, constrained by the specified boundaries.

---

## 🔗 License

All snippets are licensed under the MIT License.
