# Lab 5: Links and Images

## 1. Practical Aim
To link two HTML pages together using anchor tags and embed an image with custom width, height, and alternative text.

## 2. Theoretical Background
- **Anchor Tag (`<a>`):** Used to create hyperlinks between web pages using the `href` attribute.
- **Image Tag (`<img>`):** Used to embed images into a webpage. It is a self-closing tag.
- **Source Attribute (`src`):** Specifies the path or URL of the image file.
- **Alternative Text (`alt`):** Provides text description for an image if it fails to load or for screen readers.
- **Dimensions (`width` and `height`):** Attributes used to set the display size of images in pixels.

## 3. Pre-requisites & Tools Used
- Visual Studio Code
- Modern Web Browser (Chrome/Edge)
- Windows File Explorer

## 4. Step-by-Step Procedure
1. Created `home.html` with heading `Welcome to My Site` and a paragraph linking to `portfolio.html` using anchor text `portfolio`.
2. Created `portfolio.html` with a heading, descriptive text, and a back-link pointing to `home.html`.
3. Created `portfolio-image.html` featuring a heading and an image tag pointing to a local image with dimensions set to 200x200 and a descriptive `alt` attribute.
4. Verified link navigation between pages and image rendering in the browser.
5. Captured and saved browser screenshots inside `lab-5/images/`.

## 5. Command Log / Source Code

### Task 1: `home.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home Page</title>
</head>
<body>
    <h1>Welcome to My Site</h1>
    <p>Check out my <a href="portfolio.html">portfolio</a> page.</p>
</body>
</html>
 
####Task 2: portfolio.html
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio Page</title>
</head>
<body>
    <h1>My Portfolio</h1>
    <p>This is my portfolio page showcasing my projects and works.</p>
    <p><a href="home.html">Back to Home Page</a></p>
</body>
</html>
 
###Task 3: portfolio-image.html



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio Image</title>
</head>
<body>
    <h1>Portfolio Gallery</h1>
    <img src="images/sample.jpg" width="200" height="200" alt="A preview photo of portfolio work">
</body>
</html>
6. Screenshots & Output Evidence
Task 1 Output: ![Task 1 Home Page](images/task1.png)

Task 2 Output: ![Task 2 Portfolio Page](images/task2.png)

Task 3 Output: ![Task 3 Portfolio Image](images/task3.png)

7. Key Learning Outcomes
Learned how to navigate across multiple local HTML files using hyperlinks.

Understood how to embed images and control their display size using HTML attributes.

Recognized the importance of alt text for web accessibility and error fallback.

8. Common Errors & Troubleshooting
Broken Image Links: Incorrect file paths in the src attribute cause images not to render. Fixed by verifying relative paths pointing inside the images/ directory.

Broken Relative Links: Misspelled filenames in href result in 404/file not found errors when clicking links. Checked exact filenames.

9. Viva / Interview Questions
Q: What attribute is mandatory inside the <img> tag for accessibility?

A: The alt attribute, which describes the image for screen readers and displays text if the image fails to load.

Q: How do you link to another local HTML page in the same folder?

A: By using the anchor tag with the href attribute set to the target filename, e.g., <a href="portfolio.html">portfolio</a>.

10. Submission Checklist
[x] Task 1 (home.html) code & screenshot

[x] Task 2 (portfolio.html) code & screenshot

[x] Task 3 (portfolio-image.html) code & screenshot

[x] Complete README documentation


---








