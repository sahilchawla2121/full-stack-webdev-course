# 02. Flexbox & CSS Grid Layouts

Modern layout engines enable robust arrangement of elements across single and multi-dimensional planes.

---

## 📏 Flexbox (1-Dimensional Layouts)
Flexbox handles items in either rows or columns, making alignment and distribution intuitive.

```css
.flex-container {
    display: flex;
    flex-direction: row;        /* Arranges items horizontally */
    justify-content: space-between; /* Spreads items evenly along main axis */
    align-items: center;        /* Centers items vertically along cross axis */
    gap: 16px;                  /* Creates uniform gap between items */
}



📐 CSS Grid (2-Dimensional Layouts)
CSS Grid manages columns and rows simultaneously for complex structured layouts.

CSS
.grid-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr); /* Creates 3 equal-width columns */
    grid-template-rows: 200px 200px;       /* Defines two row heights */
    gap: 20px;                             /* Spacing between grid cells */
}

.grid-item {
    background-color: #f8fafc;
    padding: 20px;
}
