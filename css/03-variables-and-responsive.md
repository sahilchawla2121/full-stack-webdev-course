# 03. CSS Variables, Interactions, & Responsive Design

Mastering dynamic states, design tokens, and media queries to build scalable, modern interfaces.

---

## 🎨 CSS Variables (Custom Properties)
Variables centralize values like color schemes and spacing tokens, making global updates and dark-mode toggling seamless.

```css
:root {
    --primary-color: #4f46e5;
    --bg-color: #ffffff;
    --text-color: #1f2937;
    --spacing-sm: 8px;
    --spacing-md: 16px;
}

/* Dynamic theme switching override */
[data-theme="dark"] {
    --bg-color: #0f172a;
    --text-color: #f8fafc;
}

body {
    background-color: var(--bg-color);
    color: var(--text-color);
    font-family: system-ui, sans-serif;
    padding: var(--spacing-md);
}



🖱️ Pseudo-Classes & Pseudo-Elements
Targeting specific element states or inserting generated content without modifying the HTML structure.

CSS
/* Interactive states */
button {
    background-color: var(--primary-color);
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 6px;
    cursor: pointer;
    transition: background-color 0.2s ease, transform 0.1s ease;
}

button:hover {
    background-color: #4338ca;
    transform: translateY(-2px);
}

button:active {
    transform: translateY(0);
}

/* Structural pseudo-classes */
li:nth-child(even) {
    background-color: #f1f5f9;
}

/* Pseudo-elements for decorative content */
h2::before {
    content: "⚡ ";
}



✨ Transitions & Animations
Adding smooth visual feedback and motion to UI components.

CSS
.card {
    transition: box-shadow 0.3s ease-in-out;
}

.card:hover {
    box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
}

/* Keyframe Animations */
@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(10px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.modal {
    animation: fadeIn 0.4s cubic-bezier(0.16, 1, 0.3, 1) forwards;
}


📱 Media Queries (Responsive Design)
Media queries adjust layout rules dynamically based on device screen dimensions to ensure mobile-friendly designs.

CSS
/* Base mobile layout */
.dashboard {
    display: flex;
    flex-direction: column;
}

.sidebar {
    display: none;
}

/* Tablet and Desktop screens (min-width: 768px) */
@media (min-width: 768px) {
    .dashboard {
        flex-direction: row;
    }
    
    .sidebar {
        display: block;
        width: 250px;
    }
}
