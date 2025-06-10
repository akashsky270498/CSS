```
# CSS Basics and Concepts

## Selectors

- HTML elements are called **selectors**.
- **Selectors** are used to target elements to which we want to apply CSS styles.

## Types of CSS

### 1. Inline CSS
- Inline CSS is used directly within an HTML element using the `style` attribute.

Example:
<p style="color: red;">This is red text.</p>

### 2. Internal CSS
- Internal CSS means using a `<style>` tag within the `<head>` section of the HTML page to define styles.

Example:
<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>

### 3. External CSS
- External CSS involves creating a separate `.css` file and writing all your CSS code inside it. This file is then linked to your HTML file using the `<link>` tag.

Example:
<link rel="stylesheet" href="styles.css">

---

## box-sizing: border-box

- When `box-sizing: border-box` is applied, the specified `width` and `height` of the element include the **content**, **padding**, and **border**, but **not the margin**.

Example:
box-sizing: border-box;
height: 400px;

- This means the total height of the element will **not exceed 400px**, even if padding and border are added.
- The browser adjusts the content area accordingly to make everything fit within the declared height.

---

## Margin Collapse

- When vertical margins of two adjacent block elements meet, they can **collapse into a single margin**, rather than adding together.

Example:

If one box has:
margin-bottom: 30px

And the next box has:
margin-top: 25px

→ The resulting vertical space between the two boxes will be **30px**, not 55px.  
Only the **larger margin value** is applied.
```
