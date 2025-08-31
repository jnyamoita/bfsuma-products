# bfsuma-products
JANE NYAMOITA BFSUMA PRODUCTS
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>BFsuma Products</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom right, #ffe4ec, #e6e6fa, #d6f0ff);
      color: #333;
    }
    header {
      background: #fff;
      padding: 15px 30px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      flex-wrap: wrap;
    }
    header h1 {
      font-size: 24px;
      background: linear-gradient(to right, #ff4d94, #7a42f4);
      -webkit-background-clip: text;
      color: transparent;
      margin: 0;
    }
    nav {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      align-items: center;
    }
    nav a {
      text-decoration: none;
      color: #555;
      font-weight: bold;
      transition: color 0.3s;
      cursor: pointer;
    }
    nav a:hover {
      color: #ff4d94;
    }
    .hero {
      text-align: center;
      padding: 50px 20px;
      background: linear-gradient(to right, #ffb6d5, #d8b6ff, #b6e0ff);
    }
    .hero h2 {
      font-size: 32px;
      margin: 0;
    }
    .hero p {
      font-size: 18px;
      margin: 10px 0 20px;
    }
    .hero button {
      padding: 12px 25px;
      border: none;
      border-radius: 25px;
      font-size: 16px;
      font-weight: bold;
      background: linear-gradient(to right, #ff4d94, #7a42f4);
      color: #fff;
      cursor: pointer;
      transition: transform 0.2s;
    }
    .hero button:hover {
      transform: scale(1.05);
    }
    .section {
      padding: 40px 20px;
      text-align: center;
    }
    .section h2 {
      font-size: 28px;
      margin-bottom: 20px;
      color: #ff4d94;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
      padding: 0 20px;
    }
    .product {
      background: #fff;
      border-radius: 20px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      overflow: hidden;
      transition: transform 0.2s;
    }
    .product:hover {
      transform: scale(1.05);
    }
    .product img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }
    .product-info {
      padding: 15px;
    }
    .product-info h3 {
      margin: 0;
      font-size: 18px;
    }
    .product-info p {
      color: #ff4d94;
      font-weight: bold;
      margin: 10px 0;
    }
    .product-info button {
      width: 100%;
      padding: 10px;
      border: none;
      border-radius: 10px;
      background: linear-gradient(to right, #ff4d94, #7a42f4);
      color: #fff;
      font-weight: bold;
      cursor: pointer;
    }
    #cartList {
      list-style: none;
      padding: 0;
      max-width: 600px;
      margin: auto;
    }
    #cartList li {
      background: #fff;
      margin: 10px 0;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      text-align: left;
    }
    footer {
      text-align: center;
      padding: 20px;
      background: linear-gradient(to right, #b6e0ff, #d8b6ff, #ffb6d5);
      margin-top: 30px;
    }
  </style>
</head>
<body>

  <header>
    <h1>BFsuma Products</h1>
    <nav>
      <a href="#home">HOME</a>
      <a href="#about">ABOUT US</a>
      <a href="#products">PRODUCTS</a>
      <a href="#news">NEWS</a>
      <a href="#contact">CONTACTS</a>
      <a href="#cart">CART 🛒</a>
      <!-- Social Media Links -->
      <a href="https://www.facebook.com/Janet-Nyomaita" target="_blank">Facebook</a>
      <a href="https://www.instagram.com/Nyomaita-janet" target="_blank">Instagram</a>
      <a href="https://www.tiktok.com/@Janetnyamoita51" target="_blank">TikTok</a>
      <a href="https://www.youtube.com/@janetnyamoita7594" target="_blank">YouTube</a>
    </nav>
  </header>

  <section id="home" class="hero">
    <h2>Welcome to BFsuma Products</h2>
    <p>Your trusted source for natural supplements & health solutions ✨</p>
    <button onclick="document.getElementById('products').scrollIntoView({behavior:'smooth'})">Start Shopping</button>
  </section>

  <section id="about" class="section">
    <h2>About Us</h2>
    <p>BFsuma Products is dedicated to providing high-quality health supplements designed to 
       support wellness and help manage a wide range of health conditions.  
       From boosting immunity, managing chronic illnesses, supporting energy, digestion, heart 
       health, and overall body vitality – we have supplements for all diseases and body needs.  
       We believe in a healthier, stronger, and happier you through natural health solutions.</p>
  </section>

  <section id="products" class="section">
    <h2>Products</h2>
    <div class="products">
      <div class="product">
        <img src="https://source.unsplash.com/400x400/?supplements" alt="Health Supplement">
        <div class="product-info">
          <h3>Immune Booster</h3>
          <p>KES 4500</p>
          <button onclick="addToCart('Immune Booster - KES 4500')">Add to Cart</button>
        </div>
      </div>
      <div class="product">
        <img src="https://source.unsplash.com/400x400/?vitamins" alt="Vitamins">
        <div class="product-info">
          <h3>Multivitamins</h3>
          <p>KES 3800</p>
          <button onclick="addToCart('Multivitamins - KES 3800')">Add to Cart</button>
        </div>
      </div>
      <div class="product">
        <img src="https://source.unsplash.com/400x400/?herbal" alt="Herbal Capsules">
        <div class="product-info">
          <h3>Herbal Capsules</h3>
          <p>KES 5000</p>
          <button onclick="addToCart('Herbal Capsules - KES 5000')">Add to Cart</button>
        </div>
      </div>
    </div>
  </section>

  <section id="news" class="section">
    <h2>News</h2>
    <p>Stay tuned for updates on our latest arrivals, health tips, and discounts! 🌟</p>
  </section>

  <section id="contact" class="section">
    <h2>Contacts</h2>
    <p>📍 Location: Nairobi, Kenya</p>
    <p>📞 Phone: 0713960775</p>
    <p>✉️ Email: bfsuma@healthproducts.com</p>
  </section>

  <section id="cart" class="section">
    <h2>Your Cart</h2>
    <ul id="cartList"></ul>
    <p id="emptyCart">Your cart is empty.</p>
  </section>

  <footer>
    <p>© 2025 BFsuma Products | Designed with ❤️ for your health</p>
  </footer>

  <script>
    let cart = [];
    function addToCart(product) {
      cart.push(product);
      updateCart();
      alert(product + " has been added to your cart! 🛒");
    }
    function updateCart() {
      const cartList = document.getElementById("cartList");
      const emptyMsg = document.getElementById("emptyCart");
      cartList.innerHTML = "";
      if (cart.length === 0) {
        emptyMsg.style.display = "block";
      } else {
        emptyMsg.style.display = "none";
        cart.forEach((item, index) => {
          const li = document.createElement("li");
          li.textContent = item;
          cartList.appendChild(li);
        });
      }
    }
  </script>

</body>
</html>
