# Pizza_Landing_page

HTML (index.html):

```html
<!DOCTYPE html>
```
- This line declares the document type and version of HTML being used

```html
<html lang="en">
```
- This line starts the HTML document and specifies the language attribute as "en" for English.

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pizza Landing Page</title>
    <link rel="stylesheet" href="styles.css">
</head>
```
- The `<head>` section contains metadata for the document, including character encoding, viewport settings for responsiveness, and the document title.
- It also links an external stylesheet (`styles.css`) to apply styles to the HTML elements.

```html
<body>
```
- The `<body>` section contains the content of the HTML document.

```html
    <header>
        <h1>Welcome to Pizza Palace</h1>
        <nav>
            <ul>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#about">About Us</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
```
- This section defines the header of the page, including the main heading ("Welcome to Pizza Palace") and a navigation menu with links to different sections of the page.

```html
    <section id="hero">
        <div class="hero-text">
            <h2>Delicious Pizza</h2>
            <p>Order Now and Get 20% Off</p>
            <a href="#menu" class="btn">Order Now</a>
        </div>
    </section>
```
- The `<section>` element with the ID "hero" contains the hero section of the page, which typically features a prominent image or message to capture the visitor's attention. In this case, it showcases a message about delicious pizza and an order button.

```html
    <section id="menu">
        <h2>Our Menu</h2>
        <div class="menu-item">
            <img src="pizza.jpg" alt="Pizza">
            <h3>Classic Margherita</h3>
            <p>Fresh tomatoes, mozzarella, basil</p>
            <span>$10</span>
        </div>
        <!-- More menu items can be added here -->
    </section>
```
- The `<section>` element with the ID "menu" displays the menu of the pizza place. It includes various menu items with images, names, descriptions, and prices.

```html
    <section id="about">
        <h2>About Us</h2>
        <p>We are passionate about making the best pizzas in town. Our ingredients are sourced locally and our recipes are crafted with love.</p>
    </section>
```
- This section provides information about the pizza place, including a brief description of its values and offerings.

```html
    <section id="contact">
        <h2>Contact Us</h2>
        <form id="contact-form">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            <button type="submit">Send</button>
        </form>
    </section>
```
- This section contains a contact form where visitors can submit their name, email, and message to the pizza place.

```html
    <footer>
        <p>&copy; 2024 Pizza Palace. All rights reserved.</p>
    </footer>
```
- The footer of the page, which typically includes copyright information or other relevant details.

```html
    <script src="script.js"></script>
</body>
</html>
```
- This line includes an external JavaScript file (`script.js`) to add interactivity or functionality to the page.

CSS (styles.css):

```css
/* styles.css */

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}
```
- This block of CSS code sets the font family for the entire page to Arial or sans-serif, removes default margin and padding from the body element.

```css
header {
    background-color: #f8f8f8;
    padding: 20px;
    text-align: center;
}
```
- Styles the header section with a light gray background color, 20 pixels of padding, and centers the content.

```css
nav ul {
    list-style-type: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin-right: 20px;
}

nav ul li a {
    text-decoration: none;
    color: #333;
}
```
- Defines styles for the navigation menu, removing default list styles, setting padding to 0, and styling list items as inline elements with 20 pixels of right margin. Also removes underline from anchor elements and sets their color to dark gray.

```css
#hero {
    background-image: url('pizza-hero.jpg');
    background-size: cover;
    color: #fff;
    text-align: center;
    padding: 100px 20px;
}
```
- Styles the hero section with a background image ('pizza-hero.jpg'), covering the entire area, setting text color to white, centering the content both horizontally and vertically, and providing padding of 100 pixels at the top and bottom and 20 pixels on the sides.

```css
.menu-item {
    margin-bottom: 30px;
}

.menu-item img {
    width: 100%;
    height: auto;
}
```
- Styles menu items with 30 pixels of bottom margin. Ensures menu item images occupy 100% of their container width while maintaining their aspect ratio.

```css
.btn {
    background-color: #FF4500;
    color: #fff;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    text-decoration: none;
}
```
- Styles buttons with an orange background color, white text color, 10 pixels of padding on top and bottom, 20 pixels of padding on the sides, no border, and a border-radius of 5 pixels. Also removes underline from anchor elements.

```css
#about,
#contact {
    padding: 50px;
}
```
- Applies 50 pixels of padding to the about and contact sections.

```css
footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 20px;
}
```
- Styles the footer with a dark background color, white text color, centered text, and 20 pixels of padding.

JavaScript (script.js):

```javascript
// Add any JavaScript functionality here if needed
document.getElementById("contact-form").addEventListener("submit", function(event){
    event.preventDefault(); // Prevent form submission
    // Add your code to handle form submission (e
