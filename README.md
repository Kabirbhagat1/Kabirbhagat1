## Hi there 👋
ecommerce-site/
│
├── backend/
│   ├── server.js
│   ├── models/
│   └── routes/
│
├── frontend/
│   ├── index.html
│   ├── product.html
│   ├── cart.html
│   ├── css/
│   │   └── styles.css
│   └── js/
│       └── script.js
│
└── README.md
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>ShopEasy</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <h1>ShopEasy</h1>
        <nav>
            <a href="index.html">Home</a>
            <a href="cart.html">Cart</a>
        </nav>
    </header>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}
header {
    background-color: #222;
    color: white;
    padding: 15px;
    text-align: center;
}
nav a {
    margin: 0 10px;
    color: white;
    text-decoration: none;
}
#product-list {
    display: flex;
    flex-wrap: wrap;
    padding: 20px;
    gap: 20px;
}
.product {
    border: 1px solid #ccc;
    padding: 15px;
    width: 200px;
}
    <main id="product-list"></main>

    <script src="js/script.js"></script>
</body>ecommerce-site/
│
├── backend/
│   ├── server.js
│   ├── models/
│   └── routes/
│
├── frontend/
│   ├── index.html
│   ├── product.html
│   ├── cart.html
│   ├── css/
│   │   └── styles.css
│   └── js/
│       └── script.js
│
└── README.md
</html><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>ShopEasy</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <h1>ShopEasy</h1>
        <nav>
            <a href="index.html">Home</a>
            <a href="cart.html">Cart</a>
        </nav>
    </header>

    <main id="product-list"></main>

    <script src="js/script.js"></script>
</body>
</html>const products = [
    { id: 1, name: "T-shirt", price: 299, image: "https://via.placeholder.com/150" },
    { id: 2, name: "Shoes", price: 999, image: "https://via.placeholder.com/150" }
];

window.onload = function () {
    const productList = document.getElementById("product-list");
    products.forEach(p => {
        const div = document.createElement("div");
        div.className = "product";
        div.innerHTML = `
            <img src="${p.image}" alt="${p.name}" width="150">
            <h3>${p.name}</h3>
            <p>Price: ₹${p.price}</p>
            <button onclick="addToCart(${p.id})">Add to Cart</button>
        `;
        productList.appendChild(div);
    });
};

function addToCart(productId) {
    alert(`Product ${productId} added to cart!`);
}const express = require('express');
const cors = require('cors');
const app = express();

app.use(cors());
app.use(express.json());

const products = [
    { id: 1, name: 'T-shirt', price: 299 },
    { id: 2, name: 'Shoes', price: 999 }
];

app.get('/api/products', (req, res) => {
    res.json(products);
});

app.listen(3000, () => console.log('Server running on http://localhost:3000'));
**Kabirbhagat1/Kabirbhagat1** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
