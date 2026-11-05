# Lab 11: Units and CSS Variables

## 1. Practical Aim
To apply various CSS units (`px`, `%`, `rem`) and store colors, heading sizes, and spacing tokens using CSS custom properties (`--*` and `var()`).

## 2. Theoretical Background
- **Absolute Units (`px`):** Fixed pixel measurements that do not scale with device layout.
- **Relative Units (`%`, `rem`):** Scalable units where `%` is relative to the parent element and `rem` is relative to the root HTML font size.
- **CSS Variables (Custom Properties):** Defined inside `:root` using double-hyphen prefixes (`--variable-name`) and accessed via the `var()` function to ensure maintainable and reusable code.

## 3. Pre-requisites & Tools Used
- Visual Studio Code
- Modern Web Browser (Chrome/Edge)
- Windows File Explorer

## 4. Step-by-Step Procedure
1. Created `units.html` containing a fixed 200px box, a 50% width responsive box, and a paragraph with `1.5rem` font size.
2. Created `variables.html` defining custom properties (`--main-color`, `--accent-color`, `--page-padding`) inside `:root` and applying them via `var()`.
3. Created `tokens.css` containing design tokens for colors, sizing, and spacing, and linked it to `tokens.html`.
4. Captured and verified browser output screenshots for all tasks and saved them into `lab-11/images/`.

## 5. Command Log / Source Code

### Task 1: `units.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Units</title>
    <style>
        .box-fixed { width: 200px; height: 40px; background-color: lightblue; margin-bottom: 10px; }
        .box-percent { width: 50%; height: 40px; background-color: lightcoral; margin-bottom: 10px; }
        p { font-size: 1.5rem; }
    </style>
</head>
<body>
    <div class="box-fixed">200px Wide Box</div>
    <div class="box-percent">50% Width Box</div>
    <p>This is a larger text paragraph styled using rem units.</p>
</body>
</html>
Task 2: variables.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Variables</title>
    <style>
        :root {
            --main-color: #1d3557;
            --accent-color: #e63946;
            --page-padding: 20px;
        }
        body { color: var(--main-color); padding: var(--page-padding); }
        h1 { color: var(--accent-color); }
    </style>
</head>
<body>
    <h1>Heading Using Accent Colour</h1>
    <p>This body text uses the main colour and page padding defined via CSS variables.</p>
</body>
</html>
Task 3: tokens.css & tokens.html
tokens.css

CSS


:root {
    --primary-color: #1d3557;
    --accent-color: #e63946;
    --heading-size: 2rem;
    --spacing-value: 16px;
}
body { color: var(--primary-color); padding: var(--spacing-value); }
h1 { color: var(--accent-color); font-size: var(--heading-size); }
p { margin-bottom: var(--spacing-value); }
tokens.html

HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Design Tokens</title>
    <link rel="stylesheet" href="tokens.css">
</head>
<body>
    <h1>Styled Heading with Design Tokens</h1>
    <p>This paragraph and the heading are styled using variables linked from tokens.css.</p>
</body>
</html>
6. Screenshots & Output Evidence
Task 1 Output: ![Task 1 Units](images/task1.png)   
Screenshot 2026-11-04 150758.png

Task 2 Output: ![Task 2 Variables](images/task2.png)   
Screenshot 2026-11-04 150758.png

Task 3 Output: ![Task 3 Tokens](images/task3.png)   
Screenshot 2026-11-04 150758.png

7. Key Learning Outcomes
Understood the distinction and practical usage of absolute (px) vs relative (rem, %) CSS units.

Learned how to declare and utilize CSS custom properties (--*) and the var() function for scalable styling.

Implemented external design tokens sheets for centralized design maintenance.

8. Common Errors & Troubleshooting
Scope Errors: Forgetting to declare variables inside :root can lead to fallback rendering behaviors. Ensured global scope declaration.

9. Viva / Interview Questions
Q: What is the difference between rem and em units?

A: rem is relative to the root (<html>) font size, whereas em is relative to the font size of the parent element.

Q: How do you declare a CSS variable globally?

A: By defining it inside the :root pseudo-class selector[cite: 8].

10. Submission Checklist
[x] Task 1 (units.html) code & screenshot[cite: 8]

[x] Task 2 (variables.html) code & screenshot[cite: 8]

[x] Task 3 (tokens.css & tokens.html) code & screenshot[cite: 8]

[x] Complete README documentation

