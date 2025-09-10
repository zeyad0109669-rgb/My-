<!doctype html>
<html lang="ar">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>GOSSIP — Menu</title>
<style>
:root{
  --brown:#6B3E26;
  --gold:#D4AF37;
  --bg:#fff8f0;
  --card:#fffdfb;
  --muted:#8a6b5a;
  --radius:10px;
}
*{box-sizing:border-box}
body{margin:0;font-family: "Segoe UI", Roboto, "Helvetica Neue", Arial; background:var(--bg); color:var(--brown); -webkit-font-smoothing:antialiased;}
.header{
  background:linear-gradient(90deg,var(--brown), #4f2c1d);
  color:var(--gold);
  padding:22px 16px;
  text-align:center;
  position:sticky;top:0;z-index:50;
  box-shadow:0 2px 8px rgba(0,0,0,0.08);
}
.header h1{margin:0;font-size:20px;letter-spacing:2px}
.header p{margin:6px 0 0;font-size:13px;color:rgba(212,175,55,0.95)}
.container{display:flex;gap:20px;padding:18px;max-width:1200px;margin:18px auto;}
.sidebar{
  width:220px;background:linear-gradient(180deg, rgba(255,255,255,0.7), rgba(255,255,255,0.9));
  border-radius:var(--radius); padding:12px; box-shadow:0 6px 18px rgba(107,62,38,0.06);
  height:calc(100vh - 120px); position:sticky; top:70px; overflow:auto;
}
.logo-mini{display:flex;gap:10px;align-items:center;margin-bottom:12px}
.logo-circle{width:46px;height:46px;border-radius:10px;background:var(--gold);display:flex;align-items:center;justify-content:center;color:var(--brown);font-weight:700}
.search{margin-bottom:12px}
.search input{
  width:100%;padding:10px;border-radius:8px;border:1px solid rgba(107,62,38,0.12);
  font-size:14px;background:#fff;
}
.section-links{display:flex;flex-direction:column;gap:6px}
.section-links a{
  display:flex;align-items:center;gap:8px;padding:8px;border-radius:8px;color:var(--brown);text-decoration:none;
  font-weight:600;font-size:14px;border-left:3px solid transparent; transition:all .18s;
}
.section-links a:hover{background:rgba(212,175,55,0.08);transform:translateX(4px);border-left-color:var(--gold)}
.main{flex:1;min-width:0}
.top-actions{display:flex;gap:12px;align-items:center;justify-content:space-between;margin-bottom:12px}
.top-actions .note{color:var(--muted);font-size:13px}
.grid{display:grid;grid-template-columns:repeat(2,1fr);gap:14px}
@media(max-width:900px){.container{padding:12px}.sidebar{display:none}.grid{grid-template-columns:1fr}}
.card{background:var(--card);border-radius:12px;padding:12px;box-shadow:0 6px 18px rgba(107,62,38,0.06);overflow:hidden;opacity:0;transform:translateY(10px);animation:fadeIn .5s forwards}
@keyframes fadeIn{to{opacity:1;transform:none}}
.section-title{display:flex;align-items:center;gap:10px;margin:6px 0 10px}
.section-title h2{margin:0;color:var(--gold);font-size:18px;letter-spacing:1px}
.items{display:flex;flex-direction:column;gap:8px}
.item{
  display:flex;gap:12px;align-items:center;padding:10px;border-radius:10px;border:1px solid rgba(107,62,38,0.04);
  transition:transform .18s, box-shadow .18s, background .18s; background:linear-gradient(180deg,#fff,#fffdf8);
}
.item:hover{transform:translateY(-4px);box-shadow:0 8px 18px rgba(107,62,38,0.08);background:linear-gradient(180deg,#fff,#fff8f0)}
.thumb{
  width:78px;height:62px;border-radius:8px;flex-shrink:0;display:flex;align-items:center;justify-content:center;
  background:linear-gradient(135deg,var(--gold),#f4e1a6); color:var(--brown); font-weight:700;box-shadow:inset 0 -6px 12px rgba(0,0,0,0.04);
  cursor:pointer;transition:transform .12s;
}
.thumb svg{width:48px;height:48px}
.item-info{flex:1;min-width:0}
.item-info .title{display:flex;justify-content:space-between;gap:12px;align-items:flex-start}
.item-info .names{min-width:0}
.title .eng{font-weight:700;color:var(--brown)}
.title .arb{font-size:13px;color:var(--muted);margin-top:4px}
.price{font-weight:800;color:var(--brown);background:linear-gradient(90deg, rgba(212,175,55,0.12), transparent);padding:6px 10px;border-radius:8px}
.badge{font-size:12px;padding:4px 8px;border-radius:8px;background:rgba(107,62,38,0.06);color:var(--muted);margin-left:8px}
.controls{display:flex;gap:8px;align-items:center}
.btn{
  background:transparent;border:1px solid rgba(107,62,38,0.08);padding:8px 10px;border-radius:8px;font-weight:600;cursor:pointer;
}
.btn.primary{background:var(--gold);border-color:rgba(212,175,55,0.4);color:var(--brown)}
.modal{position:fixed;inset:0;background:rgba(0,0,0,0.6);display:flex;align-items:center;justify-content:center;z-index:120;opacity:0;pointer-events:none;transition:opacity .18s}
.modal.open{opacity:1;pointer-events:auto}
.modal .box{background:#fff;padding:16px;border-radius:12px;max-width:720px;width:92%;max-height:90vh;overflow:auto}
.modal img{max-width:100%;border-radius:8px;display:block}
.topline{display:flex;gap:10px;align-items:center;justify-content:space-between;margin-bottom:8px}
.small-muted{font-size:12px;color:var(--muted)}
.footer{margin-top:18px;padding:12px;background:linear-gradient(180deg,#fff,#fffefc);border-radius:12px;font-size:13px;color:var(--muted)}
/* collapsible */
.collapse{cursor:pointer;display:flex;align-items:center;gap:8px;padding:8px;border-radius:8px}
.collapse .arrow{transition:transform .18s}
.collapse.collapsed .arrow{transform:rotate(-90deg)}
/* small screens */
@media(max-width:520px){
  .header h1{font-size:18px}
  .grid{grid-template-columns:1fr}
  .thumb{width:60px;height:50px}
  .container{padding:10px}
}
</style>
</head>
<body>

<div class="header">
  <h1>GOSSIP — LIVE LAUGH GOSSIP</h1>
  <p>Register No.: 93932 • Tax ID No.: 432589287</p>
</div>

<div class="container">

  <aside class="sidebar" aria-label="Menu sections">
    <div class="logo-mini">
      <div class="logo-circle">G</div>
      <div>
        <div style="font-weight:700">GOSSIP</div>
        <div style="font-size:12px;color:var(--muted)">Cafe & Restaurant</div>
      </div>
    </div>

    <div class="search">
      <input id="search" placeholder="ابحث عن صنف أو سعر..." aria-label="search">
    </div>

    <div class="section-links" id="toc">
      <!-- links injected by JS for exact ordering -->
    </div>

    <div style="margin-top:14px" class="small-muted">
      <div>Address: 19, Kamal El Din Salah Street, Smouha - Alexandria</div>
      <div>Tel: 034238828 / 01558443147</div>
      <div style="margin-top:8px">Subject to 12% service and 14% taxes</div>
    </div>
  </aside>

  <main class="main">
    <div class="top-actions">
      <div class="note">قائمة الطعام كاملة وتفاعلية — المسح بالبحث سريعاً أو استخدم روابط الأقسام على اليسار</div>
      <div class="controls">
        <button class="btn" id="toggleAll">طي/توسيع الكل</button>
        <button class="btn primary" id="downloadPdf">حفظ كـ PDF</button>
      </div>
    </div>

    <!-- menu sections container -->
    <div id="menuSections" class="grid">
      <!-- sections injected by JS -->
    </div>

    <div class="footer">
      <strong>GOSSIP</strong> — LIVE LAUGH GOSSIP<br>
      Email: gossipcafealex@gmail.com  • Register No.: 93932 • Tax ID: 432589287
    </div>
  </main>

</div>

<!-- modal for images/details -->
<div id="modal" class="modal" role="dialog" aria-modal="true" aria-hidden="true">
  <div class="box">
    <div class="topline">
      <div><strong id="modalTitle">Title</strong><div id="modalSub" class="small-muted"></div></div>
      <div><button class="btn" id="closeModal">Close</button></div>
    </div>
    <img id="modalImg" alt="">
    <div id="modalDesc" style="margin-top:10px;color:var(--muted)"></div>
  </div>
</div>

<script>
/* ---------- data: full menu (from user's messages) ---------- */
/* Each section: id, titleEn, titleAr, items: {eng, arb, price, short (desc), imgSVG(optional)} */
const menuData = [
  {
    id:"hot-drinks", titleEn:"Hot Drinks", titleAr:"المشروبات الساخنة",
    items:[
      {eng:"Espresso", arb:"إسبريسو", price:"57"},
      {eng:"Double Espresso", arb:"إسبريسو دبيل", price:"75"},
      {eng:"Macchiato", arb:"كياتو", price:"75"},
      {eng:"Double Macchiato", arb:"كياتو دبل", price:"85"},
      {eng:"Cappuccino", arb:"كابتشينو", price:"105"},
      {eng:"Latté", arb:"لاتي", price:"105"},
      {eng:"Nescafe", arb:"نسكافيه", price:"85"},
      {eng:"Mocha", arb:"موك", price:"115"},
      {eng:"Hot Chocolate", arb:"هوت شوكليت", price:"100"},
      {eng:"Nutella coffee", arb:"قهوة نوتيلا", price:"100"},
      {eng:"Lotus coffee", arb:"قهوة لوتس", price:"110"},
      {eng:"Flat White", arb:"فلات وايت", price:"110"},
      {eng:"Americano", arb:"أمريكانو", price:"100"},
      {eng:"Turkish Coffee", arb:"قهوة تركي", price:"52"},
      {eng:"Double Turkish Coffee", arb:"قهوة تركي دبل", price:"65"},
      {eng:"Turkish with Milk", arb:"قهوة تركي باللبن", price:"75"},
      {eng:"Turkish Hazelnut", arb:"قهوة تركي بندق", price:"80"},
      {eng:"Tea", arb:"شاي", price:"50"},
      {eng:"Tea Pot (Zarda)", arb:"شاي نكهات", price:"90"},
      {eng:"Flavored Tea", arb:"ميكس اعشاب", price:"60"},
      {eng:"Mixed Herbs", arb:"ميكس اعشاب", price:"85"},
      {eng:"Hot Cider", arb:"هوت سيدر", price:"85"},
      {eng:"Frappé", arb:"فرابيه", price:"115", short:"Caramel, Vanilla, Cinnamon, Hazelnut"},
      {eng:"Mocha (Frappé)", arb:"موك", price:"125"},
      {eng:"Lotus (Frappé)", arb:"لوتس", price:"140"}
    ]
  },

  {
    id:"iced-drinks", titleEn:"Iced Drinks", titleAr:"المشروبات المثلجة",
    items:[
      {eng:"Iced Chocolate", arb:"ايس شوكليت", price:"115"},
      {eng:"Iced Espresso", arb:"ايس إسبريسو", price:"115"},
      {eng:"Iced Latté", arb:"ايس لاتيه", price:"115"},
      {eng:"Iced Mocha", arb:"ايس موك", price:"107"},
      {eng:"Iced Double Espresso", arb:"ايس دبل إسبريسو", price:"120"},
      {eng:"Iced Nescafe", arb:"ايس نسكافية", price:"105"},
      {eng:"Iced Tea", arb:"شاى مثلج", price:"100"}
    ]
  },

  {
    id:"sparkling", titleEn:"Sparkling Cocktails", titleAr:"كوكتيلات فواره",
    items:[
      {eng:"Espresso Red Bull", arb:"إسيريسو ريديول", price:"155"},
      {eng:"Cherry cola", arb:"شيري كولا", price:"95"},
      {eng:"Classic Mojito", arb:"موخيتو كلاسيك", price:"115"},
      {eng:"Flavored Mojito", arb:"موخيتو نكهات", price:"130"},
      {eng:"Sunshine", arb:"صن شاين", price:"95"},
      {eng:"Submarine (Redbull + Peach)", arb:"صب مارين", price:"120"}
    ]
  },

  {
    id:"cocktails", titleEn:"Cocktails", titleAr:"كوكتيلات",
    items:[
      {eng:"Alex Night, Paradise", arb:"اليكس نايت، باراديس", price:"130"},
      {eng:"Kiwi Slash, Blueberry Slash", arb:"كيوي سلاش، بلوبيري سلاش", price:"122"},
      {eng:"Fruit Mint", arb:"فواكه بالنعناع", price:"112"}
    ]
  },

  {
    id:"fresh-juice", titleEn:"Fresh Juice", titleAr:"عصائر فريش",
    items:[
      {eng:"Mango, Strawberry, Pomegranate", arb:"مانجو، فراولة، رمان", price:"110"},
      {eng:"Guava, Banana, Watermelon, kiwi, orange", arb:"جوافة، موز، بطيخ، كيوي، برتقال", price:"100"},
      {eng:"Lemon", arb:"ليمون", price:"90"},
      {eng:"Mint Lemon", arb:"ليمون نعناع", price:"95"}
    ]
  },

  {
    id:"smoothies", titleEn:"Smoothies", titleAr:"Smoothies",
    items:[
      {eng:"Mango, Strawberry, Lemon, Banana, Guava, kiwi, Watermelon, Pomegranate", arb:"مانجو، فراولة، ليمون، موز، جوافة، كيوي، بطيخ، رمان", price:"116"}
    ]
  },

  {
    id:"milkshakes", titleEn:"Milk Shake", titleAr:"ميلك شيك",
    items:[
      {eng:"Oreo, Kiwi, Mango, Strawberry, Vanilla, Chocolate", arb:"اوريو، كيوي، مانجو، فراولة، فانيلا، شوكليت", price:"140"},
      {eng:"Nutella", arb:"نوتيلا", price:"155"},
      {eng:"Lotus, Pistachio", arb:"لوتس، فسدق", price:"155"}
    ]
  },

  {
    id:"soft-drinks", titleEn:"Soft Drink", titleAr:"مشروبات غازيه",
    items:[
      {eng:"Water Small", arb:"مياه معدنيه صغيرة", price:"25"},
      {eng:"Water Large", arb:"مياه معدنيه كبيرة", price:"50"},
      {eng:"Cola, Sprite, Fanta", arb:"كوكاكولا.فانتا.سبرايت", price:"55"},
      {eng:"Fayrouz, Birell, Schweppes", arb:"فيروز.بيريل شوبيس", price:"65"},
      {eng:"Red Bull", arb:"ريديول", price:"130"}
    ]
  },

  {
    id:"breakfast", titleEn:"Breakfast", titleAr:"وجبة الافطار",
    items:[
      {eng:"Standard breakfast", arb:"معيارى", price:"350"},
      {eng:"Extras", arb:"اضافات", price:"60"}
    ]
  },

  {
    id:"appetizers", titleEn:"Appetizers", titleAr:"المقبلات",
    items:[
      {eng:"Mozzarella sticks (5 Pieces)", arb:"اصابع موتزاريلا (٥ قطع)", price:"120"},
      {eng:"French fries", arb:"فرانش فرايز", price:"60"},
      {eng:"Homemade chips", arb:"بطاطس مقلية شيبس", price:"60"},
      {eng:"Chicken strips (5 Pieces)", arb:"تشيكن ستربس (٥ قطع)", price:"150"},
      {eng:"Chicken wings (6 Pieces)", arb:"اجنحة الدجاج (٦ قطع)", price:"135"},
      {eng:"Fried shrimps", arb:"جمبري مقلى", price:"190"},
      {eng:"Shrimp cocktail", arb:"كوكتيل جمبري", price:"200"},
      {eng:"Calamari", arb:"كالماري", price:"--"},
      {eng:"Oriental sausages (Local Meat)", arb:"سجق بلدي", price:"170"},
      {eng:"White Cheese and tomatoes", arb:"جبنة بالطماطم", price:"80"},
      {eng:"Carrots & Cucumber slices", arb:"شرائح جزر و خيار", price:"50"},
      {eng:"Tehina", arb:"طحينة", price:"60"},
      {eng:"Pickles", arb:"مخلل", price:"40"}
    ]
  },

  {
    id:"soups", titleEn:"Soups", titleAr:"الشوربة",
    items:[
      {eng:"Seasonal Soup", arb:"شوربة موسمية", price:"110"},
      {eng:"Molokheya", arb:"ملوخية", price:"90"},
      {eng:"Seafood", arb:"سي فود", price:"220"},
      {eng:"Chicken Cream", arb:"كريمة الدجاج", price:"150"},
      {eng:"Mushroom", arb:"مشروم", price:"130"},
      {eng:"Onion", arb:"بصل", price:"140"}
    ]
  },

  {
    id:"salads", titleEn:"Salads", titleAr:"السلطات",
    items:[
      {eng:"Shrimp Caesar Salad", arb:"سلطة السيزر بالجمبري", price:"300", short:"Grilled shrimps, vegetables and cheese topping"},
      {eng:"Chicken Caesar Salad", arb:"سلطة السيزر بالدجاج", price:"210", short:"Grilled chicken, vegetables and cheese topping"},
      {eng:"Greek Salad", arb:"سلطة يونانية", price:"210", short:"Vegetables and white cheese"},
      {eng:"Tuna Salad", arb:"سلطة تونا", price:"210", short:"Tuna marinated in special sauce with vegetables"},
      {eng:"Rocca Salad", arb:"سلطة الجرجير (روكا)", price:"240", short:"Rocca, walnut, vinaigrette sauce and olive oil"},
      {eng:"Gossip Salad", arb:"سلطة جوسيب", price:"300", short:"Caramelized walnut, onion, red beans, corn and apple"}
    ]
  },

  {
    id:"main-courses", titleEn:"Main Courses", titleAr:"الاطباق الرئيسية",
    items:[
      {eng:"Shredded Mexican Chicken", arb:"قطع دجاج بصوص مكسيكان", price:"290"},
      {eng:"Chicken Curry", arb:"دجاج كاري", price:"290"},
      {eng:"Chicken Panne", arb:"دجاج بانيه", price:"290"},
      {eng:"Crispy Chicken", arb:"دجاج كريسبي", price:"320"},
      {eng:"Grilled Chicken with Lemon Sauce", arb:"دجاج مشوي بصوص الليمون", price:"330"},
      {eng:"Grilled Chicken with Mushroom Sauce", arb:"دجاج مشوي بصوص كريم المشروم", price:"350"},
      {eng:"Chicken Cordon Bleu", arb:"كوردون بلو", price:"310"},
      {eng:"Chicken Cacciatore", arb:"دجاج كاتشاتوري", price:"360"},
      {eng:"Chicken Gossip", arb:"دجاج جوسيب", price:"300", short:"Two pieces with béchamel & mozzarella"},
      {eng:"All plates served with 2 sides or pasta", arb:"جميع الاطباق تقدم مع اختياركم من صنفين", price:""}
    ]
  },

  {
    id:"meat-seafood", titleEn:"Meat & Seafood", titleAr:"اللحم و السي فود",
    items:[
      {eng:"Beef Stroganoff", arb:"بيف ستراجانوف", price:"450"},
      {eng:"Beef Fillet (Mushroom/Garlic/Pepper)", arb:"فيليه لحم (مشروم/ ثوم/ فلفل اسود)", price:"580"},
      {eng:"Surf & Turf", arb:"لحم بالجمبري سيرف اند تيرف", price:"610"},
      {eng:"Mixed Grill", arb:"ميكس جريل", price:"550"},
      {eng:"Mixed Seafood Platter", arb:"طبق سي فود مشكل", price:"520"},
      {eng:"Jumbo Shrimps (8 pcs)", arb:"جمبري جامبو (٨ قطع)", price:"590"},
      {eng:"Salmon Fillet Lemon and Butter Sauce", arb:"فيليه سالمون", price:"680"},
      {eng:"Fish and Chips", arb:"فيش اند شيبس", price:"340"}
    ]
  },

  {
    id:"fajitas", titleEn:"Fajitas", titleAr:"فاهيت",
    items:[
      {eng:"Chicken Fajita", arb:"دجاج", price:"360", short:"Striped grilled chicken, Mexican style"},
      {eng:"Beef Fajita", arb:"لحم", price:"430"},
      {eng:"Shrimp Fajita", arb:"جمبري", price:"490"}
    ]
  },

  {
    id:"pasta", titleEn:"Pasta", titleAr:"المكرونيات",
    items:[
      {eng:"Arabiata (Olive, bell pepper in red spicy sauce)", arb:"اربياتا", price:"165"},
      {eng:"Alfredo (Chicken in white sauce with herbs)", arb:"الفريدو", price:"210"},
      {eng:"Bolognese (Local meat marinated in red sauce)", arb:"بولونيز", price:"210"},
      {eng:"Negresco (Chicken & mushroom, oven baked mozzarella)", arb:"نجر سكو", price:"250"},
      {eng:"Crispy chicken (white sauce)", arb:"دجاج كريسبي", price:"210"},
      {eng:"Seafood (Shrimps and calamari)", arb:"سي فود", price:"290"},
      {eng:"Chicken Pesto (Pesto sauce with walnuts & olives)", arb:"دجاج بالريحان", price:"240"},
      {eng:"Mac Cheese", arb:"ماك تشيز", price:"220"},
      {eng:"Mushroom (White mushroom with creamy sauce)", arb:"شروم", price:"190"}
    ]
  },

  {
    id:"pizza", titleEn:"Pizza", titleAr:"البيتزا",
    items:[
      {eng:"Pizza Margherita", arb:"بيتزا مارجريتا", price:"200"},
      {eng:"Pizza Vegetarian", arb:"بيتزا خضروات", price:"200"},
      {eng:"Pizza Chicken (BBQ - Ranch)", arb:"بيتزا دجاج (بربكيو - رانش)", price:"240"},
      {eng:"Pizza Oriental Sausage", arb:"بيتزا سجق", price:"250"},
      {eng:"Pizza Tuna", arb:"بيتزا تونة", price:"250"},
      {eng:"Pizza Seafood", arb:"بيتزا سي فود", price:"290"},
      {eng:"Pizza Salami", arb:"بيتزا سلامى", price:"250"},
      {eng:"Pizza Anchovies", arb:"بيتزا انشوجة", price:"290"},
      {eng:"Pizza Mixed Beef", arb:"بيتزا مشكل لحوم", price:"300"}
    ]
  },

  {
    id:"burgers", titleEn:"Burger Sandwiches", titleAr:"سندويتشات البرجر",
    items:[
      {eng:"Classic Burger (200g)", arb:"برجر كلاسيك", price:"280"},
      {eng:"Cheese Burger", arb:"برجر بالجبنة", price:"300"},
      {eng:"Mushroom Burger", arb:"برجر مشروم", price:"310"},
      {eng:"Gossip Burger", arb:"برجر جوسيب", price:"340"}
    ]
  },

  {
    id:"sandwiches", titleEn:"Sandwiches", titleAr:"السندويتشات",
    items:[
      {eng:"Chicken Panne", arb:"دجاج بانية", price:"210"},
      {eng:"Chicken Crispy", arb:"دجاج كرسبى", price:"210"},
      {eng:"Cordon Bleu", arb:"كوردن بلو", price:"250"},
      {eng:"Seafood (Fried)", arb:"سي فود (مقلى)", price:"250"},
      {eng:"Chicken Fajita", arb:"فاهيتا الدجاج", price:"230"},
      {eng:"Beef Fajita", arb:"فاهيتا لحم", price:"270"},
      {eng:"Seafood Fajita", arb:"فاهيتا سى فود", price:"290"},
      {eng:"Cheesy Steak", arb:"ستيك بالجبنة", price:"310"}
    ]
  },

  {
    id:"dessert", titleEn:"Dessert", titleAr:"الديزيرت",
    items:[
      {eng:"Molten Cake", arb:"مولتن كيك", price:"140"},
      {eng:"Brownies", arb:"براونيز", price:"120"},
      {eng:"Oreo Madness", arb:"اوريو مادنس", price:"175"},
      {eng:"Om Aly with Nuts", arb:"ام علي بالمكسرات", price:"165"},
      {eng:"Classic Ice Cream (3 scoops)", arb:"ايس كريم كلاسيك (٣ بولة)", price:"140"},
      {eng:"Waffle (Nutella, Lotus, Fruit, Caramel)", arb:"وافل (نوتيلا لوتس فواكه.كراميل)", price:"150"},
      {eng:"Fruit Salad", arb:"فروت سلاد", price:"150"}
    ]
  },

  {
    id:"extras", titleEn:"Extras", titleAr:"الاضافات",
    items:[
      {eng:"Ice Cream", arb:"ايس كريم", price:"50"},
      {eng:"Nuts", arb:"مكسرات", price:"50"},
      {eng:"Flavors", arb:"نكهمات", price:"50"},
      {eng:"Nutella", arb:"نوتيلا", price:"50"},
      {eng:"Shishah", arb:"الشيشة", price:"250"},
      {eng:"Meassel (2)", arb:"معسل (2 حجر)", price:"275"},
      {eng:"Flavors (shisha)", arb:"نكهات", price:"295"},
      {eng:"Pyrex Glass", arb:"زجاج بيركس", price:"50"}
    ]
  }
];

/* ---------- helper: small SVG placeholder generator ---------- */
function svgData(color1="#D4AF37", color2="#6B3E26", letter="G"){
  const svg = `<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'>
  <defs><linearGradient id='g' x1='0' x2='1'><stop offset='0' stop-color='${color1}'/><stop offset='1' stop-color='${color2}'/></linearGradient></defs>
  <rect width='100' height='100' rx='12' fill='url(#g)'/>
  <text x='50' y='57' font-size='42' font-family='Arial' font-weight='700' text-anchor='middle' fill='#fff'>${letter}</text>
  </svg>`;
  return "data:image/svg+xml;charset=utf-8," + encodeURIComponent(svg);
}

/* ---------- render menu ---------- */
const menuSections = document.getElementById('menuSections');
const toc = document.getElementById('toc');

function createSectionBlock(section){
  // card container
  const card = document.createElement('div');
  card.className = 'card';
  card.id = section.id;

  // title + collapse
  const titleWrap = document.createElement('div');
  titleWrap.className = 'section-title';
  titleWrap.innerHTML = `<div style="display:flex;align-items:center;gap:10px">
    <div style="width:10px;height:30px;background:var(--gold);border-radius:6px"></div>
    <h2>${section.titleAr} <span style="font-size:12px;margin-left:8px;color:var(--muted)}">(${section.titleEn})</span></h2>
    </div>`;

  card.appendChild(titleWrap);

  const itemsWrap = document.createElement('div');
  itemsWrap.className = 'items';

  section.items.forEach((it, idx) => {
    const item = document.createElement('div'); item.className='item';
    // thumbnail
    const thumb = document.createElement('div'); thumb.className='thumb';
    const svg = document.createElement('img'); svg.alt = it.eng; svg.src = svgData();
    thumb.appendChild(svg);
    thumb.addEventListener('click',()=>openModal(it));

    const info = document.createElement('div'); info.className='item-info';
    const title = document.createElement('div'); title.className='title';
    const names = document.createElement('div'); names.className='names';
    const eng = document.createElement('div'); eng.className='eng'; eng.textContent = it.eng;
    const arb = document.createElement('div'); arb.className='arb'; arb.textContent = it.arb;
    names.appendChild(eng); names.appendChild(arb);

    const priceBox = document.createElement('div'); priceBox.className='price';
    priceBox.textContent = it.price ? it.price + " EGP" : "-";

    title.appendChild(names); title.appendChild(priceBox);
    info.appendChild(title);
    if(it.short){
      const short = document.createElement('div'); short.className='small-muted'; short.style.marginTop='6px';
      short.textContent = it.short; info.appendChild(short);
    }

    // add to item
    item.appendChild(thumb); item.appendChild(info);

    // optional badge or actions
    const controls = document.createElement('div'); controls.style.marginLeft='10px';
    const addBtn = document.createElement('button'); addBtn.className='btn'; addBtn.textContent='تفاصيل';
    addBtn.addEventListener('click',()=>openModal(it));
    controls.appendChild(addBtn);
    item.appendChild(controls);

    itemsWrap.appendChild(item);
  });

  card.appendChild(itemsWrap);
  return card;
}

// populate TOC and sections
menuData.forEach(section=>{
  // add to sections grid (full-width 2 columns handled by grid)
  const secBlock = createSectionBlock(section);
  menuSections.appendChild(secBlock);

  // create toc link
  const a = document.createElement('a');
  a.href = "#"+section.id;
  a.innerHTML = `<span style="width:10px;height:10px;border-radius:3px;background:var(--gold);display:inline-block"></span> ${section.titleAr}`;
  a.addEventListener('click', (e)=>{
    e.preventDefault();
    document.getElementById(section.id).scrollIntoView({behavior:'smooth',block:'start'});
  });
  toc.appendChild(a);
});

// search filter
const searchEl = document.getElementById('search');
searchEl.addEventListener('input', e=>{
  const q = e.target.value.trim().toLowerCase();
  document.querySelectorAll('.item').forEach(it=>{
    const text = it.innerText.toLowerCase();
    if(!q || text.indexOf(q) !== -1) it.style.display = '';
    else it.style.display = 'none';
  });
});

// modal functions
const modal = document.getElementById('modal');
const modalImg = document.getElementById('modalImg');
const modalTitle = document.getElementById('modalTitle');
const modalSub = document.getElementById('modalSub');
const modalDesc = document.getElementById('modalDesc');
document.getElementById('closeModal').addEventListener('click',closeModal);
modal.addEventListener('click', (ev)=>{ if(ev.target===modal) closeModal(); });

function openModal(item){
  modal.classList.add('open');
  modal.setAttribute('aria-hidden','false');
  modalTitle.textContent = item.eng + " — " + item.arb;
  modalSub.textContent = item.price ? (item.price + " EGP") : "";
  modalImg.src = svgData(); // placeholder (replace with real image url if available)
  modalImg.alt = item.eng;
  modalDesc.textContent = item.short ? item.short : "تفاصيل إضافية غير متاحة.";
}

function closeModal(){
  modal.classList.remove('open');
  modal.setAttribute('aria-hidden','true');
}

/* toggle collapse all: simply toggle display of items (for quick UX) */
document.getElementById('toggleAll').addEventListener('click', ()=>{
  const all = document.querySelectorAll('.items');
  const first = all[0];
  if(!first) return;
  const isHidden = first.style.display === 'none';
  all.forEach(a=> a.style.display = isHidden ? 'flex' : 'none');
});

/* download as PDF — use browser print */
document.getElementById('downloadPdf').addEventListener('click', ()=>{
  // give the user instruction for best results: open print dialog
  window.print();
});

/* smooth insertion animation */
document.querySelectorAll('.card').forEach((c,i)=> c.style.animationDelay = (i*80)+'ms');

</script>

</body>
</html>
