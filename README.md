
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>SouqLuma | سوق لوما</title>
<style>
*{box-sizing:border-box}
body{margin:0;background:#111;color:#fff;font-family:Arial,sans-serif}
header{padding:22px;background:#191714;text-align:center;border-bottom:2px solid #c9a45c}
.logo{font-size:30px;color:#d9b76e;font-weight:bold}
nav{padding:15px;text-align:center}
nav a{color:#d9b76e;margin:10px;text-decoration:none}
.hero{text-align:center;padding:65px 15px;background:linear-gradient(130deg,#292015,#111)}
h1{color:#e3c27b;font-size:35px}
.hero p{color:#ddd;line-height:1.8}
button{background:#d9b76e;color:#111;border:0;padding:12px 24px;border-radius:25px;font-weight:bold;cursor:pointer}
.products{padding:25px 15px}
h2{text-align:center;color:#d9b76e}
.grid{display:grid;grid-template-columns:repeat(2,1fr);gap:15px}
.card{background:#201e1a;padding:18px;border-radius:12px;text-align:center}
.icon{font-size:42px;padding:15px}
.card p{color:#ccc}
footer{text-align:center;padding:25px;color:#d9b76e}
</style>
</head>
<body>
<header><div class="logo">SouqLuma</div></header>
<nav>
<a href="#">الرئيسية</a>
<a href="#products">المنتجات</a>
<a href="#contact">اتصل بنا</a>
</nav>
<section class="hero">
<h1 id="title">مرحبا بك في SouqLuma</h1>
<p id="description">اكتشف أجمل المنتجات بأفضل الاختيارات.<br>متجرك الإلكتروني للأناقة والجودة.</p>
<button onclick="document.getElementById('products').scrollIntoView()">تسوق الآن</button>
<button onclick="changeLanguage()">English</button>
</section>
<section class="products" id="products">
<h2>اكتشف منتجاتنا</h2>
<div class="grid">
<div class="card"><div class="icon">📱</div><h3>الإلكترونيات</h3><p>منتجات تقنية متنوعة</p></div>
<div class="card"><div class="icon">👕</div><h3>الملابس</h3><p>أناقة لكل يوم</p></div>
<div class="card"><div class="icon">🌸</div><h3>العطور والجمال</h3><p>اختيارات مميزة</p></div>
<div class="card"><div class="icon">🏠</div><h3>المنزل</h3><p>كل ما تحتاجه لبيتك</p></div>
<div class="card"><div class="icon">⌚</div><h3>الإكسسوارات</h3><p>لمسات أنيقة</p></div>
<div class="card"><div class="icon">🎁</div><h3>منتجات متنوعة</h3><p>اكتشف المزيد</p></div>
</div>
</section>
<footer id="contact">
<h3>SouqLuma</h3>
<p>للطلب والاستفسار تواصل معنا</p>
<a href="https://wa.me/212603290434">
<button>اطلب عبر واتساب</button>
</a>
<p>© SouqLuma 2026</p>
</footer>
<script>
let english=false;
function changeLanguage(){
english=!english;
document.documentElement.lang=english?"en":"ar";
document.documentElement.dir=english?"ltr":"rtl";
document.getElementById("title").textContent=english?"Welcome to SouqLuma":"مرحبا بك في SouqLuma";
document.getElementById("description").textContent=english?"Discover beautiful products for your everyday life.":"اكتشف أجمل المنتجات بأفضل الاختيارات.";
}
</script>
</body>
</html>
