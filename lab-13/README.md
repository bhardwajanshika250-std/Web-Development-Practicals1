# Lab 13: Flexbox Layouts

## 1. Practical Aim
To design and implement a horizontal navigation bar, centered card layouts, and wrapping card containers using CSS Flexbox.

## 2. Theoretical Background
- **Flexbox Layout (`display: flex`):** A one-dimensional layout model designed for arranging items in rows or columns with sophisticated alignment and space distribution control.
- **Main Axis Alignment (`justify-content`):** Controls alignment along the main axis (e.g., `center`, `space-between`).
- **Cross Axis Alignment (`align-items`):** Controls alignment along the cross axis (e.g., `center`, `flex-start`).
- **Flex Wrapping (`flex-wrap: wrap`):** Allows flex items to wrap onto multiple rows when container width becomes constrained.

## 3. Pre-requisites & Tools Used
- Visual Studio Code
- Modern Web Browser (Chrome/Edge)
- Windows File Explorer

## 4. Step-by-Step Procedure
1. Created `nav-flex.html` featuring a dark-themed horizontal navigation bar (`<nav>`) with four white links side by side using `display: flex`.
2. Created `centred-cards.html` containing a row div holding three cards (Starter, Standard, Premium) centered horizontally and vertically using `justify-content` and `align-items`.
3. Created `wrapping-cards.html` under the heading "Stationery Shop" featuring four items (Notebook, Pen, Bag, Book) inside a `flex-wrap` container that adapts and wraps on narrower browser windows.
4. Captured and verified browser output screenshots for all tasks and saved them into `lab-13/images/`.

## 5. Command Log / Source Code

### Task 1: `nav-flex.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Navigation Bar</title>
    <style>
        body { margin: 0; font-family: Arial, sans-serif; }
        .navbar { display: flex; background-color: #333; padding: 14px 20px; gap: 20px; }
        .navbar a { color: white; text-decoration: none; font-size: 16px; }
    </style>
</head>
<body>
    <nav class="navbar">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
    </nav>
</body>
</html>