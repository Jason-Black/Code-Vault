# 🌀 GSAP Code Snippets

This file contains a collection of beautiful and reusable GSAP code snippets. Each snippet is designed to be easy to understand, implement, and enhance your projects.

---

## 📌 Basic Tween Animation

```bash
import { gsap } from 'gsap';

gsap.to('.box', { duration: 2, x: 300 });
```

### Explanation:
This snippet demonstrates a basic tween animation using GSAP. The `.box` element will move 300 pixels along the x-axis over 2 seconds.

---

## 🌟 Staggered Animations

```bash
import { gsap } from 'gsap';

gsap.from('.staggered-item', { duration: 1, opacity: 0, y: -50, stagger: 0.2 });
```

### Explanation:
This snippet shows how to create staggered animations where each `.staggered-item` element fades in and moves up with a slight delay between each item.

---

## ✨ ScrollTrigger Animation

```bash
import { gsap } from 'gsap';
import { ScrollTrigger } from 'gsap/ScrollTrigger';

gsap.registerPlugin(ScrollTrigger);

gsap.to('.scroll-box', {
  scrollTrigger: {
    trigger: '.scroll-box',
    start: 'top 80%',
    end: 'top 20%',
    scrub: true,
  },
  x: 500,
  rotation: 360,
});
```

### Explanation:
This snippet uses GSAP's `ScrollTrigger` plugin to animate the `.scroll-box` element as it enters the viewport. The element will move 500 pixels along the x-axis and rotate 360 degrees as the user scrolls.

---

## 📏 Timeline Animation Sequence

```bash
import { gsap } from 'gsap';

const tl = gsap.timeline({ repeat: -1, yoyo: true });

tl.to('.box', { duration: 1, x: 100 })
  .to('.box', { duration: 1, y: 100 })
  .to('.box', { duration: 1, x: 0 })
  .to('.box', { duration: 1, y: 0 });
```

### Explanation:
This snippet demonstrates how to create a timeline animation sequence using GSAP. The `.box` element moves to different positions in a sequence, and the animation repeats infinitely with a yoyo effect.

---

## 🎨 Morphing SVG Paths

```bash
import { gsap } from 'gsap';
import { MorphSVGPlugin } from 'gsap/MorphSVGPlugin';

gsap.registerPlugin(MorphSVGPlugin);

gsap.to('#circle', { duration: 2, morphSVG: '#star' });
```

### Explanation:
This snippet shows how to use the `MorphSVGPlugin` to morph an SVG element with the ID `#circle` into another shape with the ID `#star` over 2 seconds.

---

## 🔗 License

All snippets are licensed under the MIT License.
