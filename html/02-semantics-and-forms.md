# 02. Semantic HTML & Advanced Forms

Moving beyond generic containers enhances accessibility, code maintainability, and SEO rankings.

---

## 🏗️ Semantic Layout Elements
Semantic tags explicitly describe their meaning to both the browser and the developer.

```html
<body>
    <header>
        <h1>Site Logo & Title</h1>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About</a>
        </nav>
    </header>

    <main>
        <article>
            <h2>Understanding Semantics</h2>
            <p>Content inside an article element should be independently distributable.</p>
        </article>
    </main>

    <footer>
        <p>&copy; 2026 Web Dev Course</p>
    </footer>
</body>






📋 Advanced Forms and Validation

HTML5 handles native client-side validation using built-in attributes, reducing manual JavaScript overhead.

HTML
<form action="/submit-data" method="POST">
    <!-- Email validation -->
    <label for="email">Email Address:</label>
    <input type="email" id="email" name="email" required placeholder="user@example.com">

    <!-- Pattern matching validation (alphanumeric only) -->
    <label for="username">Username:</label>
    <input type="text" id="username" name="username" pattern="[A-Za-z0-9]+" title="Letters and numbers only" required>

    <!-- Numeric range limitation -->
    <label for="age">Age (18-100):</label>
    <input type="number" id="age" name="age" min="18" max="100">

    <button type="submit">Submit Registration</button>
</form>
