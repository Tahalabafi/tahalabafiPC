
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080f20">
<meta name="description" content="TahaPC | خدمات کامپیوتری طاها لبافی، نصب ویندوز، نرم افزار و پشتیبانی کامپیوتر در تهران">
<title>TahaPC | طاها لبافی</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>
:root{
--bg:#080f20;
--card:#111d33;
--blue:#2563eb;
--cyan:#38bdf8;
--orange:#f59e0b;
--white:#f8fafc;
--gray:#a5b4c8;
}
*{margin:0;padding:0;box-sizing:border-box}
html{scroll-behavior:smooth}
body{
font-family:'Vazirmatn',sans-serif;
background:var(--bg);
color:var(--white);
line-height:1.9;
overflow-x:hidden;
}
a{text-decoration:none;color:inherit}
.container{width:90%;max-width:1150px;margin:auto}
header{
position:sticky;top:0;z-index:100;
background:rgba(8,15,32,.94);
backdrop-filter:blur(15px);
border-bottom:1px solid #263750;
}
nav{
min-height:70px;display:flex;
align-items:center;justify-content:space-between;
}
.logo{font-size:25px;font-weight:800;color:var(--cyan)}
.logo span{color:white}
.nav-links{display:flex;gap:22px;font-size:13px}
.nav-links a:hover{color:var(--cyan)}
.menu-btn{display:none;background:none;border:0;color:white;font-size:27px}
.hero{
min-height:650px;display:flex;align-items:center;
background:linear-gradient(90deg,rgba(8,15,32,.65),#080f20 100%),
url('https://images.unsplash.com/photo-1593640408182-31c70c8268f5?w=1600') center/cover;
}
.hero-content{max-width:650px;padding:100px 0}
.tag{
display:inline-block;padding:6px 15px;border-radius:30px;
background:#163b67;color:#7dd3fc;font-size:13px;
}
h1{font-size:clamp(34px,7vw,62px);line-height:1.5;margin:20px 0}
h1 span{color:var(--cyan)}
.hero p{color:var(--gray);font-size:17px}
.actions{display:flex;gap:12px;flex-wrap:wrap;margin-top:30px}
.btn{
padding:12px 24px;border-radius:12px;
background:var(--blue);font-weight:700;
display:inline-block;transition:.3s;
}
.btn:hover{transform:translateY(-4px);background:#3b82f6}
.btn-outline{background:transparent;border:1px solid var(--cyan)}
section{padding:85px 0}
.section-title{text-align:center;margin-bottom:40px}
.section-title h2{font-size:30px}
.section-title p{color:var(--gray);margin-top:8px}
.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:35px;align-items:center}
.about-img{width:100%;height:350px;object-fit:cover;border-radius:20px}
.about-text p{color:var(--gray);margin:15px 0}
.cards{
display:grid;grid-template-columns:repeat(3,1fr);gap:20px;
}
.card{
background:var(--card);border:1px solid #243650;
border-radius:18px;overflow:hidden;transition:.3s;
}
.card:hover{transform:translateY(-7px);border-color:var(--cyan)}
.card img{width:100%;height:190px;object-fit:cover}
.card-content{padding:20px}
.card h3{font-size:18px;margin-bottom:8px}
.card p{color:var(--gray);font-size:14px}
.icon{font-size:30px;margin-bottom:10px}
.features{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
.feature{
background:var(--card);padding:25px;border-radius:15px;
border:1px solid #263750;text-align:center;
}
.gallery{display:grid;grid-template-columns:repeat(3,1fr);gap:15px}
.gallery img{width:100%;height:220px;object-fit:cover;border-radius:15px;transition:.3s}
.gallery img:hover{transform:scale(1.03)}
.contact-box{
background:linear-gradient(135deg,#142c54,#102039);
padding:40px;border-radius:22px;text-align:center;
}
.contact-box p{color:var(--gray);margin:10px}
form{max-width:600px;margin:25px auto 0;display:grid;gap:12px}
input,select,textarea{
width:100%;padding:14px;border-radius:10px;
background:#0b172b;border:1px solid #33445e;
color:white;font:inherit;outline:none;
}
textarea{min-height:110px;resize:vertical}
form button{border:0;color:white;font:inherit;cursor:pointer}
.faq details{
background:var(--card);padding:17px;margin:12px 0;
border-radius:12px;border:1px solid #263750;
}
.faq summary{cursor:pointer;font-weight:600}
.faq p{color:var(--gray);padding-top:10px}
footer{
padding:35px 0;text-align:center;
border-top:1px solid #263750;color:var(--gray);
}
.social{display:flex;justify-content:center;gap:15px;margin:20px 0}
.social a{color:var(--cyan)}
.float{
position:fixed;bottom:20px;left:18px;z-index:90;
background:#16a34a;color:white;padding:12px 17px;
border-radius:40px;box-shadow:0 5px 20px #0008;
}
@media(max-width:750px){
.nav-links{
display:none;position:absolute;top:70px;right:0;
width:100%;background:#0c172a;padding:20px;
flex-direction:column;gap:15px;
}
.nav-links.show{display:flex}
.menu-btn{display:block}
.hero{min-height:590px;background-position:center}
.hero-content{padding:80px 0}
.hero p{font-size:15px}
section{padding:65px 0}
.about-grid{grid-template-columns:1fr}
.about-img{height:250px}
.cards{grid-template-columns:1fr 1fr;gap:12px}
.card img{height:130px}
.card-content{padding:13px}
.card h3{font-size:15px}
.card p{font-size:12px}
.features{grid-template-columns:1fr 1fr}
.gallery{grid-template-columns:1fr 1fr;gap:10px}
.gallery img{height:140px}
.section-title h2{font-size:25px}
.contact-box{padding:25px 15px}
}
@media(max-width:390px){
.cards,.features{grid-template-columns:1fr}
}
</style>
</head>

<body>

<header>
<div class="container">
<nav>
<a href="#" class="logo">TAHA<span>PC</span></a>
<button class="menu-btn" onclick="document.querySelector('.nav-links').classList.toggle('show')">☰</button>
<div class="nav-links">
<a href="#home">خانه</a>
<a href="#about">درباره من</a>
<a href="#services">خدمات</a>
<a href="#gallery">گالری</a>
<a href="#faq">سوالات</a>
<a href="#contact">تماس</a>
</div>
</nav>
</div>
</header>

<main>
<section class="hero" id="home">
<div class="container">
<div class="hero-content">
<span class="tag">خدمات کامپیوتری با طاها لبافی</span>
<h1>تکنولوژی،<br><span>ساده‌تر از همیشه.</span></h1>
<p>از نصب ویندوز و نرم‌افزار تا عیب‌یابی و خدمات کامپیوتری؛ همراه شما در دنیای دیجیتال.</p>
<div class="actions">
<a href="#contact" class="btn">درخواست خدمات</a>
<a href="#services" class="btn btn-outline">مشاهده خدمات</a>
</div>
</div>
</div>
</section>

<section id="about">
<div class="container about-grid">
<div>
<img class="about-img" src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?w=900" alt="میز کار کامپیوتری">
</div>
<div class="about-text">
<span class="tag">ABOUT TAHA</span>
<h2>من طاها لبافی هستم</h2>
<p>به دنیای TahaPC خوش اومدید! من طاها لبافی هستم و به دنیای کامپیوتر، فناوری، نرم‌افزار و شبکه علاقه‌مندم.</p>
<p>هدف من ارائه خدمات کامپیوتری با کیفیت، ارتباط شفاف و کمک به حل مشکلات دیجیتال شماست.</p>
<a href="#contact" class="btn">ارتباط با من</a>
</div>
</div>
</section>

<section id="services">
<div class="container">
<div class="section-title">
<h2>خدمات TahaPC</h2>
<p>راهکارهای کامپیوتری برای نیازهای شما</p>
</div>
<div class="cards">
<div class="card">
<img src="https://images.unsplash.com/photo-1587202372775-e229f172b9d7?w=700" alt="کامپیوتر">
<div class="card-content"><h3>نصب ویندوز</h3><p>نصب و راه‌اندازی ویندوز و تنظیمات اولیه سیستم.</p></div>
</div>
<div class="card">
<img src="https://images.unsplash.com/photo-1518770660439-4636190af475?w=700" alt="سخت افزار">
<div class="card-content"><h3>سخت‌افزار</h3><p>بررسی و عیب‌یابی مشکلات سخت‌افزاری کامپیوتر.</p></div>
</div>
<div class="card">
<img src="https://images.unsplash.com/photo-1519389950473-47ba0277781c?w=700" alt="نرم افزار">
<div class="card-content"><h3>نصب نرم‌افزار</h3><p>نصب و راه‌اندازی برنامه‌های کاربردی.</p></div>
</div>
<div class="card">
<img src="https://images.unsplash.com/photo-1591488320449-011701bb6704?w=700" alt="سیستم گیمینگ">
<div class="card-content"><h3>راه‌اندازی سیستم</h3><p>آماده‌سازی و تنظیم سیستم‌های کامپیوتری.</p></div>
</div>
<div class="card">
<img src="https://images.unsplash.com/photo-1496181133206-80ce9b88a853?w=700" alt="لپ تاپ">
<div class="card-content"><h3>خدمات لپ‌تاپ</h3><p>بررسی مشکلات نرم‌افزاری و راه‌اندازی لپ‌تاپ.</p></div>
</div>
<div class="card">
<img src="https://images.unsplash.com/photo-1558494949-ef010cbdcc31?w=700" alt="سرور">
<div class="card-content"><h3>شبکه و اینترنت</h3><p>عیب‌یابی اتصال و تنظیمات شبکه.</p></div>
</div>
</div>
</div>
</section>

<section>
<div class="container">
<div class="section-title">
<h2>چرا TahaPC؟</h2>
<p>تجربه‌ای حرفه‌ای و ارتباطی مطمئن</p>
</div>
<div class="features">
<div class="feature"><div class="icon">⚡</div><h3>پاسخگویی</h3><p>ارتباط و هماهنگی راحت</p></div>
<div class="feature"><div class="icon">🛠️</div><h3>دقت در کار</h3><p>بررسی دقیق مشکلات</p></div>
<div class="feature"><div class="icon">💻</div><h3>تخصص فناوری</h3><p>تمرکز بر دنیای کامپیوتر</p></div>
</div>
</div>
</section>

<section id="gallery">
<div class="container">
<div class="section-title">
<h2>دنیای کامپیوتر و تکنولوژی</h2>
<p>نگاهی به دنیای سخت‌افزار و فناوری</p>
</div>
<div class="gallery">
<img src="https://images.unsplash.com/photo-1593640408182-31c70c8268f5?w=700" alt="کامپیوتر دسکتاپ">
<img src="https://images.unsplash.com/photo-1591488320449-011701bb6704?w=700" alt="سیستم گیمینگ">
<img src="https://images.unsplash.com/photo-1587202372775-e229f172b9d7?w=700" alt="قطعات کامپیوتر">
<img src="https://images.unsplash.com/photo-1518770660439-4636190af475?w=700" alt="مادربرد">
<img src="https://images.unsplash.com/photo-1496181133206-80ce9b88a853?w=700" alt="لپ تاپ">
<img src="https://images.unsplash.com/photo-1558494949-ef010cbdcc31?w=700" alt="تجهیزات شبکه">
</div>
</div>
</section>

<section id="faq">
<div class="container faq">
<div class="section-title"><h2>سوالات متداول</h2></div>
<details><summary>چه خدماتی ارائه می‌دهید؟</summary><p>نصب ویندوز، نرم‌افزار، عیب‌یابی و خدمات کامپیوتری ارائه می‌شود.</p></details>
<details><summary>در کدام مناطق فعالیت دارید؟</summary><p>شرق تهران و سایر مناطق تهران با هماهنگی قبلی.</p></details>
<details><summary>چطور درخواست ثبت کنم؟</summary><p>از فرم تماس سایت یا واتساپ درخواست خود را ارسال کنید.</p></details>
<details><summary>هزینه خدمات چطور مشخص می‌شود؟</summary><p>هزینه نهایی پس از بررسی نیاز و هماهنگی مشخص خواهد شد.</p></details>
</div>
</section>

<section id="contact">
<div class="container">
<div class="contact-box">
<span class="tag">CONTACT TAHA</span>
<h2>با طاها لبافی در ارتباط باش</h2>
<p>برای دریافت خدمات یا مشاوره، درخواست خودت رو ارسال کن.</p>
<form id="requestForm">
<input id="name" placeholder="نام و نام خانوادگی" required>
<input id="phone" type="tel" placeholder="شماره تماس" required>
<select id="service">
<option>انتخاب نوع خدمات</option>
<option>نصب ویندوز</option>
<option>نصب نرم‌افزار</option>
<option>عیب‌یابی کامپیوتر</option>
<option>خدمات لپ‌تاپ</option>
<option>شبکه و اینترنت</option>
</select>
<textarea id="message" placeholder="توضیحات درخواست شما"></textarea>
<button class="btn" type="submit">ارسال درخواست به واتساپ</button>
</form>
<div class="social">
<a href="https://instagram.com/Taha_labafi">Instagram</a>
<a href="https://wa.me/989129175621">WhatsApp</a>
<a href="tel:09129175621">تماس تلفنی</a>
</div>
<p>شماره تماس: 09129175621</p>
<p>ایمیل: tahalabafi1388@gmail.com</p>
</div>
</div>
</section>
</main>

<footer>
<div class="container">
<div class="logo">TAHA<span>PC</span></div>
<p>طاها لبافی | خدمات کامپیوتری و دنیای تکنولوژی</p>
<p>© TahaPC - تمامی حقوق محفوظ است.</p>
</div>
</footer>

<a class="float" href="https://wa.me/989129175621">واتساپ</a>

<script>
document.getElementById('requestForm').addEventListener('submit',function(e){
e.preventDefault();
const name=document.getElementById('name').value;
const phone=document.getElementById('phone').value;
const service=document.getElementById('service').value;
const message=document.getElementById('message').value;
const text=`سلام طاها لبافی، درخواست خدمات دارم.%0Aنام: ${encodeURIComponent(name)}%0Aشماره: ${encodeURIComponent(phone)}%0Aخدمات: ${encodeURIComponent(service)}%0Aتوضیحات: ${encodeURIComponent(message)}`;
window.open('https://wa.me/989129175621?text='+text,'_blank');
});
</script>

</body>
</html>

