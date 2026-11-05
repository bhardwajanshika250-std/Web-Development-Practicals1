# Lab 10: CSS Fundamentals

## 1. Practical Aim
To apply CSS styling in three ways (inline, internal, and linked external stylesheet) and utilize various selectors (`element`, `.class`, `#id`) along with text styling properties.

## 2. Theoretical Background
- **Inline CSS:** Applied directly to an HTML element using the `style` attribute (highest specificity).
- **Internal CSS:** Placed inside a `<style>` block in the document `<head>` section.
- **Linked (External) CSS:** Written in a separate `.stylesheet` file linked via `<link rel="stylesheet" href="...">`.
- **Selectors:** 
  - Element selector (`h1`, `p`) targets HTML tag names.
  - Class selector (`.note`) targets elements with a specific class attribute.
  - ID selector (`#title`) targets a unique element with a specific ID attribute.

## 3. Pre-requisites & Tools Used
- Visual Studio Code
- Modern Web Browser (Chrome/Edge)
- Windows File Explorer

## 4. Step-by-Step Procedure
1. Created `inline-internal.html` containing internal styles for navy headings (`h1`) and yellow background classes (`.highlight`), alongside an inline red-colored paragraph (`style="color: red;"`).
2. Created `style.css` containing rules for `h1` (navy), `.note` (italic), `#title` (underlined), and `p` elements (`font-size: 18px`, grey color).
3. Created `linked.html` linking `style.css` with an `h1` bearing `id="title"` and paragraphs bearing `class="note"`.
4. Captured and verified browser output screenshots for all tasks and saved them into `lab-10/images/`.

## 5. Command Log / Source Code

### Task 1: `inline-internal.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Inline and Internal CSS</title>
    <style>
        h1 { color: navy; }
        .highlight { background-color: yellow; }
    </style>
</head>
<body>
    <h1>This is a Navy Heading</h1>
    <p style="color: red;">This is a red paragraph styled using inline CSS.</p>
    <p class="highlight">This is a paragraph with a yellow background highlighted using internal CSS.</p>
</body>
</html>

Task 2: style.css
CSS


h1 {
    color: navy;
}

.note {
    font-style: italic;
}

#title {
    text-decoration: underline;
}

p {
    font-size: 18px;
    color: grey;
}
Task 3: linked.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Linked CSS Page</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1 id="title">Welcome to CSS Styling</h1>
    <p class="note">This is the first note paragraph styled via external stylesheet.</p>
    <p class="note">This is the second note paragraph displaying font size and grey color.</p>
</body>
</html>
6. Screenshots & Output Evidence
Task 1 Output: ![Task 1 Inline Internal](images/task1.png)   
Screenshot 2026-11-04 150157.png

Task 2 & 3 Output: ![Task 3 Linked CSS](images/task3.png)   
Screenshot 2026-11-04 150157.png

7. Key Learning Outcomes
Understood the hierarchy and implementation methods of inline, internal, and external CSS.

Mastered the use of element, class, and ID selectors to target and style specific DOM elements.

Applied properties such as color, background color, font size, and text decoration.

8. Common Errors & Troubleshooting
Path Errors in External Stylesheets: If style.css is not in the same folder as linked.html, the styles fail to load. Resolved by ensuring both files reside in the same directory[cite: 9].

9. Viva / Interview Questions
Q: What is the order of precedence (specificity) among inline, internal, and external CSS?

A: Inline CSS has the highest priority, followed by internal CSS, and external CSS has the lowest priority (unless overridden by !important).

Q: How do you select an element by its ID in CSS?

A: By using the hash symbol (#) followed by the ID name (e.g., #title).

10. Submission Checklist
[x] Task 1 (inline-internal.html) code & screenshot[cite: 9]

[x] Task 2 (style.css) code[cite: 9]

[x] Task 3 (linked.html) code & screenshot[cite: 9]

[x] Complete README documentation


---






