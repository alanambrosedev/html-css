## 🧩 HTML & CSS Flash Practice Notes

### 🧱 1. HTML Structure

**Q: Write the basic HTML5 boilerplate.**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body></body>
</html>
```

**Q: Add a main title, one paragraph, and an image with alt text.**

```html
<h1>Welcome</h1>
<p>
  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Suscipit possimus
  quasi dolorem itaque quae veritatis ab minima officiis.
</p>
<img src="https://picsum.photos/200/300" alt="profile pic" />
```

---

### 🔗 2. Links and Semantic Tags

**Q: Create a navigation bar using semantic HTML (`<nav>`, `<ul>`, `<li>`, `<a>`).**

```html
<nav>
  <ul>
    <li><a href="https://picsum.photos/200/300">Profile Pic</a></li>
  </ul>
</nav>
```

**Q: Add a footer that says “© 2025 My Website”.**

```html
<footer><p>© 2025 My Website</p></footer>
```

---

### 🎨 3. CSS Box Model

**Q: Draw (mentally or on paper) the box model and label:**

- **Content** → inside
- **Padding** → space around content
- **Border** → edge around padding
- **Margin** → space outside the border

**Q: Add 20px padding and 10px margin to a `.card` class.**

```css
.card {
  padding: 20px;
  margin: 10px; /* ✅ fixed typo: was '10ox' */
}
```

---

### 🧭 4. Display & Position

**Q: Make `.nav-item` appear side by side using CSS.**

```css
.nav-container {
  display: flex;
  gap: 1rem; /* optional spacing */
}

.nav-item {
  /* no need for flex here unless styling internal content */
}
```

**Q: Position a `.badge` absolutely inside a relative `.card`.**

```css
.card {
  position: relative;
}

.badge {
  position: absolute;
  top: 10px;
  right: 10px;
}
```

---

### ⚙️ 5. Flexbox

**Q: Create a flex container that centers items both horizontally and vertically.**

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh; /* optional for full viewport centering */
}
```

**Q: Stack items vertically using Flexbox.**

```css
.container {
  display: flex;
  flex-direction: column;
  align-items: center; /* centers items horizontally */
}
```

---

### 📱 6. Responsive Design

**Q: At screen width below 600px, stack all cards vertically.**

```css
@media (max-width: 600px) {
  .card-container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .card {
    width: 100%;
    margin-bottom: 1rem;
  }
}
```

---

### ✨ 7. Hover & Transition

**Q: Make `.card` lift up slightly and cast a deeper shadow on hover.**

```css
.card {
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
  transform: translateY(-10px);
  box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.2);
}
```
