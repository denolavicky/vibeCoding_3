# Pricing Card Component: Debugging & Refactoring Task

## 🛠 Assignment Overview
This project involved taking a "broken" HTML/CSS snippet of a pricing card and transforming it into a functional, reusable, and professionally styled web component using AI-assisted development (Cursor).

---

## 1. Before Code (Original Broken Snippet)
The initial code contained several critical issues:
* **HTML Syntax:** The `<h2>` tag for the title was incorrectly closed with another `<h2>` instead of `</h2>`.
* **CSS Syntax:** The `box-shadow` property was misspelled as `box-shdow`, causing the depth effect to fail.
* **Responsiveness:** The layout used fixed widths and lacked modern alignment techniques.
* **Architecture:** The data was hardcoded, making it impossible to scale without repeating code.

```html
<!DOCTYPE html>
<html>
<head>
<style>
.pricing {
width: 300px;
margin: auto;
background-color: #fff;
box-shdow: 0 0 10px #ccc; /* Typo here */
padding: 10px;
text-align: left;
}
/* ... rest of original snippet ... */
</style>
</head>
<body>
<div class="pricing">
<h2 class="title">Basic Plan<h2> <p class="price">$9.99 /month</p>
</div>
</body>
</html>