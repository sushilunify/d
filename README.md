// all css from halabox website becuase trhis websiote in uindertaken by mne 
body {
    font-family: Arial, sans-serif;
    padding: 20px;
}

.products {
    display: flex;
    gap: 20px;
}

.product {
    border: 1px solid #ccc;
    padding: 15px;
    width: 150px;
    text-align: center;
}

button {
    background-color: #28a745;
    color: white;
    border: none;
    padding: 8px;
    cursor: pointer;
}

button:hover {
    background-color: #218838;
}****
body {
    font-family: Arial, sans-serif;
    padding: 20px;
}

.products {
    display: flex;
    gap: 20px;
}

.product {
    border: 1px solid #ccc;
    padding: 15px;
    width: 150px;
    text-align: center;
}

button {
    background-color: #28a745;
    color: white;
    border: none;
    padding: 8px;
    cursor: pointer;
}

button:hover {
    background-color: #218838;
}


// all code from website 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Simple E-Commerce</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<h1>My Shop</h1>

<div class="products">
    <div class="product">
        <h3>Product 1</h3>
        <p>$10</p>
        <button onclick="addToCart('Product 1', 10)">Add to Cart</button>
    </div>

    <div class="product">
        <h3>Product 2</h3>
        <p>$20</p>
        <button onclick="addToCart('Product 2', 20)">Add to Cart</button>
    </div>
</div>

<h2>Cart</h2>
<ul id="cart"></ul>
<p><strong>Total:</strong> $<span id="total">0</span></p>

<script src="script.js"></script>
</body>
</html>
script from website

let total = 0;

function addToCart(name, price) {
    const cart = document.getElementById("cart");
    const item = document.createElement("li");
    item.textContent = `${name} - $${price}`;
    cart.appendChild(item);

    total += price;
    document.getElementById("total").textContent = total;
}

