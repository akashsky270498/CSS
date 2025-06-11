# 🌐 CSS Basics and Concepts

---

## 🔸 What Are Selectors?

- HTML elements are known as **selectors** in CSS.
- Selectors are used to **target HTML elements** and apply styling rules to them.

---

## 🎨 Types of CSS

### 1. 🟨 Inline CSS
- Applied **directly inside an HTML tag** using the `style` attribute.
- Used for quick or one-off styling.

✅ Example:
<p style="color: red;">This is red text.</p>

---

### 2. 🟦 Internal CSS
- CSS is written **inside a `<style>` tag** within the `<head>` section of the HTML document.
- Useful when styling a single HTML page.

✅ Example:
<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>

---

### 3. 🟩 External CSS
- CSS rules are placed in a **separate `.css` file**.
- Linked to the HTML using a `<link>` tag in the `<head>`.

✅ Example:
<link rel="stylesheet" href="styles.css">

---

## 📦 box-sizing: border-box

- When `box-sizing: border-box` is applied:
  - The declared `width` and `height` **include** content, **padding**, and **border**.
  - Margin is **not included**.

✅ Example:
box-sizing: border-box;
height: 400px;

💡 The total element height will remain 400px, even with padding and borders inside it.

---

## 📏 Margin Collapse

- When two vertical margins meet, they **don’t add up**.
- Instead, they **collapse** and only the **larger value** is applied.

✅ Example:
- First element: `margin-bottom: 30px`
- Second element: `margin-top: 25px`
- Final space between them = 30px (not 55px).

💡 This is called **margin collapsing**.

---

## 🔠 Font and Text Styling

- `font-family`: Sets the typeface (e.g., Poppins, Arial).
- `font-size`: Controls text size.
- `font-weight`: Sets thickness (e.g., bold).
- `font-style`: Normal, italic, etc.
- `font-optical-sizing`: Adjusts font rendering for optical size.
- `text-decoration`: Underline, line-through, etc.
- `text-decoration-color`: Color of decoration (e.g., underline).
- `text-decoration-style`: Style of decoration (solid, dashed).
- `text-decoration-thickness`: Thickness of underline/line.
- `text-transform`: Capitalize, uppercase, lowercase.
- `text-align`: Aligns text left, center, right.
- `line-height`: Sets space between lines.
- `letter-spacing`: Controls spacing between characters.

---

## 🎨 Color & Background

- `color`: Text color.
- `background-color`: Background color of an element.

---

## 📏 Box Model Properties

- `border`: Width, style, and color of the element’s border.
- `width`: Width of the element.

---

## 📦 Overflow and Text Overflow

- `overflow`: What to do if content overflows box (e.g., scroll, hidden).
- `text-overflow`: How to handle text overflow (e.g., ellipsis `...`).

---

## 🧱 Word and Text Break

- `word-break`: Controls how long words break across lines.
  - `normal`: Breaks at allowed break points.
  - `break-word` / `break-all`: Breaks anywhere to prevent overflow.

---

## 🔁 CSS Specificity Hierarchy (Most to Least Powerful)

1. ✅ Inline styles:  
   `<p style="color: red;">` → Highest priority

2. ✅ ID selectors:  
   `#myId { color: green; }`

3. ✅ Class, attribute, and pseudo-class selectors:  
   `.myClass`, `[type="text"]`, `:hover`

4. ✅ Element selectors:  
   `p`, `div`, `h1`

5. ✅ Universal selector:  
   `* {}` → Least specific

💡 When multiple rules apply, **more specific selectors win**. If specificity is equal, the one defined last overrides.

---

## ✅ Quick Summary of CSS Units

- `px`: Fixed size.
- `vw`: 1% of viewport width.
- `vh`: 1% of viewport height.
- `em`: Relative to parent font size.
- `rem`: Relative to root (`html`) font size.
- `vmin`: 1% of the smaller of width or height.
- `vmax`: 1% of the larger of width or height.
- `min-height`: Minimum allowed height (can grow, but not shrink).
- `width: 50%`: Sets width to 50% of the parent element.
- `margin: auto`: Horizontally centers block elements.

---

✨ That’s your CSS basics cheat sheet — clear, complete, and copy-paste ready.


📏 CSS Units & Concepts (Simplified)

-----------------------------------------
🧱 px – Pixels
-----------------------------------------
- Fixed unit of measurement.
- 1px = 1/96 of an inch.
- Not responsive. Large values can cause scrollbars (overflow).

-----------------------------------------
🖥️ vw – Viewport Width
-----------------------------------------
- 1vw = 1% of the browser window’s width.
- 100vw = full width of the screen.
- Good for responsive layouts.

-----------------------------------------
📏 vh – Viewport Height
-----------------------------------------
- 1vh = 1% of the browser window’s height.
- 100vh = full height of the screen.
- Useful for fullscreen sections, banners, etc.

-----------------------------------------
🎯 margin: auto
-----------------------------------------
- Horizontally centers block-level elements.
- Doesn’t work with inline elements.

-----------------------------------------
🔡 em – Relative to Parent Font Size
-----------------------------------------
- 1em = font size of the parent element.
- Example: If parent = 18px, then 1.5em = 27px.
- Inherits and multiplies based on the parent.

-----------------------------------------
🧱 rem – Relative to Root Font Size
-----------------------------------------
- 1rem = font size of the root `<html>` element.
- By default, 1rem = 16px.
- More consistent than em, as it doesn’t depend on the parent.

-----------------------------------------
🔁 vmin – 1% of Smaller Viewport Dimension
-----------------------------------------
- Takes the smaller of width or height.
- Example: screen = 1200px x 800px → 1vmin = 8px.

-----------------------------------------
🔁 vmax – 1% of Larger Viewport Dimension
-----------------------------------------
- Takes the larger of width or height.
- Example: screen = 1200px x 800px → 1vmax = 12px.

-----------------------------------------
📐 min-height
-----------------------------------------
- Sets the minimum height of an element.
- Element can grow taller if needed.
- Cannot shrink below the defined min-height.
- Good for flexible/responsive layouts.

-----------------------------------------
📏 width: 50%
-----------------------------------------
- Width is 50% of the parent element's width.
