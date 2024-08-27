# 🌬️ TailwindCSS Code Snippets

This file contains a collection of beautiful and reusable TailwindCSS code snippets. Each snippet is designed to be easy to understand, implement, and enhance your projects.

---

## 📌 Responsive Flexbox Centering

```bash
<div class="flex items-center justify-center h-screen">
  <!-- Content goes here -->
</div>
```

### Explanation:
This snippet centers content both vertically and horizontally within a full-screen height container using TailwindCSS's flexbox utilities.

---

## 🌟 Responsive Grid Layout

```bash
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
  <!-- Grid items go here -->
</div>
```

### Explanation:
A responsive grid layout that adjusts the number of columns based on the screen size, using TailwindCSS's grid and responsive utilities.

---

## ✨ Hover Transition Effect

```bash
<button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded transition duration-300 ease-in-out">
  Hover me
</button>
```

### Explanation:
A button with a smooth hover transition effect, changing the background color on hover with a 300ms duration using TailwindCSS's utility classes.

---

## 📏 Full-Width Button

```bash
<button class="w-full bg-green-500 text-white font-bold py-2 px-4 rounded">
  Full-Width Button
</button>
```

### Explanation:
A full-width button that spans the entire width of its container, styled using TailwindCSS utilities.

---

## 🎨 Responsive Center Card w/Drop shadow

```bash
div class="relative flex min-h-screen flex-col justify-center overflow-hidden bg-gray-50 py-6 sm:py-12">
  <img src="/img/beams.jpg" alt="" class="absolute top-1/2 left-1/2 max-w-none -translate-x-1/2 -translate-y-1/2" width="1308" />
  <div class="absolute inset-0 bg-[url(/img/grid.svg)] bg-center [mask-image:linear-gradient(180deg,white,rgba(255,255,255,0))]"></div>
  <div class="relative bg-white px-6 pt-10 pb-8 shadow-xl ring-1 ring-gray-900/5 sm:mx-auto sm:max-w-lg sm:rounded-lg sm:px-10">
    <div class="mx-auto max-w-md">
      <img src="/img/logo.svg" class="h-6" alt="Tailwind Play" />
      <div class="divide-y divide-gray-300/50">
        <div class="space-y-6 py-8 text-base leading-7 text-gray-600">
          <p>An advanced online playground for Tailwind CSS, including support for things like:</p>
          <ul class="space-y-4">
            <li class="flex items-center">
              <svg class="h-6 w-6 flex-none fill-sky-100 stroke-sky-500 stroke-2" stroke-linecap="round" stroke-linejoin="round">
                <circle cx="12" cy="12" r="11" />
                <path d="m8 13 2.165 2.165a1 1 0 0 0 1.521-.126L16 9" fill="none" />
              </svg>
              <p class="ml-4">
                Customizing your
                <code class="text-sm font-bold text-gray-900">tailwind.config.js</code> file
              </p>
            </li>
            <li class="flex items-center">
              <svg class="h-6 w-6 flex-none fill-sky-100 stroke-sky-500 stroke-2" stroke-linecap="round" stroke-linejoin="round">
                <circle cx="12" cy="12" r="11" />
                <path d="m8 13 2.165 2.165a1 1 0 0 0 1.521-.126L16 9" fill="none" />
              </svg>
              <p class="ml-4">
                Extracting classes with
                <code class="text-sm font-bold text-gray-900">@apply</code>
              </p>
            </li>
            <li class="flex items-center">
              <svg class="h-6 w-6 flex-none fill-sky-100 stroke-sky-500 stroke-2" stroke-linecap="round" stroke-linejoin="round">
                <circle cx="12" cy="12" r="11" />
                <path d="m8 13 2.165 2.165a1 1 0 0 0 1.521-.126L16 9" fill="none" />
              </svg>
              <p class="ml-4">Code completion with instant preview</p>
            </li>
          </ul>
          <p>Perfect for learning how the framework works, prototyping a new idea, or creating a demo to share online.</p>
        </div>
        <div class="pt-8 text-base font-semibold leading-7">
          <p class="text-gray-900">Want to dig deeper into Tailwind?</p>
          <p>
            <a href="https://tailwindcss.com/docs" class="text-sky-500 hover:text-sky-600">Read the docs &rarr;</a>
          </p>
        </div>
      </div>
    </div>
  </div>
</div>


```

### Explanation:
A custom card component with an image, title, and description, styled using TailwindCSS.


## 🎨 Custom Card Component

```bash
<div class="max-w-sm rounded overflow-hidden shadow-lg">
  <img class="w-full" src="path-to-image.jpg" alt="Image">
  <div class="px-6 py-4">
    <div class="font-bold text-xl mb-2">Card Title</div>
    <p class="text-gray-700 text-base">
      Description goes here.
    </p>
  </div>
</div>
```

### Explanation:
A custom card component with an image, title, and description, styled using TailwindCSS.

---

## 🔗 License

All snippets are licensed under the MIT License.
