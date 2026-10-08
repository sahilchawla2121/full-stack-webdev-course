# 01. HTML Basics & Structure

HTML (HyperText Markup Language) is the standard markup language for documents designed to be displayed in a web browser. It forms the skeletal structure of all web pages.

---

## 📄 The HTML Boilerplate
Every valid HTML document requires a specific foundational structure to render correctly across modern browsers.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document Title</title>
</head>
<body>
    <h1>Hello World</h1>
</body>
</html>
<!DOCTYPE html>: Declares the document type and HTML5 standard.

<html lang="en">: The root element wrapping all content; specifies the language for screen readers and search engines.

<meta charset="UTF-8">: Ensures proper character encoding (supports universal text and symbols).




📝 Text Content & Headings
Headings dictate hierarchy (<h1> to <h6>), while paragraph tags (<p>) structure standard text blocks.

HTML
<h1>Main Page Title (H1)</h1>
<h2>Section Subheading (H2)</h2>
<p>This is a standard text block used to convey core content and explanations on a web page.</p>



🔗 Links and Media



Connecting pages or embedding visual assets requires targeted attributes.

HTML
<!-- Hyperlink to external resources -->
<a href="[https://github.com](https://github.com)" target="_blank" rel="noopener noreferrer">Visit GitHub</a>

<!-- Embedded Image asset -->
<img src="avatar.jpg" alt="Profile avatar description" width="300">




📑 Lists (Ordered & Unordered)
Lists organize sequential procedures or navigation options.

HTML
<!-- Unordered Bulleted List -->
<ul>
    <li>HTML5 Structure</li>
    <li>CSS Layouts</li>
    <li>JavaScript Logic</li>
</ul>

<!-- Ordered Numbered List -->
<ol>
    <li>Step One: Clone repository</li>
    <li>Step Two: Install dependencies</li>
    <li>Step Three: Run local server</li>
</ol


