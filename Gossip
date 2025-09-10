<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>GOSSIP - Menu</title>
<link rel="preconnect" href="https://fonts.gstatic.com">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<style>
  :root{
    --bg:#0f0f11;
    --card:#141414;
    --muted:#bfb8a8;
    --accent:#c8a951;
    --glass: rgba(255,255,255,0.03);
  }
  *{box-sizing:border-box}
  body{
    margin:0;
    font-family: Inter, "Segoe UI", Tahoma, sans-serif;
    background: linear-gradient(180deg,#0b0b0c 0%, #111 60%);
    color:#eee;
    -webkit-font-smoothing:antialiased;
    -moz-osx-font-smoothing:grayscale;
    line-height:1.45;
  }
  

header {
  padding:40px 20px;
  text-align:center;
  border-bottom:1px solid rgba(200,169,81,0.12);
  background: rgba(0,0,0,0.6);
  position: fixed;
  top:0;
  left:0;
  right:0;
  z-index:100;
  transition: transform 0.3s ease, opacity 0.3s ease;
}
header.hidden {
  transform: translateY(-100%);
  opacity: 0;
  pointer-events: none;
}

header.hidden {
  transform: translateY(-100%);
  opacity: 0;
  pointer-events: none;
}

  .brand{
    display:inline-block;
    padding:8px 18px;
    border-radius:8px;
    animation: pop 900ms ease;
  }
  h1{ margin:0; font-size:36px; letter-spacing:2px; color:var(--accent); }
  p.lead{ margin:6px 0 0; color:var(--muted); font-size:14px; letter-spacing:3px; }
  main{ max-width:1100px; margin:30px auto; padding:160px 18px 60px; }
  .grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:18px;
  }
  .section{
    background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    border:1px solid rgba(255,255,255,0.03);
    padding:18px;
    border-radius:12px;
    box-shadow: 0 6px 18px rgba(0,0,0,0.6);
    transform-origin:center;
    overflow:hidden;
  }
  .section h2{
    margin:0 0 8px; color:var(--accent); font-size:18px;
    display:flex; justify-content:space-between; align-items:center;
  }
  .toggle{
    font-size:13px; color:var(--muted); cursor:pointer; background:transparent; border:0;
  }
  ul.list{ list-style:none; padding:0; margin:10px 0 0; max-height:600px; overflow:auto; }
  li.item{
    display:flex; gap:12px; align-items:center; justify-content:space-between;
    padding:10px 12px; border-radius:8px;
    background: linear-gradient(90deg, rgba(255,255,255,0.01), transparent);
    margin-bottom:8px;
    border:1px solid rgba(255,255,255,0.02);
    transition: transform .18s ease, box-shadow .18s ease;
  }
  li.item:hover{ transform: translateY(-6px); box-shadow:0 10px 30px rgba(200,169,81,0.08); }
  .name{ font-weight:600; color:#f5f3ea; }
  .price{ color:var(--accent); font-weight:700; min-width:52px; text-align:right; }
  .muted{ color:var(--muted); font-weight:500; font-size:13px; }
  footer{ margin-top:30px; padding:28px 18px; color:var(--muted); text-align:center; border-top:1px solid rgba(200,169,81,0.06); }
  .badge{ display:inline-block; padding:6px 10px; border-radius:999px; background:var(--glass); color:var(--muted); border:1px solid rgba(255,255,255,0.02); margin-top:6px; }
  
  .quick-icons {
    margin-top: 15px;
    display: flex;
    gap: 20px;
    justify-content: center;
    flex-wrap: wrap;
  }
  .quick-icons a {
    background: var(--glass);
    border: 1px solid rgba(255,255,255,0.08);
    padding: 10px 14px;
    border-radius: 10px;
    color: var(--accent);
    font-weight: 600;
    text-decoration: none;
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 70px;
    transition: transform 0.2s ease, background 0.2s ease;
  }
  .quick-icons a i {
    font-size: 22px;
    margin-bottom: 6px;
  }
  .quick-icons a span {
    font-size: 12px;
  }
  .quick-icons a:hover {
    transform: translateY(-5px);
    background: rgba(200,169,81,0.1);
  }

  
  .side-icons {
    position: fixed;
    top: 50%;
    right: 20px;
    transform: translateY(-50%);
    display: flex;
    flex-direction: column;
    gap: 12px;
    z-index: 200;
  }
  .side-icons a {
    background: var(--glass);
    border: 1px solid rgba(255,255,255,0.08);
    padding: 8px;
    border-radius: 50%;
    color: var(--accent);
    font-size: 18px;
    text-align: center;
    transition: transform 0.2s ease, background 0.2s ease;
  }
  .side-icons a:hover {
    transform: scale(1.2);
    background: rgba(200,169,81,0.1);
  }

  
  .bottom-icons {
    position: fixed;
    bottom: 20px;
    right: 20px;
    display: flex;
    flex-direction: column;
    gap: 12px;
    z-index: 200;
  }
  .bottom-icons a {
    background: var(--glass);
    border: 1px solid rgba(255,255,255,0.08);
    padding: 8px 14px;
    border-radius: 20px;
    color: var(--accent);
    font-size: 14px;
    text-decoration: none;
    display: flex;
    align-items: center;
    gap: 8px;
    transition: transform 0.2s ease, background 0.2s ease;
  }
  .bottom-icons a i {
    font-size: 18px;
  }
  .bottom-icons a:hover {
    transform: translateX(-5px);
    background: rgba(200,169,81,0.1);
  }

  
  .bottom-icons.hidden {
    transform: translateY(150%);
    opacity: 0;
    pointer-events: none;
    transition: transform 0.3s ease, opacity 0.3s ease;
  }

  
  .top-icons {
    position: fixed;
    top: 100px;
    right: 20px;
    display: flex;
    flex-direction: column;
    gap: 12px;
    z-index: 200;
  }
  .top-icons a {
    background: var(--glass);
    border: 1px solid rgba(255,255,255,0.08);
    padding: 8px 14px;
    border-radius: 20px;
    color: var(--accent);
    font-size: 14px;
    text-decoration: none;
    display: flex;
    align-items: center;
    gap: 8px;
    transition: transform 0.2s ease, background 0.2s ease;
  }
  .top-icons a i {
    font-size: 18px;
  }
  .top-icons a:hover {
    transform: translateX(-5px);
    background: rgba(200,169,81,0.1);
  }

  
  header.hidden .lead {
    opacity: 0;
    transform: translateY(-20px);
    transition: opacity 0.3s ease, transform 0.3s ease;
  }

  
  
  .bottom-bar {
    margin: 20px 0;
    padding: 12px 20px;
    background: rgba(0,0,0,0.4);
    border: 1px solid rgba(255,255,255,0.08);
    border-radius: 12px;
    display: flex;
    justify-content: center;
    gap: 24px;
  }
  .bottom-bar a {
    color: var(--accent);
    text-decoration: none;
    font-weight: 600;
    display: flex;
    align-items: center;
    gap: 6px;
    font-size: 14px;
    transition: color 0.2s ease;
  }
  .bottom-bar a i {
    font-size: 18px;
  }
  .bottom-bar a:hover {
    color: #fff;
  }


  
  .brand {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 14px;
  }
  .brand img.logo {
    height: 60px;
    width: auto;
  }

  
  .bottom-bar {
    margin: 20px 0;
    padding: 12px 10px;
    background: rgba(0,0,0,0.4);
    border: 1px solid rgba(255,255,255,0.08);
    border-radius: 12px;
    display: flex;
    gap: 18px;
    overflow-x: auto;
    white-space: nowrap;
  }
  .bottom-bar::-webkit-scrollbar {
    display: none;
  }
  .bottom-bar a {
    color: var(--accent);
    text-decoration: none;
    font-weight: 600;
    display: inline-flex;
    align-items: center;
    gap: 6px;
    font-size: 14px;
    transition: color 0.2s ease;
    padding: 6px 10px;
    border-radius: 8px;
  }
  .bottom-bar a:hover {
    color: #fff;
    background: rgba(200,169,81,0.1);
  }

  /* animations */
  @keyframes pop{ from{ transform: translateY(-10px) scale(.98); opacity:0 } to{ transform:none; opacity:1 } }
  .fade-in{ animation: fadeIn .6s ease both; }
  @keyframes fadeIn{ from{ opacity:0; transform:translateY(8px) } to{ opacity:1; transform:none } }
  /* responsive tweak for narrow screens */
  @media (max-width:520px){
    h1{ font-size:26px }
    .grid{ grid-template-columns: 1fr; }
  }
  /* sticky quick-nav */
  


    position: fixed; right:18px; bottom:18px; z-index:30; display:flex; flex-direction:column; gap:10px;
  }
  .quick a{ background:var(--accent); color:#111; padding:10px 12px; border-radius:8px; text-decoration:none; font-weight:700; box-shadow:0 6px 18px rgba(200,169,81,0.22); }
  /* collapse */
  .collapsed ul.list{ max-height:0; padding:0; margin:0; overflow:hidden; transition: max-height .35s ease; }
  .section .hint{ font-size:12px; color:var(--muted); margin-left:8px; }
</style>
</head>
<body>

<header id="main-header">
  <div class="brand">
    <h1>GOSSIP</h1>
    <p class="lead">LIVE · LAUGH · GOSSIP</p>
  </div>

    

  
</header>


<main>

  
  <nav class="bottom-bar">
    <a href="#hot-drinks">☕ Hot Drinks</a>
    <a href="#iced-drinks">🧊 Iced Drinks</a>
    <a href="#sparkling">✨ Sparkling</a>
    <a href="#cocktails">🍹 Cocktails</a>
    <a href="#fresh-juice">🍊 Fresh Juice</a>
    <a href="#smoothies">🥭 Smoothies</a>
    <a href="#milkshake">🥤 Milk Shake</a>
    <a href="#soft-drinks">🥤 Soft Drinks</a>
    <a href="#breakfast">🍳 Breakfast</a>
    <a href="#appetizers">🥟 Appetizers</a>
    <a href="#soups">🍲 Soups</a>
    <a href="#salads">🥗 Salads</a>
    <a href="#main-chicken">🍗 Chicken</a>
    <a href="#meat">🥩 Meat</a>
    <a href="#seafood">🦐 Seafood</a>
    <a href="#fajitas">🌯 Fajitas</a>
    <a href="#pasta">🍝 Pasta</a>
    <a href="#pizza">🍕 Pizza</a>
    <a href="#burgers">🍔 Burgers</a>
    <a href="#sandwiches">🥪 Sandwiches</a>
    <a href="#dessert">🍰 Dessert</a>
    <a href="#extras">➕ Extras</a>
  </nav>



  

  <div style="display:flex;gap:18px;flex-direction:column;">
    <div class="grid">
      <section class="section fade-in" id="hot-drinks">
        <h2>Hot Drinks <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Espresso</div><div class="price">57</div></li>
          <li class="item"><div class="name">Double Espresso</div><div class="price">75</div></li>
          <li class="item"><div class="name">Macchiato</div><div class="price">75</div></li>
          <li class="item"><div class="name">Double Macchiato</div><div class="price">85</div></li>
          <li class="item"><div class="name">Cappuccino</div><div class="price">105</div></li>
          <li class="item"><div class="name">Latte</div><div class="price">105</div></li>
          <li class="item"><div class="name">Nescafe</div><div class="price">85</div></li>
          <li class="item"><div class="name">Mocha</div><div class="price">115</div></li>
          <li class="item"><div class="name">Hot Chocolate</div><div class="price">100</div></li>
          <li class="item"><div class="name">Nutella Coffee</div><div class="price">100</div></li>
          <li class="item"><div class="name">Lotus Coffee</div><div class="price">110</div></li>
          <li class="item"><div class="name">Flat White</div><div class="price">110</div></li>
          <li class="item"><div class="name">Americano</div><div class="price">100</div></li>
          <li class="item"><div class="name">Turkish Coffee</div><div class="price">52</div></li>
          <li class="item"><div class="name">Double Turkish Coffee</div><div class="price">65</div></li>
          <li class="item"><div class="name">Turkish with Milk</div><div class="price">75</div></li>
          <li class="item"><div class="name">Turkish Hazelnut</div><div class="price">80</div></li>
          <li class="item"><div class="name">Tea</div><div class="price">50</div></li>
          <li class="item"><div class="name">Tea Pot (Zarda)</div><div class="price">90</div></li>
          <li class="item"><div class="name">Flavored Tea</div><div class="price">60</div></li>
          <li class="item"><div class="name">Mixed Herbs</div><div class="price">85</div></li>
          <li class="item"><div class="name">Hot Cider</div><div class="price">85</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="iced-drinks">
        <h2>Iced Drinks <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Iced Chocolate</div><div class="price">115</div></li>
          <li class="item"><div class="name">Iced Espresso</div><div class="price">115</div></li>
          <li class="item"><div class="name">Iced Latte</div><div class="price">115</div></li>
          <li class="item"><div class="name">Iced Mocha</div><div class="price">107</div></li>
          <li class="item"><div class="name">Iced Double Espresso</div><div class="price">120</div></li>
          <li class="item"><div class="name">Iced Nescafe</div><div class="price">105</div></li>
          <li class="item"><div class="name">Iced Tea</div><div class="price">100</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="sparkling">
        <h2>Sparkling Cocktails <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Espresso Red Bull</div><div class="price">155</div></li>
          <li class="item"><div class="name">Cherry Cola</div><div class="price">95</div></li>
          <li class="item"><div class="name">Classic Mojito</div><div class="price">115</div></li>
          <li class="item"><div class="name">Flavored Mojito</div><div class="price">130</div></li>
          <li class="item"><div class="name">Sunshine</div><div class="price">95</div></li>
          <li class="item"><div class="name">Submarine (Red Bull + Peach Topping)</div><div class="price">120</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="cocktails">
        <h2>Cocktails <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Alex Night / Paradise</div><div class="price">130</div></li>
          <li class="item"><div class="name">Kiwi Slash / Blueberry Slash</div><div class="price">122</div></li>
          <li class="item"><div class="name">Fruit Mint</div><div class="price">112</div></li>
        </ul>
      </section>

    </div> <!-- grid first row -->

    <div class="grid">
      <section class="section fade-in" id="fresh-juice">
        <h2>Fresh Juice <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Mango / Strawberry / Pomegranate</div><div class="price">110</div></li>
          <li class="item"><div class="name">Guava / Banana / Watermelon / Kiwi / Orange</div><div class="price">100</div></li>
          <li class="item"><div class="name">Lemon</div><div class="price">90</div></li>
          <li class="item"><div class="name">Mint Lemon</div><div class="price">95</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="smoothies">
        <h2>Smoothies <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Mixed Fruits (Mango, Strawberry, Lemon, Banana, Guava, Kiwi, Watermelon, Pomegranate)</div><div class="price">116</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="milkshake">
        <h2>Milk Shake <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Oreo / Kiwi</div><div class="price">140</div></li>
          <li class="item"><div class="name">Mango / Strawberry</div><div class="price">140</div></li>
          <li class="item"><div class="name">Vanilla / Chocolate</div><div class="price">140</div></li>
          <li class="item"><div class="name">Nutella</div><div class="price">155</div></li>
          <li class="item"><div class="name">Lotus / Pistachio</div><div class="price">155</div></li>
        </ul>
      </section>
    </div> <!-- grid second row -->

    <div class="grid">
      <section class="section fade-in" id="soft-drinks">
        <h2>Soft Drinks <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Water Small</div><div class="price">-</div></li>
          <li class="item"><div class="name">Water Large</div><div class="price">-</div></li>
          <li class="item"><div class="name">Cola / Sprite / Fanta</div><div class="price">-</div></li>
          <li class="item"><div class="name">Fayrouz / Birell / Schweppes</div><div class="price">-</div></li>
          <li class="item"><div class="name">Red Bull</div><div class="price">-</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="breakfast">
        <h2>Breakfast <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Standard Breakfast</div><div class="price">350</div></li>
          <li class="item"><div class="name">Extras</div><div class="price">60</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="appetizers">
        <h2>Appetizers <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Mozzarella Sticks (5 Pieces)</div><div class="price">120</div></li>
          <li class="item"><div class="name">French Fries</div><div class="price">60</div></li>
          <li class="item"><div class="name">Homemade Chips</div><div class="price">60</div></li>
          <li class="item"><div class="name">Chicken Strips (5 Pieces)</div><div class="price">150</div></li>
          <li class="item"><div class="name">Chicken Wings (6 Pieces)</div><div class="price">135</div></li>
          <li class="item"><div class="name">Fried Shrimps</div><div class="price">190</div></li>
          <li class="item"><div class="name">Shrimp Cocktail</div><div class="price">200</div></li>
          <li class="item"><div class="name">Calamari</div><div class="price">-</div></li>
          <li class="item"><div class="name">Oriental Sausages</div><div class="price">-</div></li>
          <li class="item"><div class="name">White Cheese & Tomatoes</div><div class="price">80</div></li>
          <li class="item"><div class="name">Carrots & Cucumber Slices</div><div class="price">50</div></li>
          <li class="item"><div class="name">Tehina</div><div class="price">60</div></li>
          <li class="item"><div class="name">Pickles</div><div class="price">40</div></li>
        </ul>
      </section>
    </div> <!-- grid third row -->

    <div class="grid">
      <section class="section fade-in" id="soups">
        <h2>Soups <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Seasonal Soup</div><div class="price">110</div></li>
          <li class="item"><div class="name">Molokheya</div><div class="price">90</div></li>
          <li class="item"><div class="name">Seafood Soup</div><div class="price">220</div></li>
          <li class="item"><div class="name">Chicken Cream</div><div class="price">150</div></li>
          <li class="item"><div class="name">Mushroom Soup</div><div class="price">130</div></li>
          <li class="item"><div class="name">Onion Soup</div><div class="price">140</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="salads">
        <h2>Salads <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Shrimp Caesar Salad</div><div class="price">210</div></li>
          <li class="item"><div class="name">Chicken Caesar Salad</div><div class="price">160</div></li>
          <li class="item"><div class="name">Greek Salad</div><div class="price">210</div></li>
          <li class="item"><div class="name">Tuna Salad</div><div class="price">210</div></li>
          <li class="item"><div class="name">Rocca Salad</div><div class="price">210</div></li>
          <li class="item"><div class="name">Gossip Salad</div><div class="price">240</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="main-chicken">
        <h2>Main Courses - Chicken <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Shredded Mexican Chicken</div><div class="price">290</div></li>
          <li class="item"><div class="name">Chicken Curry</div><div class="price">290</div></li>
          <li class="item"><div class="name">Chicken Panne</div><div class="price">290</div></li>
          <li class="item"><div class="name">Crispy Chicken</div><div class="price">320</div></li>
          <li class="item"><div class="name">Grilled Chicken with Lemon Sauce</div><div class="price">330</div></li>
          <li class="item"><div class="name">Grilled Chicken with Mushroom Sauce</div><div class="price">350</div></li>
          <li class="item"><div class="name">Chicken Cordon Bleu</div><div class="price">310</div></li>
          <li class="item"><div class="name">Chicken Cacciatore</div><div class="price">360</div></li>
          <li class="item"><div class="name">Chicken Gossip</div><div class="price">-</div></li>
        </ul>
      </section>
    </div> <!-- grid fourth row -->

    <div class="grid">
      <section class="section fade-in" id="meat">
        <h2>Meat <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Beef Stroganoff</div><div class="price">450</div></li>
          <li class="item"><div class="name">Beef Fillet (Mushroom / Garlic / Pepper)</div><div class="price">580</div></li>
          <li class="item"><div class="name">Surf & Turf</div><div class="price">610</div></li>
          <li class="item"><div class="name">Mixed Grill</div><div class="price">550</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="seafood">
        <h2>Seafood <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Mixed Seafood Platter</div><div class="price">520</div></li>
          <li class="item"><div class="name">Jumbo Shrimps (8 pcs)</div><div class="price">590</div></li>
          <li class="item"><div class="name">Salmon Fillet Lemon & Butter</div><div class="price">680</div></li>
          <li class="item"><div class="name">Fish and Chips</div><div class="price">340</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="fajitas">
        <h2>Fajitas <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Chicken Fajita</div><div class="price">360</div></li>
          <li class="item"><div class="name">Beef Fajita</div><div class="price">430</div></li>
          <li class="item"><div class="name">Shrimp Fajita</div><div class="price">490</div></li>
        </ul>
      </section>
    </div> <!-- grid fifth row -->

    <div class="grid">
      <section class="section fade-in" id="pasta">
        <h2>Pasta <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Arabiata</div><div class="price">165</div></li>
          <li class="item"><div class="name">Alfredo</div><div class="price">210</div></li>
          <li class="item"><div class="name">Bolognese</div><div class="price">210</div></li>
          <li class="item"><div class="name">Negresco</div><div class="price">250</div></li>
          <li class="item"><div class="name">Crispy Chicken Pasta</div><div class="price">210</div></li>
          <li class="item"><div class="name">Seafood Pasta</div><div class="price">290</div></li>
          <li class="item"><div class="name">Chicken Pesto</div><div class="price">240</div></li>
          <li class="item"><div class="name">Mac & Cheese</div><div class="price">220</div></li>
          <li class="item"><div class="name">Mushroom Pasta</div><div class="price">190</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="pizza">
        <h2>Pizza <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Pizza Margherita</div><div class="price">200</div></li>
          <li class="item"><div class="name">Pizza Vegetarian</div><div class="price">200</div></li>
          <li class="item"><div class="name">Pizza Chicken (BBQ / Ranch)</div><div class="price">240</div></li>
          <li class="item"><div class="name">Pizza Oriental Sausage</div><div class="price">250</div></li>
          <li class="item"><div class="name">Pizza Tuna</div><div class="price">250</div></li>
          <li class="item"><div class="name">Pizza Seafood</div><div class="price">290</div></li>
          <li class="item"><div class="name">Pizza Salami</div><div class="price">250</div></li>
          <li class="item"><div class="name">Pizza Anchovies</div><div class="price">290</div></li>
          <li class="item"><div class="name">Pizza Mixed Beef</div><div class="price">300</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="burgers">
        <h2>Burgers <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Classic Burger (200g)</div><div class="price">280</div></li>
          <li class="item"><div class="name">Cheese Burger (200g)</div><div class="price">300</div></li>
          <li class="item"><div class="name">Mushroom Burger (200g)</div><div class="price">310</div></li>
          <li class="item"><div class="name">Gossip Burger (200g)</div><div class="price">340</div></li>
        </ul>
      </section>
    </div> <!-- grid sixth row -->

    <div class="grid">
      <section class="section fade-in" id="sandwiches">
        <h2>Sandwiches <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Chicken Panne</div><div class="price">210</div></li>
          <li class="item"><div class="name">Chicken Crispy</div><div class="price">210</div></li>
          <li class="item"><div class="name">Cordon Bleu</div><div class="price">250</div></li>
          <li class="item"><div class="name">Seafood (Fried)</div><div class="price">250</div></li>
          <li class="item"><div class="name">Chicken Fajita</div><div class="price">230</div></li>
          <li class="item"><div class="name">Beef Fajita</div><div class="price">270</div></li>
          <li class="item"><div class="name">Seafood Fajita</div><div class="price">290</div></li>
          <li class="item"><div class="name">Cheesy Steak</div><div class="price">310</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="dessert">
        <h2>Dessert <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Molten Cake</div><div class="price">140</div></li>
          <li class="item"><div class="name">Brownies</div><div class="price">120</div></li>
          <li class="item"><div class="name">Oreo Madness</div><div class="price">175</div></li>
          <li class="item"><div class="name">Om Aly with Nuts</div><div class="price">165</div></li>
          <li class="item"><div class="name">Classic Ice Cream (3 scoops)</div><div class="price">140</div></li>
          <li class="item"><div class="name">Waffle (Nutella, Lotus, Fruit, Caramel)</div><div class="price">150</div></li>
          <li class="item"><div class="name">Fruit Salad</div><div class="price">150</div></li>
        </ul>
      </section>

      <section class="section fade-in" id="extras">
        <h2>Extras & Shishah <button class="toggle" onclick="toggleCollapse(this)">Toggle</button></h2>
        <ul class="list">
          <li class="item"><div class="name">Ice Cream (extra)</div><div class="price">50</div></li>
          <li class="item"><div class="name">Nuts</div><div class="price">50</div></li>
          <li class="item"><div class="name">Flavors</div><div class="price">50</div></li>
          <li class="item"><div class="name">Nutella (extra)</div><div class="price">50</div></li>
          <li class="item"><div class="name">Shishah - Meassel (2 coals)</div><div class="price">250</div></li>
          <li class="item"><div class="name">Shishah Flavors (premium)</div><div class="price">275</div></li>
          <li class="item"><div class="name">Pyrex Glass</div><div class="price">295</div></li>
        </ul>
      </section>
    </div> <!-- last row -->

  </div>

  

  

</main>

<footer>
  <div class="badge">Register No.: 93932 · Tax ID: 432589287</div>
  <p>Subject to 12% service and 14% taxes</p>
  <p>Address: 19, Kamal El Din Salah Street, Smouha - Alexandria</p>
  <p>Tel: 03 4238828 · Mob: 01558443147 · Email: gossipcafealex@gmail.com</p>
</footer>

<script>
  

// hide header on scroll (with hidden class)
let lastScroll = 0;
const header = document.querySelector('header');
window.addEventListener('scroll', () => {
  const currentScroll = window.pageYOffset;
  if (currentScroll > lastScroll && currentScroll > 50) {
    header.classList.add('hidden');
  } else {
    header.classList.remove('hidden');
  }
  lastScroll = currentScroll;
});

  


// hide header on scroll (with hidden class)
let lastScroll = 0;
const header = document.querySelector('header');
window.addEventListener('scroll', () => {
  const currentScroll = window.pageYOffset;
  if (currentScroll > lastScroll && currentScroll > 50) {
    header.classList.add('hidden');
  } else {
    header.classList.remove('hidden');
  }
  lastScroll = currentScroll;
});

  // simple collapse toggle for sections
  function toggleCollapse(btn){
    const section = btn.closest('.section');
    section.classList.toggle('collapsed');
    const list = section.querySelector('.list');
    if(section.classList.contains('collapsed')){
      list.style.maxHeight = '0px';
      btn.textContent = 'Show';
    } else {
      list.style.maxHeight = list.scrollHeight + 'px';
      btn.textContent = 'Hide';
    }
  }
  // ensure initial heights
  document.querySelectorAll('.section').forEach(s=>{
    const list = s.querySelector('.list');
    list.style.maxHeight = list.scrollHeight + 'px';
  });

  // small entrance animation stagger
  window.addEventListener('load', ()=>{
    document.querySelectorAll('.fade-in').forEach((el,i)=>{
      el.style.animationDelay = (i*80) + 'ms';
    });
  });
</script>










</body>
</html>
