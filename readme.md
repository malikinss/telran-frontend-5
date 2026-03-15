# Homework 5 – Star Wars Page

## Task Definition

Create an HTML page with CSS styles according to the classwork design about Star Wars.

**Requirements:**

1. Build the "Dream Team" block **without using `<table>`**.
2. Implement responsive layout using CSS (floats or positioning).
3. Include a navigation menu, header, main content, and footer.
4. Use images, text, and hover effects for styling.

---

## 📝 Description

This project creates a **Star Wars-themed page** featuring:

- **Header** with navigation menu and main title (_Luke Skywalker_).
- **Left section** with Luke's image.
- **Right section** called "Dream Team" showcasing 9 character images in a **grid-style gallery** (no `<table>` used).
- **Text section** describing Luke's story.
- **Footer** with a styled button.

---

## 📁 Project Structure

```

/project
├─ index.html
├─ CSS/
│   └─ style.css
└─ Images/
	├─ sky.jpg
	├─ luke.jpg
	├─ friend1.jpg
	├─ friend2.jpg
	├─ friend3.jpg
	├─ friend4.jpg
	├─ friend5.jpg
	├─ friend6.jpg
	├─ friend7.jpg
	├─ friend8.jpg
	├─ friend9.jpg
	└─ icon.jpg

```

---

## 🎯 Purpose

This homework focuses on practicing:

1. **Page layout** using floats and positioning.
2. Creating a **grid-like image gallery** without tables.
3. Styling with **CSS hover effects, rounded corners, and background images**.
4. Responsive design with **flexible widths and margins**.

---

## 🔍 How It Works

### 1. Header and Navigation

- **Navigation** is fixed to the top.
- **Menu items** are inline and spaced horizontally.
- **Header** contains the main title centered.

```css
header,
footer {
	background-color: rgba(68, 69, 67, 0.6);
	padding: 0.5em;
	border-radius: 16px;
}

nav {
	position: fixed;
	top: 0;
	width: 100%;
	z-index: 1000;
}
```

---

### 2. Left Section – Luke's Image

- Floated left with **25% width**.
- Image is full-width of container, with **rounded corners** and **shadow**.

```css
.left {
	float: left;
	width: 25%;
	margin-right: 1.2rem;
}

.left img {
	width: 100%;
	box-shadow: 0.6rem 0.6rem 0.6rem gray;
	border-radius: 16px;
	display: block;
}
```

---

### 3. Right Section – Dream Team Gallery

- Floated right with **50% width**.
- Contains `h2` title and `.gallery` with 9 images.
- Images are floated left, **32% width** each, allowing 3 per row with **equal spacing**.

```css
.gallery img {
	float: left;
	width: 32%;
	margin: calc(4% / (3 * 2));
	border-radius: 16px;
	transition: transform 0.3s;
}

.gallery img:hover {
	transform: scale(1.05);
}
```

---

### 4. Text Section

- Large, justified text describing Luke's story.
- Letter spacing and line height adjusted for readability.

```css
.fartext {
	font-size: 1.8rem;
	letter-spacing: 0.1em;
	text-align: justify;
	line-height: 1.5;
	margin: 1em;
}
```

---

### 5. Footer

- Full width with semi-transparent background.
- Button positioned and styled with **hover effect**.

```css
footer .button {
	position: relative;
	right: 40%;
}
```

---

## 📜 Example Layout

```
------------------------------------------------
| Header: Navigation + Luke Skywalker Title   |
------------------------------------------------
| Left: Luke Image   | Right: Dream Team      |
|                   | Image Gallery (3x3)    |
------------------------------------------------
| Text describing Luke's story                 |
------------------------------------------------
| Footer: Send me email                        |
------------------------------------------------
```

---

## 📦 Usage

1. Open `index.html` in a web browser.
2. Ensure all images exist in the `/Images` folder.
3. The page displays **Luke Skywalker**, a **Dream Team gallery**, and story text with styled header/footer.

---

## ✅ Project Status

**Status:** ✅ Completed

- Dream Team gallery created without `<table>`.
- Floats used for multi-column layout.
- Hover effects applied to images and buttons.
- Responsive design with relative widths.

---

## 📄 License

MIT License

---

Made with ❤️ using **HTML + CSS** by **Sam Malikin**
