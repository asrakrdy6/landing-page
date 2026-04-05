<!DOCTYPE html><html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>مطعم الشيف - فاخر</title><style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Arial;}

body{
background:#0f0f0f;
color:white;
}

/* NAV */
nav{
display:flex;
justify-content:space-between;
align-items:center;
padding:15px 25px;
background:rgba(0,0,0,0.6);
backdrop-filter:blur(10px);
position:sticky;
top:0;
z-index:10;
}

nav a{
color:white;
margin:0 10px;
text-decoration:none;
transition:0.3s;
}
nav a:hover{color:orange;}

/* HERO */
.hero{
height:100vh;
display:flex;
align-items:center;
justify-content:center;
text-align:center;
background:linear-gradient(rgba(0,0,0,0.7),rgba(0,0,0,0.7)),
url('https://images.unsplash.com/photo-1529692236671-f1f6cf9683ba') center/cover;
}

.hero h1{
font-size:55px;
animation:fadeIn 2s ease;
}

.hero p{
margin-top:10px;
font-size:18px;
color:#ddd;
}

.btn{
display:inline-block;
padding:12px 25px;
margin:10px;
border-radius:30px;
text-decoration:none;
font-weight:bold;
transition:0.3s;
}

.btn-primary{
background:orange;
color:black;
}

.btn-primary:hover{
transform:scale(1.05);
}

.btn-green{
background:green;
color:white;
}

/* SECTIONS */
section{
padding:70px 20px;
text-align:center;
}

h2{
font-size:32px;
margin-bottom:30px;
color:orange;
}

/* MENU */
.menu{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
gap:20px;
max-width:1000px;
margin:auto;
}

.card{
background:#1c1c1c;
padding:20px;
border-radius:15px;
transition:0.3s;
}

.card:hover{
transform:translateY(-8px);
background:#2a2a2a;
}

.price{
color:lightgreen;
margin-top:10px;
font-weight:bold;
}

/* BOOKING */
.booking{
background:#141414;
max-width:500px;
margin:auto;
padding:25px;
border-radius:15px;
box-shadow:0 0 20px rgba(255,165,0,0.2);
}

input{
width:100%;
padding:12px;
margin:8px 0;
border-radius:10px;
border:none;
outline:none;
}

button{
width:100%;
padding:12px;
background:orange;
border:none;
border-radius:10px;
font-weight:bold;
cursor:pointer;
transition:0.3s;
}

button:hover{transform:scale(1.03);}

footer{
padding:20px;
background:#000;
text-align:center;
margin-top:40px;
}

@keyframes fadeIn{
from{opacity:0;transform:translateY(30px);}
to{opacity:1;transform:translateY(0);}
}

</style></head>
<body><nav>
<div>🍽️ مطعم الشيف</div>
<div>
<a href="#menu">المنيو</a>
<a href="#book">حجز</a>
<a href="#contact">تواصل</a>
</div>
</nav><div class="hero">
<div>
<h1>مطعم الشيف الفاخر 🍽️</h1>
<p>تجربة طعام لا تُنسى بأعلى جودة</p>
<a href="#menu" class="btn btn-primary">استعرض المنيو</a>
<a href="https://wa.me/963000000000" class="btn btn-green">واتساب</a>
</div>
</div><section id="menu">
<h2>🔥 المنيو الفاخر</h2>
<div class="menu">
<div class="card">
<h3>🥩 ستيك</h3>
<p>لحم فاخر مشوي بعناية</p>
<div class="price">12$</div>
</div><div class="card">
<h3>🍣 سوشي</h3>
<p>طازج يومياً</p>
<div class="price">15$</div>
</div><div class="card">
<h3>🍕 بيتزا إيطالية</h3>
<p>جبنة موزاريلا أصلية</p>
<div class="price">10$</div>
</div>
</div>
</section><section id="book">
<h2>📅 احجز طاولتك</h2>
<div class="booking">
<input type="text" id="name" placeholder="اسمك">
<input type="date" id="date">
<input type="time" id="time">
<input type="number" id="people" placeholder="عدد الأشخاص">
<button onclick="bookTable()">تأكيد الحجز</button>
</div>
</section><footer id="contact">
📍 مطعم الشيف الفاخر | خدمة 5 نجوم
</footer><script>
function bookTable(){
let name=document.getElementById('name').value;
let date=document.getElementById('date').value;
let time=document.getElementById('time').value;
let people=document.getElementById('people').value;

let msg=حجز جديد:%0Aالاسم: ${name}%0Aالتاريخ: ${date}%0Aالوقت: ${time}%0Aالأشخاص: ${people};

window.open(https://wa.me/963000000000?text=${msg},'_blank');
}
</script></body>
</html>
