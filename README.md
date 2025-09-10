<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GOSSIP MENU</title>
<style>
body {margin:0; font-family:"Georgia", serif; background-color:#fffdf6; color:#3e2f1c;}
header {background:linear-gradient(90deg, #5e4632, #a18860); color:white; padding:20px; text-align:center;}
header h1 {margin:0; font-size:2.5em; letter-spacing:2px;}
nav {background:#3e2f1c; display:flex; justify-content:center; flex-wrap:wrap;}
nav a {color:#f5e1a4; padding:12px 20px; text-decoration:none; font-weight:bold; transition:background 0.3s;}
nav a:hover {background:#a18860; color:#fff;}
section {padding:40px 20px; max-width:900px; margin:auto; animation:fadeIn 1s ease-in;}
section h2 {border-bottom:3px solid #a18860; padding-bottom:10px; margin-bottom:20px; font-size:1.8em; text-transform:uppercase;}
.item {display:flex; justify-content:space-between; padding:8px 0; border-bottom:1px dotted #c9b89a;}
.item:last-child {border:none;}
.price {font-weight:bold; color:#5e4632;}
@keyframes fadeIn {from {opacity:0; transform:translateY(20px);} to {opacity:1; transform:translateY(0);}}
</style>
</head>
<body>

<header>
  <h1>GOSSIP</h1>
  <p>LIVE • LAUGH • GOSSIP</p>
</header>

<nav>
  <a href="#breakfast">Breakfast</a>
  <a href="#appetizers">Appetizers</a>
  <a href="#soups">Soups</a>
  <a href="#salads">Salads</a>
  <a href="#chicken">Chicken</a>
  <a href="#meat">Meat</a>
  <a href="#seafood">Seafood</a>
  <a href="#pasta">Pasta</a>
  <a href="#pizza">Pizza</a>
  <a href="#burgers">Burgers</a>
  <a href="#sandwiches">Sandwiches</a>
  <a href="#dessert">Dessert</a>
  <a href="#drinks">Drinks</a>
  <a href="#extras">Extras</a>
</nav>

<section id="breakfast">
<h2>Breakfast</h2>
<div class="item"><span>Standard Breakfast</span><span class="price">350</span></div>
<div class="item"><span>Extras</span><span class="price">60</span></div>
</section>

<section id="appetizers">
<h2>Appetizers</h2>
<div class="item"><span>Mozzarella Sticks (5 pcs)</span><span class="price">120</span></div>
<div class="item"><span>French Fries</span><span class="price">60</span></div>
<div class="item"><span>Homemade Chips</span><span class="price">60</span></div>
<div class="item"><span>Chicken Strips (5 pcs)</span><span class="price">150</span></div>
<div class="item"><span>Chicken Wings (6 pcs)</span><span class="price">135</span></div>
<div class="item"><span>Fried Shrimps</span><span class="price">190</span></div>
<div class="item"><span>Shrimp Cocktail</span><span class="price">200</span></div>
<div class="item"><span>Calamari</span><span class="price">—</span></div>
<div class="item"><span>Oriental Sausages</span><span class="price">170</span></div>
<div class="item"><span>White Cheese & Tomatoes</span><span class="price">80</span></div>
<div class="item"><span>Carrots & Cucumber Slices</span><span class="price">50</span></div>
<div class="item"><span>Tehina</span><span class="price">60</span></div>
<div class="item"><span>Pickles</span><span class="price">40</span></div>
</section>

<section id="soups">
<h2>Soups</h2>
<div class="item"><span>Seasonal Soup</span><span class="price">110</span></div>
<div class="item"><span>Molokheya</span><span class="price">90</span></div>
<div class="item"><span>Seafood Soup</span><span class="price">220</span></div>
<div class="item"><span>Chicken Cream</span><span class="price">150</span></div>
<div class="item"><span>Mushroom</span><span class="price">130</span></div>
<div class="item"><span>Onion</span><span class="price">140</span></div>
</section>

<section id="salads">
<h2>Salads</h2>
<div class="item"><span>Shrimp Caesar Salad</span><span class="price">210</span></div>
<div class="item"><span>Chicken Caesar Salad</span><span class="price">160</span></div>
<div class="item"><span>Greek Salad</span><span class="price">210</span></div>
<div class="item"><span>Tuna Salad</span><span class="price">210</span></div>
<div class="item"><span>Rocca Salad</span><span class="price">240</span></div>
<div class="item"><span>Gossip Salad</span><span class="price">300</span></div>
</section>

<section id="chicken">
<h2>Chicken</h2>
<div class="item"><span>Shredded Mexican Chicken</span><span class="price">290</span></div>
<div class="item"><span>Chicken Curry</span><span class="price">290</span></div>
<div class="item"><span>Chicken Panne</span><span class="price">290</span></div>
<div class="item"><span>Crispy Chicken</span><span class="price">320</span></div>
<div class="item"><span>Grilled Chicken with Lemon Sauce</span><span class="price">330</span></div>
<div class="item"><span>Grilled Chicken with Mushroom Sauce</span><span class="price">350</span></div>
<div class="item"><span>Chicken Cordon Bleu</span><span class="price">310</span></div>
<div class="item"><span>Chicken Cacciatore</span><span class="price">360</span></div>
<div class="item"><span>Chicken Gossip</span><span class="price">360</span></div>
</section>

<section id="meat">
<h2>Meat</h2>
<div class="item"><span>Beef Stroganoff</span><span class="price">450</span></div>
<div class="item"><span>Beef Fillet with Mushroom/Garlic/Pepper</span><span class="price">580</span></div>
<div class="item"><span>Surf & Turf</span><span class="price">610</span></div>
<div class="item"><span>Mixed Grill</span><span class="price">550</span></div>
</section>

<section id="seafood">
<h2>Seafood</h2>
<div class="item"><span>Mixed Seafood Platter</span><span class="price">520</span></div>
<div class="item"><span>Jumbo Shrimps (8 pcs)</span><span class="price">590</span></div>
<div class="item"><span>Salmon Fillet Lemon and Butter Sauce</span><span class="price">680</span></div>
<div class="item"><span>Fish and Chips</span><span class="price">340</span></div>
</section>

<section id="pasta">
<h2>Pasta</h2>
<div class="item"><span>Arabiata</span><span class="price">165</span></div>
<div class="item"><span>Alfredo</span><span class="price">210</span></div>
<div class="item"><span>Bolognese</span><span class="price">210</span></div>
<div class="item"><span>Negresco</span><span class="price">250</span></div>
<div class="item"><span>Crispy Chicken</span><span class="price">210</span></div>
<div class="item"><span>Seafood</span><span class="price">290</span></div>
<div class="item"><span>Chicken Pesto</span><span class="price">240</span></div>
<div class="item"><span>Mac Cheese</span><span class="price">220</span></div>
<div class="item"><span>Mushroom</span><span class="price">190</span></div>
</section>

<section id="pizza">
<h2>Pizza</h2>
<div class="item"><span>Pizza Margherita</span><span class="price">200</span></div>
<div class="item"><span>Pizza Vegetarian</span><span class="price">200</span></div>
<div class="item"><span>Pizza Chicken (BBQ/Ranch)</span><span class="price">240</span></div>
<div class="item"><span>Pizza Oriental Sausage</span><span class="price">250</span></div>
<div class="item"><span>Pizza Tuna</span><span class="price">250</span></div>
<div class="item"><span>Pizza Seafood</span><span class="price">290</span></div>
<div class="item"><span>Pizza Salami</span><span class="price">250</span></div>
<div class="item"><span>Pizza Anchovies</span><span class="price">290</span></div>
<div class="item"><span>Pizza Mixed Beef</span><span class="price">300</span></div>
</section>

<section id="burgers">
<h2>Burgers</h2>
<div class="item"><span>Classic Burger</span><span class="price">280</span></div>
<div class="item"><span>Cheese Burger</span><span class="price">300</span></div>
<div class="item"><span>Mushroom Burger</span><span class="price">310</span></div>
<div class="item"><span>Gossip Burger</span><span class="price">340</span></div>
</section>

<section id="sandwiches">
<h2>Sandwiches</h2>
<div class="item"><span>Chicken Panne</span><span class="price">210</span></div>
<div class="item"><span>Chicken Crispy</span><span class="price">210</span></
