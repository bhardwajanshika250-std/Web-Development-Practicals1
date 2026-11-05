# Lab 7: About Me Page

## 1. Practical Aim
To build a concise "About Me" webpage utilizing semantic HTML tags, internal page jump links, and an email contact link.

## 2. Theoretical Background
- **Semantic Tags (`<header>`, `<main>`, `<section>`, `<footer>`):** Provide meaningful structural meaning to the browser and developers regarding document sections.
- **Internal Anchors (`href="#id"`):** Enable smooth page jumping to specific sections identified by unique `id` attributes.
- **Mailto Links (`href="mailto:..."`):** Opens the user's default mail client to send an email directly to the specified address.

## 3. Pre-requisites & Tools Used
- Visual Studio Code
- Modern Web Browser (Chrome/Edge)
- Windows File Explorer

## 4. Step-by-Step Procedure
1. Created `about-me.html` with a `<header>` containing an `h1` with name and a `<nav>` linking to `#about` and `#contact`.
2. Added a `<main>` element containing a `<section>` with `id="about"`, an `h2` heading (`About me`), and a descriptive paragraph[cite: 6].
3. Added a `<footer>` with `id="contact"` containing a paragraph with a clickable `mailto:` email link[cite: 6].
4. Captured and verified browser output and jump link behavior, saving screenshots in `lab-7/images/`.

## 5. Command Log / Source Code

### Source Code: `about-me.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Me</title>
</head>
<body>
    <header>
        <h1>Madhav</h1>
        <nav>
            <a href="#about">About</a> | 
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <main>
        <section id="about">
            <h2>About me</h2>
            <p>Hello! I am a computer science student passionate about software development, coding, and building structured web applications.</p>
        </section>
    </main>

    <footer id="contact">
        <p>Get in touch via email: <a href="mailto:madhav@example.com">madhav@example.com</a></p>
    </footer>
</body>
</html>

6. Screenshots & Output Evidence
Webpage Output: ![About Me Page Output](images/task1.png)[cite: 6]

7. Key Learning Outcomes
Understood the practical implementation of semantic layout elements in HTML5.

Learned how to configure internal jump links using id attributes and href="#".

Implemented mailto: links for quick communication channels.

8. Common Errors & Troubleshooting
Broken Jump Links: Mismatch between the anchor href="#about" and the target element's id="about" prevents smooth navigation. Verified correct matching of IDs.

9. Viva / Interview Questions
Q: What is the benefit of using semantic tags like <header> and <footer> instead of generic <div> tags?

A: Semantic tags clearly describe their meaning to both the browser and the developer, improving accessibility and code readability.

Q: How do you create an internal link that jumps to a specific section on the same page?

A: By setting the anchor href attribute to the target element's ID prefixed with a hash symbol (e.g., href="#about").

10. Submission Checklist
[x] about-me.html created with semantic tags, internal nav, and mailto link[cite: 6]

[x] Browser screenshot captured and saved[cite: 6]

[x] Complete README documentation









