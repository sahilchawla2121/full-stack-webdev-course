# 01. CSS Selectors & The Box Model

CSS (Cascading Style Sheets) governs the visual styling, layout, and responsiveness of HTML elements.

---

## 🎯 Selectors
Selectors target specific HTML elements to apply styling properties.

```css
/* Element Selector */
p {
    font-size: 16px;
    color: #333333;
}

/* Class Selector */
.card-container {
    background-color: #ffffff;
    border-radius: 8px;
}

/* ID Selector (Unique identifier) */
#main-header {
    background-color: #1e293b;
}


📦 The CSS Box ModelEvery element rendered on a web page is treated as a rectangular box consisting of four layers: Content $\rightarrow$ Padding $\rightarrow$ Border $\rightarrow$ Margin.CSS.box-example {
    width: 300px;
    padding: 20px;           /* Space between content and border */
    border: 2px solid #cbd5e1; /* Outer boundary frame */
    margin: 15px auto;       /* Space outside the border; centers element horizontally */
}
