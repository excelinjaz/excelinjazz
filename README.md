<!doctype html>
<html lang="ar" dir="rtl">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>إكسل وإنجاز للمقاولات | أعمال الحديد</title>
<style>
:root{
  --navy:#071b2b;
  --gold:#d6ad59;
  --text:#102331;
  --muted:#667783;
  --line:#dfe5e9;
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{font-family:'Segoe UI',Tahoma,sans-serif;background:#f8f9fa;color:var(--text)}
.container{width:min(1180px,92%);margin:auto}
.en{display:none}
body.english{direction:ltr}
body.english .ar{display:none!important}
body.english .en{display:inline}

header{position:sticky;top:0;z-index:100;background:rgba(255,255,255,.97);border-bottom:2px solid var(--gold);backdrop-filter:blur(8px)}
.nav{min-height:78px;display:flex;align-items:center;gap:20px;flex-wrap:wrap}
.brand{display:flex;align-items:center;gap:12px}
.brand-logo{width:50px;height:50px;background:var(--navy);border-radius:50%;display:flex;align-items:center;justify-content:center;color:var(--gold);font-weight:900;font-size:22px}
.brand-text strong{display:block;color:var(--navy);font-size:18px}
.brand-text small{color:#70808b;font-size:13px}
nav{display:flex;gap:22px;margin-inline-start:auto;flex-wrap:wrap}
nav a{text-decoration:none;color:var(--navy);font-weight:700;font-size:15px;transition:.3s}
nav a:hover{color:var(--gold)}
.lang{border:2px solid var(--navy);background:transparent;color:var(--navy);border-radius:8px;padding:8px 16px;font-weight:800;cursor:pointer;transition:.3s}
.lang:hover{background:var(--navy);color:#fff}

.hero{min-height:580px;display:flex;align-items:center;background:linear-gradient(135deg,rgba(7,27,43,.92),rgba(7,27,43,.7)),url('https://images.unsplash.com/photo-1504917595217-d4dc5ebe6122?w=1200') center/cover no-repeat;color:#fff}
.hero-content{max-width:760px;padding:60px 0}
.hero .kicker{color:var(--gold);font-weight:800}
.hero h1{font-size:48px;margin:12px 0 18px;line-height:1.15}
.hero h1 span{color:var(--gold)}
.hero p{font-size:18px;line-height:1.9;color:#dce4ea;margin-bottom:25px}
.hero-buttons{display:flex;gap:16px;flex-wrap:wrap}
.btn{display:inline-block;padding:14px 38px;border-radius:50px;font-weight:700;text-decoration:none;transition:.3s;font-size:16px}
.btn-primary{background:var(--gold);color:var(--navy)}
.btn-primary:hover{background:#c49a3f;transform:scale(1.03)}
.btn-outline{border:2px solid #fff;color:#fff}
.btn-outline:hover{background:#fff;color:var(--navy)}
.signature{margin-top:20px;padding-top:16px;border-top:1px solid rgba(214,173,89,.4);color:var(--gold);font-weight:600}

section{padding:70px 0}
.section-head{text-align:center;margin-bottom:40px}
.section-head .label{color:var(--gold);font-weight:800}
.section-head h2{font-size:36px;color:var(--navy);margin:8px 0 10px}
.section-head p{color:var(--muted);line-height:1.8;max-width:700px;margin:auto}

.about-grid{display:grid;grid-template-columns:1.2fr .8fr;gap:40px;align-items:center}
.about-grid h2{font-size:34px;color:var(--navy)}
.about-grid p{color:#596b77;line-height:1.9;font-size:16px}
.features{display:grid;grid-template-columns:1fr 1fr;gap:14px}
.feature{background:#fff;border:1px solid var(--line);border-radius:12px;padding:20px;text-align:center;box-shadow:0 2px 8px rgba(0,0,0,.04)}
.feature .icon{font-size:32px;display:block;margin-bottom:6px}
.feature strong{display:block;color:var(--navy);font-size:16px}
.feature span{color:var(--muted);font-size:14px}

.services{background:#f4f6f7}
.services-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
.service{background:#fff;border-radius:12px;padding:24px;border-top:4px solid var(--gold);box-shadow:0 2px 12px rgba(0,0,0,.06);transition:.3s}
.service:hover{transform:translateY(-5px);box-shadow:0 8px 25px rgba(0,0,0,.1)}
.service .icon{font-size:32px;display:block;margin-bottom:8px}
.service h3{font-size:18px;color:var(--navy);margin-bottom:6px}
.service p{color:#687984;font-size:14px;line-height:1.7}

.works{background:var(--navy)}
.works .section-head h2{color:#fff}
.works .section-head p{color:#b0c0cb}
.works-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:22px}
.work-card{background:#fff;border-radius:14px;overflow:hidden;box-shadow:0 8px 30px rgba(0,0,0,.2);transition:.3s}
.work-card:hover{transform:scale(1.02)}
.work-card img{width:100%;height:240px;object-fit:cover;display:block}
.work-info{padding:16px 18px 20px}
.work-info strong{display:block;color:var(--navy);font-size:17px;margin-bottom:4px}
.work-info .tag{display:inline-block;background:var(--gold);color:var(--navy);padding:2px 14px;border-radius:20px;font-size:12px;font-weight:700}

.quality{background:#f4f6f7;text-align:center}
.quality h2{font-size:34px;color:var(--navy)}
.quality p{color:#647580;line-height:1.9;max-width:750px;margin:10px auto 0}

.contact{background:linear-gradient(135deg,#071b2b,#0c314a);color:#fff}
.contact-grid{display:grid;grid-template-columns:1fr 1fr;gap:40px;align-items:center}
.contact h2{font-size:34px}
.contact p{color:#cbd6dd;line-height:1.8}
.contact-links{display:grid;gap:12px}
.contact-links a{color:#fff;text-decoration:none;padding:16px 20px;background:rgba(255,255,255,.07);border-right:4px solid var(--gold);border-radius:10px;transition:.3s;display:flex;align-items:center;gap:12px}
.contact-links a:hover{background:rgba(255,255,255,.14)}
.contact-links .icon{font-size:22px}

footer{padding:25px 0;background:#04111b;color:#9aabb7;text-align:center;font-size:13px}

@media(max-width:900px){nav{display:none}.about-grid,.contact-grid{grid-template-columns:1fr}.services-grid,.works-grid{grid-template-columns:1fr 1fr}}
@media(max-width:600px){.hero h1{font-size:30px}.hero-buttons .btn{width:100%;text-align:center}.services-grid,.works-grid,.features{grid-template-columns:1fr}.work-card img{height:200px}section{padding:50px 0}.section-head h2{font-size:28px}}
</style>
</head>
<body>
<header>
  <div class="container nav">
    <div class="brand">
      <div class="brand-logo">EI</div>
      <div class="brand-text">
        <strong><span class="ar">إكسل وإنجاز للمقاولات</span><span class="en">Excel & Injaz Contracting</span></strong>
        <small><span class="ar">أعمال الحديد والمنشآت المعدنية</span><span class="en">Steel & Metal Structures</span></small>
      </div>
    </div>
    <nav>
      <a href="#home"><span class="ar">الرئيسية</span><span class="en">Home</span></a>
      <a href="#about"><span class="ar">من نحن</span><span class="en">About</span></a>
      <a href="#services"><span class="ar">خدماتنا</span><span class="en">Services</span></a>
      <a href="#works"><span class="ar">أعمالنا</span><span class="en">Our Works</span></a>
      <a href="#contact"><span class="ar">تواصل معنا</span><span class="en">Contact</span></a>
    </nav>
    <button class="lang" onclick="toggleLanguage()">English</button>
  </div>
</header>

<main>
<section class="hero" id="home">
  <div class="container hero-content">
    <div class="kicker"><span class="ar">🏗️ حلول متكاملة في أعمال الحديد</span><span class="en">🏗️ Integrated Steel Solutions</span></div>
    <h1><span class="ar">إكسل <span>وإنجاز</span> للمقاولات</span><span class="en">Excel <span>&</span> Injaz Contracting</span></h1>
    <p><span class="ar">نقدم حلولاً متكاملة في أعمال الحديد والمنشآت المعدنية، من التصميم والتصنيع إلى التركيب والتنفيذ، بجودة عالية والتزام بالمواعيد.</span><span class="en">We provide integrated steel and metal structure solutions, from design and fabrication to installation and execution, with high quality and commitment to timelines.</span></p>
    <div class="hero-buttons">
      <a href="#works" class="btn btn-primary"><span class="ar">📂 استعرض أعمالنا</span><span class="en">📂 View Our Work</span></a>
      <a href="#contact" class="btn btn-outline"><span class="ar">📞 تواصل معنا</span><span class="en">📞 Contact Us</span></a>
    </div>
    <div class="signature"><span class="ar">جودة في التصنيع • دقة في التنفيذ • التزام في التسليم</span><span class="en">Quality Fabrication • Precise Execution • On-Time Delivery</span></div>
  </div>
</section>

<section id="about">
  <div class="container about-grid">
    <div>
      <h2><span class="ar">شريكك الموثوق في أعمال الحديد</span><span class="en">Your Trusted Partner in Steel Works</span></h2>
      <p><span class="ar">مؤسسة إكسل وإنجاز للمقاولات متخصصة في تقديم حلول متكاملة لأعمال الحديد والمنشآت المعدنية. ننفذ مشاريعنا بأعلى معايير الجودة، مع فريق فني ذو خبرة وكفاءة عالية، ونحرص على الالتزام بالمخططات والمواصفات وتلبية متطلبات العملاء.</span><span class="en">Excel & Injaz Contracting specializes in integrated steel and metal structure solutions. We execute our projects to the highest quality standards, with a highly experienced and efficient technical team, committed to drawings, specifications, and client requirements.</span></p>
    </div>
    <div class="features">
      <div class="feature"><span class="icon">⚙️</span><strong><span class="ar">جودة التصنيع</span><span class="en">Quality Fabrication</span></strong><span><span class="ar">أحدث المعدات والتقنيات</span><span class="en">Modern equipment & techniques</span></span></div>
      <div class="feature"><span class="icon">📐</span><strong><span class="ar">دقة التنفيذ</span><span class="en">Precise Execution</span></strong><span><span class="ar">مطابقة للمخططات</span><span class="en">Matching drawings</span></span></div>
      <div class="feature"><span class="icon">⏱️</span><strong><span class="ar">الالتزام بالوقت</span><span class="en">Timely Delivery</span></strong><span><span class="ar">تسليم في الموعد المتفق عليه</span><span class="en">On agreed schedule</span></span></div>
      <div class="feature"><span class="icon">🛡️</span><strong><span class="ar">ضمان الجودة</span><span class="en">Quality Assurance</span></strong><span><span class="ar">فحص واختبار لكل مرحلة</span><span class="en">Inspection at every stage</span></span></div>
    </div>
  </div>
</section>

<section class="services" id="services">
  <div class="container">
    <div class="section-head">
      <div class="label"><span class="ar">خدماتنا</span><span class="en">Our Services</span></div>
      <h2><span class="ar">جميع أعمال الحديد تحت سقف واحد</span><span class="en">All Steel Works Under One Roof</span></h2>
    </div>
    <div class="services-grid">
      <div class="service"><span class="icon">🏗️</span><h3><span class="ar">الهياكل المعدنية</span><span class="en">Steel Structures</span></h3><p><span class="ar">هياكل حديدية للمباني والمصانع والمستودعات</span><span class="en">Steel structures for buildings, factories & warehouses</span></p></div>
      <div class="service"><span class="icon">🚪</span><h3><span class="ar">بوابات وأسوار</span><span class="en">Gates & Fences</span></h3><p><span class="ar">تصنيع وتركيب بوابات حديدية وأسوار للمنازل والمنشآت</span><span class="en">Steel gates and fences for homes & facilities</span></p></div>
      <div class="service"><span class="icon">🪜</span><h3><span class="ar">سلالم وهاندريل</span><span class="en">Stairs & Handrails</span></h3><p><span class="ar">سلالم حديدية وهاندريل ودرابزين حسب الطلب</span><span class="en">Steel stairs, handrails & balustrades custom made</span></p></div>
      <div class="service"><span class="icon">☂️</span><h3><span class="ar">مظلات ومواقف</span><span class="en">Canopies & Parking</span></h3><p><span class="ar">مظلات حديدية للمداخل والمواقف والحدائق</span><span class="en">Steel canopies for entrances, parking & gardens</span></p></div>
      <div class="service"><span class="icon">🏢</span><h3><span class="ar">هياكل المصاعد</span><span class="en">Elevator Structures</span></h3><p><span class="ar">تصنيع وتأسيس هياكل المصاعد للمباني</span><span class="en">Fabrication of elevator steel structures</span></p></div>
      <div class="service"><span class="icon">🔧</span><h3><span class="ar">أعمال حسب الطلب</span><span class="en">Custom Works</span></h3><p><span class="ar">تصنيع أي أعمال حديدية حسب متطلبات المشروع</span><span class="en">Custom steel works per project requirements</span></p></div>
    </div>
  </div>
</section>

<section class="works" id="works">
  <div class="container">
    <div class="section-head">
      <div class="label"><span class="ar">📸 أعمالنا</span><span class="en">📸 Our Works</span></div>
      <h2><span class="ar">نماذج من مشاريع الحديد المنفذة</span><span class="en">Sample of Our Steel Projects</span></h2>
      <p><span class="ar">صور حقيقية لأعمالنا في مختلف مجالات الحديد والحدادة</span><span class="en">Real photos of our work across various steel sectors</span></p>
    </div>
    <div class="works-grid">
      <div class="work-card"><img src="https://images.unsplash.com/photo-1581092160607-ee22621dd758?w=600&h=400&fit=crop" alt="هيكل معدني"><div class="work-info"><strong><span class="ar">هياكل معدنية</span><span class="en">Steel Structures</span></strong><span class="tag">مصنع / مستودع</span></div></div>
      <div class="work-card"><img src="https://images.unsplash.com/photo-1590568268961-d908a375fec9?w=600&h=400&fit=crop" alt="بوابات حديدية"><div class="work-info"><strong><span class="ar">بوابات حديدية</span><span class="en">Steel Gates</span></strong><span class="tag">مداخل / فلل</span></div></div>
      <div class="work-card"><img src="https://images.unsplash.com/photo-1590568268961-d908a375fec9?w=600&h=400&fit=crop" alt="أسوار حديدية"><div class="work-info"><strong><span class="ar">أسوار حديدية</span><span class="en">Steel Fences</span></strong><span class="tag">منازل / منشآت</span></div></div>
      <div class="work-card"><img src="https://images.unsplash.com/photo-1581092160607-ee22621dd758?w=600&h=400&fit=crop" alt="سلالم حديدية"><div class="work-info"><strong><span class="ar">سلالم حديدية</span><span class="en">Steel Stairs</span></strong><span class="tag">داخلية / خارجية</span></div></div>
      <div class="work-card"><img src="https://images.unsplash.com/photo-1590568268961-d908a375fec9?w=600&h=400&fit=crop" alt="مظلات حديدية"><div class="work-info"><strong><span class="ar">مظلات ومواقف</span><span class="en">Canopies & Parking</span></strong><span class="tag">مداخل / حدائق</span></div></div>
      <div class="work-card"><img src="https://images.unsplash.com/photo-1581092160607-ee22621dd758?w=600&h=400&fit=crop" alt="هياكل المصاعد"><div class="work-info"><strong><span class="ar">هياكل المصاعد</span><span class="en">Elevator Structures</span></strong><span class="tag">مباني سكنية / تجارية</span></div></div>
      <div class="work-card"><img src="https://images.unsplash.com/photo-1590568268961-d908a375fec9?w=600&h=400&fit=crop" alt="درابزين"><div class="work-info"><strong><span class="ar">درابزين وهاندريل</span><span class="en">Handrails & Balustrades</span></strong><span class="tag">سلالم / شرفات</span></div></div>
      <div class="work-card"><img src="https://images.unsplash.com/photo-1581092160607-ee22621dd758?w=600&h=400&fit=crop" alt="هناجر"><div class="work-info"><strong><span class="ar">هناجر ومستودعات</span><span class="en">Hangars & Warehouses</span></strong><span class="tag">مشاريع صناعية</span></div></div>
      <div class="work-card"><img src="https://images.unsplash.com/photo-1590568268961-d908a375fec9?w=600&h=400&fit=crop" alt="أعمال حسب الطلب"><div class="work-info"><strong><span class="ar">أعمال حسب الطلب</span><span class="en">Custom Steel Works</span></strong><span class="tag">تصميم خاص</span></div></div>
    </div>
  </div>
</section>

<section class="quality">
  <div class="container">
    <h2><span class="ar">🛡️ الجودة أساس ثقة عملائنا</span><span class="en">🛡️ Quality Is the Foundation of Our Clients' Trust</span></h2>
    <p><span class="ar">نحرص في كل مشروع على استخدام أجود أنواع الحديد، واتباع أحدث أساليب التصنيع واللحام، مع فحص دقيق لكل مرحلة لضمان منتج نهائي متين وآمن يدوم لسنوات.</span><span class="en">In every project, we ensure the use of top-quality steel, applying the latest fabrication and welding techniques, with thorough inspection at every stage to guarantee a durable and safe final product.</span></p>
  </div>
</section>

<section class="contact" id="contact">
  <div class="container contact-grid">
    <div>
      <h2><span class="ar">📞 تواصل معنا</span><span class="en">📞 Contact Us</span></h2>
      <p><span class="ar">نرحب باستفساراتكم وطلباتكم، فريقنا جاهز للإجابة على جميع تساؤلاتكم وتقديم العروض المناسبة لمشاريعكم.</span><span class="en">We welcome your inquiries and requests, our team is ready to answer all your questions and provide suitable offers for your projects.</span></p>
    </div>
    <div class="contact-links">
      <a href="tel:+966551889096"><span class="icon">📱</span> <strong><span class="ar">مسؤول المشاريع</span><span class="en">Project Manager</span></strong> — 0551889096</a>
      <a href="https://wa.me/966554726980"><span class="icon">💬</span> <strong>WhatsApp</strong> — 0554726980</a>
      <a href="mailto:excel1lnjaz@gmail.com"><span class="icon">✉️</span> <strong>Email</strong> — excel1lnjaz@gmail.com</a>
    </div>
  </div>
</section>
</main>

<footer>
  <div class="container">
    <span class="ar">© 2026 إكسل وإنجاز للمقاولات — جميع الحقوق محفوظة</span>
    <span class="en">© 2026 Excel & Injaz Contracting — All Rights Reserved</span>
  </div>
</footer>

<script>
function toggleLanguage(){
  const isEnglish=document.body.classList.toggle("english");
  document.documentElement.lang=isEnglish?"en":"ar";
  document.documentElement.dir=isEnglish?"ltr":"rtl";
  document.querySelector(".lang").textContent=isEnglish?"العربية":"English";
}
</script>
</body>
</html>
