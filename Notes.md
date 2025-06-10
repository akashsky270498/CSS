```
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

✅ **Example:**
```html
<p style="color: red;">This is red text.</p>
```

---

### 2. 🟦 Internal CSS
- CSS is written **inside a `<style>` tag** within the `<head>` section of the HTML document.
- Useful when styling a single HTML page.

✅ **Example:**
```html
<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>
```

---

### 3. 🟩 External CSS
- CSS rules are placed in a **separate `.css` file**.
- Linked to the HTML using a `<link>` tag in the `<head>`.

✅ **Example:**
```html
<link rel="stylesheet" href="styles.css">
```

---

## 📦 `box-sizing: border-box`

- When `box-sizing: border-box` is applied:
  - The declared `width` and `height` **include** the content, **padding**, and **border**.
  - **Margin is not included** in this calculation.

✅ **Example:**
```css
box-sizing: border-box;
height: 400px;
```

💡 This means the element's total height will be **400px maximum**, regardless of padding or border. The browser adjusts the content area to ensure everything fits within that height.

---

## 📏 Margin Collapse

- When two vertical margins meet between block-level elements, **they don’t add up**.
- Instead, they **collapse**, and only the **larger** margin is used.

✅ **Example:**

- First element: `margin-bottom: 30px`
- Second element: `margin-top: 25px`
- Resulting space between the elements: **30px**, not 55px.

💡 This is called **margin collapsing**, and it's part of the standard behavior in CSS layout flow.

---



## 🔠 Font and Text Styling

- `font-family`: Specifies the typeface (e.g., Poppins, Verdana) for an element's text.
- `font-size`: Sets the size of the text.
- `font-weight`: Sets the boldness or thickness of the font.
- `font-style`: Defines the style of the font like `italic`, `normal`, etc.
- `font-optical-sizing`: Adjusts font rendering automatically for optical size (used with variable fonts).
- `text-decoration`: Adds decoration like underline, line-through, or overline to text.
- `text-decoration-color`: Sets the color of the text-decoration (like underline).
- `text-decoration-style`: Sets the style of the decoration (e.g., solid, dotted).
- `text-decoration-thickness`: Controls the thickness of the text decoration.
- `text-transform`: Controls capitalization of text (e.g., uppercase, lowercase, capitalize).
- `text-align`: Aligns the text horizontally (e.g., center, left, right).
- `line-height`: Sets the vertical space between lines of text.
- `letter-spacing`: Sets the spacing between characters (tracking).

---

## 🎨 Color & Background

- `color`: Sets the color of the text.
- `background-color`: Sets the background color of an element.

---

## 📏 Box Model Properties

- `border`: Sets the border around an element (width, style, and color).
- `width`: Sets the width of an element.

---

## 📦 Overflow and Text Overflow

- `overflow`: Controls what happens when content overflows the element box (e.g., hidden, scroll).
- `text-overflow`: Determines how overflowed text is signaled (e.g., ellipsis `...`).

---

## 🧱 Word and Text Break

- `word-break`: Specifies how to break words when they overflow (e.g., `break-all` breaks words anywhere).



```


inline style > id selector > class or attribute selector > Elelment selector > universal selector
