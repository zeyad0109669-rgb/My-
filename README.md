‏<!DOCTYPE html>
‏<html lang="en">
‏<head>
‏<meta charset="UTF-8">
‏<meta name="viewport" content="width=device-width, initial-scale=1.0">
‏<title>GOSSIP MENU</title>
‏<style>
‏body {margin:0; font-family:"Georgia", serif; background-color:#fffdf6; color:#3e2f1c;}
‏header {background:linear-gradient(90deg, #5e4632, #a18860); color:white; padding:20px; text-align:center;}
‏header h1 {margin:0; font-size:2.5em; letter-spacing:2px;}
‏nav {background:#3e2f1c; display:flex; justify-content:center; flex-wrap:wrap;}
‏nav a {color:#f5e1a4; padding:12px 20px; text-decoration:none; font-weight:bold; transition:background 0.3s;}
‏nav a:hover {background:#a18860; color:#fff;}
‏section {padding:40px 20px; max-width:900px; margin:auto; animation:fadeIn 1s ease-in;}
‏section h2 {border-bottom:3px solid #a18860; padding-bottom:10px; margin-bottom:20px; font-size:1.8em; text-transform:uppercase;}
‏.item {display:flex; justify-content:space-between; padding:8px 0; border-bottom:1px dotted #c9b89a;}
‏.item:last-child {border:none;}
‏.price {font-weight:bold; color:#5e4632;}
‏@keyframes fadeIn {from {opacity:0; transform:translateY(20px);} to {opacity:1; transform:translateY(0);}}
‏</style>
‏</head>
‏<body>

‏<header>
‏  <h1>GOSSIP</h1>
‏  <p>LIVE • LAUGH • GOSSIP</p>
‏</header>

‏<nav>
‏  <a href="#hotdrinks">Hot Drinks</a>
‏  <a href="#iceddrinks">Iced Drinks</a>
‏  <a href="#frappe">Frappé</a>
‏  <a href="#smoothies">Smoothies & Milk Shakes</a>
‏  <a href="#softdrinks">Soft Drinks</a>
‏  <a href="#cocktails">Cocktails</a>
‏  <a href="#extras">Extras</a>
‏  <a href="#dessert">Dessert</a>
‏  <a href="#breakfast">Breakfast</a>
‏  <a href="#appetizers">Appetizers</a>
‏  <a href="#soups">Soups</a>
‏  <a href="#salads">Salads</a>
‏  <a href="#chicken">Chicken</a>
‏  <a href="#meat">Meat</a>
‏  <a href="#seafood">Seafood</a>
‏  <a href="#pasta">Pasta</a>
‏  <a href="#pizza">Pizza</a>
‏  <a href="#burgers">Burgers</a>
‏  <a href="#sandwiches">Sandwiches</a>
‏</nav>

‏<!-- Hot Drinks -->
‏<section id="hotdrinks">
‏<h2>Hot Drinks</h2>
‏<div class="item"><span>Espresso</span><span class="price">57</span></div>
‏<div class="item"><span>Double Espresso</span><span class="price">75</span></div>
‏<div class="item"><span>Macchiato</span><span class="price">75</span></div>
‏<div class="item"><span>Double Macchiato</span><span class="price">85</span></div>
‏<div class="item"><span>Cappuccino</span><span class="price">105</span></div>
‏<div class="item"><span>Latte</span><span class="price">105</span></div>
‏<div class="item"><span>Nescafe</span><span class="price">85</span></div>
‏<div class="item"><span>Mocha</span><span class="price">115</span></div>
‏<div class="item"><span>Hot Chocolate</span><span class="price">100</span></div>
‏<div class="item"><span>Nutella Coffee</span><span class="price">100</span></div>
‏<div class="item"><span>Lotus Coffee</span><span class="price">110</span></div>
‏<div class="item"><span>Flat White</span><span class="price">110</span></div>
‏<div class="item"><span>Americano</span><span class="price">100</span></div>
‏<div class="item"><span>Turkish Coffee</span><span class="price">52</span></div>
‏<div class="item"><span>Double Turkish Coffee</span><span class="price">65</span></div>
‏<div class="item"><span>Turkish with Milk</span><span class="price">75</span></div>
‏<div class="item"><span>Turkish Hazelnut</span><span class="price">80</span></div>
‏<div class="item"><span>Tea</span><span class="price">50</span></div>
‏<div class="item"><span>Tea Pot (Zarda)</span><span class="price">90</span></div>
‏<div class="item"><span>Flavored Tea</span><span class="price">60</span></div>
‏<div class="item"><span>Mixed Herbs</span><span class="price">85</span></div>
‏<div class="item"><span>Hot Cider</span><span class="price">85</span></div>
‏</section>

‏<!-- Iced Drinks -->
‏<section id="iceddrinks">
‏<h2>Iced Drinks</h2>
‏<div class="item"><span>Iced Chocolate</span><span class="price">115</span></div>
‏<div class="item"><span>Iced Espresso</span><span class="price">115</span></div>
‏<div class="item"><span>Iced Latte</span><span class="price">115</span></div>
‏<div class="item"><span>Iced Mocha</span><span class="price">107</span></div>
‏<div class="item"><span>Iced Double Espresso</span><span class="price">120</span></div>
‏<div class="item"><span>Iced Nescafe</span><span class="price">105</span></div>
‏<div class="item"><span>Iced Tea</span><span class="price">100</span></div>
‏</section>

‏<!-- Frappé -->
‏<section id="frappe">
‏<h2>Frappé</h2>
‏<div class="item"><span>Caramel / Vanilla / Cinnamon / Hazelnut</span><span class="price">115</span></div>
‏<div class="item"><span>Mocha</span><span class="price">125</span></div>
‏<div class="item"><span>Lotus</span><span class="price">140</span></div>
‏</section>

‏<!-- Smoothies & Milk Shakes -->
‏<section id="smoothies">
‏<h2>Smoothies & Milk Shakes</h2>
‏<div class="item"><span>Smoothies (Mango, Strawberry, Lemon, Banana, Guava, Kiwi, Watermelon, Pomegranate)</span><span class="price">116</span></div>
‏<div class="item"><span>Milk Shake (Oreo, Kiwi, Mango, Strawberry, Vanilla, Chocolate)</span><span class="price">140</span></div>
‏<div class="item"><span>Milk Shake Nutella</span><span class="price">155</span></div>
‏<div class="item"><span>Milk Shake Lotus, Pistachio</span><span class="price">155</span></div>
‏</section>

‏<!-- Soft Drinks -->
‏<section id="softdrinks">
‏<h2>Soft Drinks</h2>
‏<div class="item"><span>Water Small</span><span class="price">25</span></div>
‏<div class="item"><span>Water Large</span><span class="price">50</span></div>
‏<div class="item"><span>Cola, Sprite, Fanta</span><span class="price">55</span></div>
‏<div class="item"><span>Fayrouz, Birell, Schweppes</span><span class="price">65</span></div>
‏<div class="item"><span>Red Bull</span><span class="price">130</span></div>
‏</section>

‏<!-- Cocktails -->
‏<section id="cocktails">
‏<h2>Cocktails</h2>
‏<div class="item"><span>Espresso Red Bull</span><span class="price">155</span></div>
‏<div class="item"><span>Cherry Cola</span><span class="price">95</span></div>
‏<div class="item"><span>Classic Mojito</span><span class="price">115</span></div>
‏<div class="item"><span>Flavored Mojito</span><span class="price">130</span></div>
‏<div class="item"><span>Sunshine</span><span class="price">95</span></div>
‏<div class="item"><span>Submarine</span><span class="price">120</span></div>
‏<div class="item"><span>Alex Night, Paradise</span><span class="price">130</span></div>
‏<div class="item"><span>Kiwi Slash, Blueberry Slash</span><span class="price">122</span></div>
‏<div class="item"><span>Fruit Mint</span><span class="price">112</span></div>
‏</section>

‏<!-- Extras -->
‏<section id="extras">
‏<h2>Extras</h2>
‏<div class="item"><span>Ice Cream</span><span class="price">50</span></div>
‏<div class="item"><span>Nuts</span><span class="price">50</span></div>
‏<div class="item"><span>Flavors</span><span class="price">50</span></div>
‏<div class="item"><span>Nutella</span><span class="price">50</span></div>
‏<div class="item"><span>Shishah Meassel (2)</span><span class="price">250</span></div>
‏<div class="item"><span>Flavors</span><span class="price">275</span></div>
‏<div class="item"><span>Pyrex Glass</span><span class="price">295</span></div>
‏</section>

‏<!-- Dessert -->
‏<section id="dessert">
‏<h2>Dessert</h2>
‏<div class="item"><span>Molten Cake</span><span class="price">140</span></div>
‏<div class="item"><span>Brownies</span><span class="price">120</span></div>
‏<div class="item"><span>Oreo Madness</span><span class="price">175</span></div>
‏<div class="item"><span>Om Aly with Nuts</span><span class="price">165</span></div>
‏<div class="item"><span>Classic Ice Cream (3 scoops)</span><span class="price">140</span></div>
‏<div class="item"><span>Waffle (Nutella, Lotus, Fruit, Caramel)</span><span class="price">150</span></div>
‏<div class="item"><span>Fruit Salad</span><span class="price">150</span></div>
‏</section>

‏<!-- Breakfast -->
‏<section id="breakfast">
‏<h2>Breakfast</h2>
‏<div class="item"><span>Standard Breakfast</span><span class="price">350</span></div>
‏<div class="item"><span>Extras</span><span class="price">60</span></div>
‏</section>

‏<!-- Appetizers -->
‏<section id="appetizers">
‏<h2>Appetizers</h2>
‏<div class="item"><span>Mozzarella Sticks (5 Pieces)</span><span class="price">120</span></div>
‏<div class="item"><span>French Fries</span><span class="price">60</span></div>
‏<div class="item"><span>Homemade Chips</span><span class="price">60</span></div>
‏<div class="item"><span>Chicken Strips (5 Pieces)</span><span class="price">150</span></div>
‏<div class="item"><span>Chicken Wings (6 Pieces)</span><span class="price">135</span></div>
‏<div class="item"><span>Fried Shrimps</span><span class="price">190</span></div>
‏<div class="item"><span>Shrimp Cocktail</span><span class="price">200</span></div>
‏<div class="item"><span>Calamari</span><span class="price">170</span></div>
‏<div class="item"><span>Oriental Sausages (Local Meat)</span><span class="price">170</span></div>
‏<div class="item"><span>White Cheese and Tomatoes</span><span class="price">80</span></div>
‏<div class="item"><span>Carrots & Cucumber Slices</span><span class="price">50</span></div>
‏<div class="item"><span>Tehina</span><span class="price">60</span></div>
‏<div class="item"><span>Pickles</span><span class="price">40</span></div>
‏</section>

‏<!-- Soups -->
‏<section id="soups">
‏<h2>Soups</h2>
‏<div class="item"><span>Seasonal Soup</span><span class="price">110</span></div>
‏<div class="item"><span>Molokheya</span><span class="price">90</span></div>
‏<div class="item"><span>Seafood</span><span class="price">220</span></div>
‏<div class="item"><span>Chicken Cream</span><span class="price">150</span></div>
‏<div class="item"><span>Mushroom</span><span class="price">130</span></div>
‏<div class="item"><span>Onion</span><span class="price">140</span></div>
‏</section>

‏<!-- Salads -->
‏<section id="salads">
‏<h2>Salads</h2>
‏<div class="item"><span>Shrimp Caesar Salad</span><span class="price">210</span></div>
‏<div class="item"><span>Chicken Caesar Salad</span><span class="price">160</span></div>
‏<div class="item"><span>Greek Salad</span><span class="price">210</span></div>
‏<div class="item"><span>Tuna Salad</span><span class="price">210</span></div>
‏<div class="item"><span>Rocca Salad</span><span class="price">240</span></div>
‏<div class="item"><span>Gossip Salad</span><span class="price">300</span></div>
‏</section>

‏<!-- Chicken -->
‏<section id="chicken">
‏<h2>Chicken</h2>
‏<div class="item"><span>Shredded Mexican Chicken</span><span class="price">290</span></div>
‏<div class="item"><span>Chicken Curry</span><span class="price">290</span></div>
‏<div class="item"><span>Chicken Panne</span><span class="price">290</span></div>
‏<div class="item"><span>Crispy Chicken</span><span class="price">320</span></div>
‏<div class="item"><span>Grilled Chicken with Lemon Sauce</span><span class="price">330</span></div>
‏<div class="item"><span>Grilled Chicken with Mushroom Sauce</span><span class="price">350</span></div>
‏<div class="item"><span>Chicken Cordon Bleu</span><span class="price">310</span></div>
‏<div class="item"><span>Chicken Cacciatore</span><span class="price">360</span></div>
‏<div class="item"><span>Chicken Gossip</span><span class="price">360</span></div>
‏</section>

‏<!-- Meat -->
‏<section id="meat">
‏<h2>Meat</h2>
‏<div class="item"><span>Beef Stroganoff</span><span class="price">450</span></div>
‏<div class="item"><span>Beef Fillet with Mushroom/Garlic/Pepper</span><span class="price">580</span></div>
‏<div class="item"><span>Surf & Turf</span><span class="price">610</span></div>
‏<div class="item"><span>Mixed Grill</span><span class="price">550</span></div>
‏</section>

‏<!-- Seafood -->
‏<section id="seafood">
‏<h2>Seafood</h2>
‏<div class="item"><span>Mixed Seafood Platter</span><span class="price">520</span></div>
‏<div class="item"><span>Jumbo Shrimps (8 pieces)</span><span class="price">590</span></div>
‏<div class="item"><span>Salmon Fillet Lemon and Butter Sauce</span><span class="price">680</span></div>
‏<div class="item"><span>Fish and Chips</span><span class="price">340</span></div>
‏</section>

‏<!-- Pasta -->
‏<section id="pasta">
‏<h2>Pasta</h2>
‏<div class="item"><span>Arabiata</span><span class="price">165</span></div>
‏<div class="item"><span>Alfredo</span><span class="price">210</span></div>
‏<div class="item"><span>Bolognese</span><span class="price">210</span></div>
‏<div class="item"><span>Negresco</span><span class="price">250</span></div>
‏<div class="item"><span>Crispy Chicken Pasta</span><span class="price">210</span></div>
‏<div class="item"><span>Seafood Pasta</span><span class="price">290</span></div>
‏<div class="item"><span>Chicken Pesto</span><span class="price">240</span></div>
‏<div class="item"><span>Mac Cheese</span><span class="price">220</span></div>
‏<div class="item"><span>Mushroom Pasta</span><span class="price">190</span></div>
‏</section>

‏<!-- Pizza -->
‏<section id="pizza">
‏<h2>Pizza</h2>
‏<div class="item"><span>Pizza Margherita</span><span class="price">200</span></div>
‏<div class="item"><span>Pizza Vegetarian</span><span class="price">200</span></div>
‏<div class="item"><span>Pizza Chicken (BBQ/Ranch)</span><span class="price">240</span></div>
‏<div class="item"><span>Pizza Oriental Sausage</span><span class="price">250</span></div>
‏<div class="item"><span>Pizza Tuna</span><span class="price">250</span></div>
‏<div class="item"><span>Pizza Seafood</span><span class="price">290</span></div>
‏<div class="item"><span>Pizza Salami</span><span class="price">250</span></div>
‏<div class="item"><span>Pizza Anchovies</span><span class="price">290</span></div>
‏<div class="item"><span>Pizza Mixed Beef</span><span class="price">300</span></div>
‏</section>

‏<!-- Burgers -->
‏<section id="burgers">
‏<h2>Burger Sandwiches</h2>
‏<div class="item"><span>Classic Burger</span><span class="price">280</span></div>
‏<div class="item"><span>Cheese Burger</span><span class="price">300</span></div>
‏<div class="item"><span>Mushroom Burger</span><span class="price">310</span></div>
‏<div class="item"><span>Gossip Burger</span><span class="price">340</span></div>
‏</section>

‏<!-- Sandwiches -->
‏<section id="sandwiches">
‏<h2>Sandwiches</h2>
‏<div class="item"><span>Chicken Panne</span><span class="price">210</span></div>
‏<div class="item"><span>Chicken Crispy</span><span class="price">210</span></div>
‏<div class="item"><span>Cordon Bleu</span><span class="price">250</span></div>
‏<div class="item"><span>Seafood (Fried)</span><span class="price">250</span></div>
‏<div class="item"><span>Chicken Fajita</span><span class="price">230</span></div>
‏<div class="item"><span>Beef Fajita</span><span class="price">270</span></div>
‏<div class="item"><span>Seafood Fajita</span><span class="price">290</span></div>
‏<div class="item"><span>Cheesy Steak</span><span class="price">310</span></div>
‏</section>

‏<!-- Footer -->
‏<footer style="background:#3e2f1c; color:#f5e1a4; padding:20px; text-align:center;">
‏  <p>Subject to 12% service and 14% taxes</p>
‏  <p>Address: 19, Kamal El Din Salah Street, Smouha - Alexandria</p>
‏  <p>Phone: 034238828 / 01558443147</p>
‏  <p>Email: gossipcafealex@gmail.com</p>
‏</footer>

‏</body>
‏</html>

‏<!-- Footer -->
‏<footer style="background:#5e4632; color:#f5e1a4; padding:30px 20px; text-align:center; margin-top:40px;">
‏  <p style="margin:5px 0;"><strong>Subject to 12% service and 14% taxes</strong></p>
‏  <p style="margin:5px 0;">Address: 19, Kamal El Din Salah Street, Smouha - Alexandria</p>
‏  <p style="margin:5px 0;">Tel: 034238828 | Mobile: 01558443147</p>
‏  <p style="margin:5px 0;">Email: gossipcafealex@gmail.com</p>
‏  <p style="margin:5px 0; font-size:0.9em;">Register No.: 93932 | Tax ID No.: 432589287</p>
‏</footer>

