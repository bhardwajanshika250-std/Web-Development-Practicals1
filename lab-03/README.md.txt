# Lab 3: Your First HTML Page

## 1. Practical Aim
To write a first HTML page with a title, headings, and a paragraph, and format some text using standard HTML elements.

## 2. Theoretical Background
- **HTML Structure (`<!DOCTYPE html>`):** Defines the document type and HTML5 standard for web browsers.
- **Headings (`<h1>` to `<h3>`):** Used to define document headings, where `<h1>` is the most important/largest and `<h3>` is a subheading.
- **Paragraphs (`<p>`):** Defines blocks of text content on a webpage.
- **Text Formatting Tags (`<strong>`, `<em>`):** `<strong>` makes text bold and indicates importance, while `<em>` italicizes text for emphasis.
- **Line Break (`<br>`):** Inserts a single line break within text content without starting a new paragraph.

## 3. Pre-requisites & Tools Used
- Visual Studio Code (Code Editor)
- Modern Web Browser (Google Chrome / Edge)
- Windows OS File Explorer

## 4. Step-by-Step Procedure
1. Created `first.html` containing document structure, title `My First Page`, and `<h1>` heading with text `Hello, I am Asha`.
2. Opened `first.html` in a web browser to verify the page title and heading output.
3. Created `headings.html` featuring multiple heading levels (`<h1>`, `<h2>`, `<h3>`) and a descriptive paragraph underneath.
4. Created `text-format.html` including two paragraphs, applying `<strong>` and `<em>` formatting tags, and inserting a `<br>` line break.
5. Captured and saved browser output screenshots for each task into the `lab-3/images/` directory.

## 5. Command Log / Source Code

### Task 1: `first.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Page</title>
</head>
<body>
    <h1>Hello, I am Asha</h1>
</body>
</html>

TASK:02

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Headings and Paragraph</title>
</head>
<body>
    <h1>This is Heading 1 (Largest)</h1>
    <h2>This is Heading 2 (Medium)</h2>
    <h3>This is Heading 3 (Smaller)</h3>
    <p>This is a paragraph placed under the headings to demonstrate standard text styling and layout structure in HTML.</p>
</body>
</html>

TASK:03

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Text Formatting</title>
</head>
<body>
    <p>This is the first paragraph. It contains a <strong>bold</strong> word using the strong tag and an <em>italicized</em> word using the em tag.</p>
    <p>This is the second paragraph.<br>This line starts after a line break using the br tag inside the paragraph.</p>
</body>
</html>
6. Screenshots & Output Evidence
Task 1 Output: ![Task 1 First HTML Page](images/task1.png)

Task 2 Output: ![Task 2 Headings](images/task2.png)

Task 3 Output: ![Task 3 Text Formatting](images/task3.png)

7. Key Learning Outcomes
Understood the fundamental structure and syntax of an HTML5 document.

Learned how to structure text content logically using headings and paragraphs.

Practiced inline text formatting and line breaks using formatting elements.

8. Common Errors & Troubleshooting
File extension error: Ensuring files are saved with .html extension instead of .txt so browsers render them correctly as webpages.

Path errors for images: Ensuring images are correctly placed inside the images/ folder with exact names matching markdown links.

9. Viva / Interview Questions
Q: What is the purpose of the <!DOCTYPE html> declaration?

A: It informs the web browser about the HTML version being used (HTML5) so the page renders correctly in standards mode.

Q: What is the difference between <strong> and <b>?

A: Both make text bold visually, but <strong> carries semantic importance/meaning for screen readers and search engines, whereas <b> is purely stylistic.

10. Submission Checklist
[x] Task 1 (first.html) code & screenshot

[x] Task 2 (headings.html) code & screenshot

[x] Task 3 (text-format.html) code & screenshot

[x] Complete README documentation


---

Ise `lab-3/README.md` mein save karke bataiye, kya aapka Lab 3 bhi poori tarah ready ho gaya? Iske baad hum **Lab 4** shuru karenge!





