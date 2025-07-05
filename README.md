# Responsive Flexbox Layout with Shrink, Wrap & Alignment in CSS

This is a beginner-friendly HTML and CSS project that demonstrates how to use **Flexbox** to build a simple, responsive layout. It covers the use of key Flexbox properties like `flex-wrap`, `flex-shrink`, `min-width`, and alignment tools like `justify-content` and `align-items`.

## 🌟 Features

- ✅ Uses `display: flex` to create a flexible layout
- 📐 `gap` property to add spacing between boxes
- ↔️ `flex-shrink` to allow boxes to shrink based on screen size
- 🔒 `min-width` to limit how small boxes can get
- 🎯 `justify-content` and `align-items` for horizontal and vertical alignment
- 📱 Media queries for responsive design on smaller screens
- 🔁 `flex-wrap` allows boxes to wrap to a new line if needed

## 🖥️ Demo Layout Preview

When you open the `index.html` in a browser, you'll see a row of colored boxes that stay aligned and responsive across different screen sizes.


## 📜 How It Works

- The `body` is styled with `display: flex` to arrange `.box` items in a row.
- A `gap` is added to space the boxes.
- The `.box` elements have `flex-shrink`, `min-width`, and fixed height/width.
- A media query (`max-width: 575px`) activates `flex-wrap` to wrap boxes on small screens.

## 💡 Example CSS Snippet

```css
body {
  display: flex;
  gap: 10px;
}

.box {
  flex-shrink: 1;
  min-width: 100px;
  height: 100px;
  width: 100px;
  background-color: blueviolet;
  display: flex;
  justify-content: center;
  align-items: center;
}

@media (max-width: 575px) {
  body {
    flex-wrap: wrap;
  }
}

