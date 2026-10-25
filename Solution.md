## Assignment 7.3 — Responsive Product Listing

### 1. `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Product Listing</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Our Products</h1>

    <div class="product-container">
        <div class="card">
            <img src="https://placehold.co/200x120" alt="Laptop">
            <h3>Laptop</h3><p>₹50,000</p>
            <button>Buy Now</button>
        </div>

        <div class="card">
            <img src="https://placehold.co/200x120" alt="Headphones">
            <h3>Headphones</h3><p>₹1,500</p>
            <button>Buy Now</button>
        </div>

        <div class="card">
            <img src="https://placehold.co/200x120" alt="Smartphone">
            <h3>Smartphone</h3><p>₹20,000</p>
            <button>Buy Now</button>
        </div>

        <div class="card">
            <img src="https://placehold.co/200x120" alt="Keyboard">
            <h3>Keyboard</h3><p>₹800</p>
            <button>Buy Now</button>
        </div>

        <div class="card">
            <img src="https://placehold.co/200x120" alt="Mouse">
            <h3>Mouse</h3><p>₹500</p>
            <button>Buy Now</button>
        </div>

        <div class="card">
            <img src="https://placehold.co/200x120" alt="Smartwatch">
            <h3>Smartwatch</h3><p>₹2,500</p>
            <button>Buy Now</button>
        </div>
    </div>
</body>
</html>
```

### 2. `style.css`

```css
body {
    font-family: Arial, sans-serif;
    background: #f0f4f8;
    margin: 20px;
    text-align: center;
}

.product-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.card {
    flex-grow: 1;
    flex-shrink: 1;
    flex-basis: 200px;
    max-width: 250px;
    padding: 15px;
    background: white;
    border-radius: 10px;
    box-shadow: 0 3px 8px #ccc;
}

.card img {
    width: 100%;
    height: 120px;
    object-fit: cover;
}

button {
    background: navy;
    color: white;
    padding: 10px 15px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

@media (max-width: 500px) {
    .card {
        flex-basis: 100%;
        max-width: 100%;
    }
}
```

**Submission:** Open `index.html` using Live Server. Take one screenshot at desktop width and another at mobile width. Cards wrap automatically because of `flex-wrap: wrap`.