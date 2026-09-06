<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>S. R. Academy | The Way to Success</title>

<meta name="description" content="S. R. Academy - Concept Based Learning, Smart Classes and Competitive Exam Preparation.">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:Arial, sans-serif;
    background:#f7f9fc;
    color:#172033;
}

:root{
    --navy:#071f41;
    --blue:#0e4d92;
    --gold:#f3bd45;
    --white:#ffffff;
}

/* NAVBAR */

header{
    position:sticky;
    top:0;
    z-index:1000;
    background:rgba(255,255,255,.97);
    box-shadow:0 3px 20px rgba(0,0,0,.08);
}

.navbar{
    max-width:1200px;
    margin:auto;
    padding:16px 5%;
    display:flex;
    align-items:center;
    justify-content:space-between;
}

.logo{
    text-decoration:none;
    font-size:25px;
    font-weight:800;
    color:var(--navy);
}

.logo small{
    display:block;
    color:#b68116;
    font-size:10px;
    letter-spacing:2px;
    margin-top:2px;
}

.nav-links{
    display:flex;
    list-style:none;
    gap:25px;
}

.nav-links a{
    text-decoration:none;
    color:#172033;
    font-weight:600;
}

.nav-links a:hover{
    color:var(--blue);
}

.menu{
    display:none;
    font-size:28px;
    cursor:pointer;
}

/* HERO */

.hero{
    min-height:650px;
    display:flex;
    align-items:center;
    position:relative;
    overflow:hidden;

    background:
    radial-gradient(circle at 80% 20%,rgba(243,189,69,.20),transparent 25%),
    linear-gradient(135deg,#061b38,#0e4d92);
}

.hero:before{
    content:"";
    position:absolute;
    width:400px;
    height:400px;
    border-radius:50%;
    background:rgba(255,255,255,.04);
    right:-100px;
    bottom:-150px;
}

.hero-content{
    max-width:1200px;
    width:90%;
    margin:auto;
    position:relative;
    z-index:2;
    color:white;
}

.tag{
    display:inline-block;
    padding:9px 17px;
    border:1px solid rgba(255,255,255,.4);
    border-radius:30px;
    margin-bottom:20px;
    font-size:14px;
}

.hero h1{
    font-size:65px;
    line-height:1.05;
    margin-bottom:10px;
}

.hero h1 span{
    color:var(--gold);
}

.hero h2{
    font-size:27px;
    font-weight:400;
    margin-bottom:18px;
}

.hero p{
    max-width:680px;
    font-size:18px;
    line-height:1.8;
    color:#e5edf8;
    margin-bottom:30px;
}

.buttons{
    display:flex;
    gap:15px;
    flex-wrap:wrap;
}

.btn{
    display:inline-block;
    padding:14px 25px;
    border-radius:8px;
    text-decoration:none;
    font-weight:bold;
    transition:.3s;
}

.btn:hover{
    transform:translateY(-3px);
}

.btn-gold{
    background:var(--gold);
    color:#14213d;
}

.btn-outline{
    border:2px solid white;
    color:white;
}

.btn-outline:hover{
    background:white;
    color:var(--navy);
}

/* STATS */

.stats{
    background:white;
    box-shadow:0 8px 25px rgba(0,0,0,.08);
}

.stats-grid{
    max-width:1100px;
    margin:auto;
    display:grid;
    grid-template-columns:repeat(4,1fr);
}

.stat{
    text-align:center;
    padding:28px 15px;
    border-right:1px solid #e6eaf0;
}

.stat:last-child{
    border:none;
}

.stat strong{
    display:block;
    font-size:30px;
    color:var(--blue);
}

.stat span{
    color:#667085;
    font-size:14px;
}

/* SECTIONS */

section{
    padding:80px 5%;
}

.container{
    max-width:1150px;
    margin:auto;
}

.section-title{
    text-align:center;
    margin-bottom:45px;
}

.section-title h2{
    font-size:38px;
    color:var(--navy);
    margin-bottom:8px;
}

.section-title p{
    color:#667085;
}

/* ABOUT */

.about-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:30px;
}

.about-card{
    background:white;
    padding:35px;
    border-radius:18px;
    box-shadow:0 8px 30px rgba(0,0,0,.06);
}

.about-card h3{
    color:var(--blue);
    margin-bottom:15px;
    font-size:24px;
}

.about-card p{
    line-height:1.8;
    color:#596579;
}

/* COURSES */

.courses{
    background:#eef4fb;
}

.course-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:22px;
}

.course-card{
    background:white;
    padding:28px;
    border-radius:16px;
    border-bottom:4px solid var(--gold);
    box-shadow:0 8px 25px rgba(0,0,0,.06);
    transition:.3s;
}

.course-card:hover{
    transform:translateY(-6px);
}

.course-card .icon{
    font-size:38px;
    margin-bottom:15px;
}

.course-card h3{
    color:var(--navy);
    margin-bottom:12px;
}

.course-card p{
    color:#667085;
    line-height:1.7;
}

/* WHY US */

.features{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:20px;
}

.feature{
    background:white;
    padding:28px 18px;
    text-align:center;
    border-radius:15px;
    box-shadow:0 7px 25px rgba(0,0,0,.06);
}

.feature-icon{
    font-size:36px;
    margin-bottom:12px;
}

.feature h3{
    color:var(--navy);
    font-size:18px;
    margin-bottom:8px;
}

.feature p{
    color:#667085;
    font-size:14px;
}

/* CTA */

.cta{
    background:linear-gradient(135deg,#071f41,#0e4d92);
    color:white;
    text-align:center;
}

.cta h2{
    font-size:40px;
    margin-bottom:10px;
}

.cta p{
    margin-bottom:25px;
    color:#dce7f5;
}

/* CONTACT */

.contact{
    background:#eef4fb;
}

.contact-box{
    background:white;
    max-width:850px;
    margin:auto;
    padding:40px;
    border-radius:18px;
    text-align:center;
    box-shadow:0 8px 30px rgba(0,0,0,.07);
}

.contact-box h3{
    font-size:28px;
    color:var(--navy);
    margin-bottom:15px;
}

.contact-box p{
    margin:10px 0;
}

/* FOOTER */

footer{
    background:#061a35;
    color:white;
    text-align:center;
    padding:35px 5%;
}

footer h3{
    font-size:25px;
    margin-bottom:8px;
}

footer p{
    color:#bdc9da;
}

.footer-bottom{
    margin-top:25px;
    padding-top:20px;
    border-top:1px solid rgba(255,255,255,.15);
    font-size:13px;
}

/* WHATSAPP */

.whatsapp{
    position:fixed;
    right:20px;
    bottom:20px;
    width:60px;
    height:60px;
    border-radius:50%;
    background:#25d366;
    color:white;
    display:flex;
    align-items:center;
    justify-content:center;
    text-decoration:none;
    font-size:28px;
    box-shadow:0 6px 20px rgba(0,0,0,.25);
    z-index:999;
}

/* MOBILE */

@media(max-width:850px){

    .menu{
        display:block;
    }

    .nav-links{
        display:none;
        position:absolute;
        top:70px;
        left:0;
        width:100%;
        background:white;
        flex-direction:column;
        padding:20px 7%;
        box-shadow:0 8px 20px rgba(0,0,0,.1);
    }

    .nav-links.active{
        display:flex;
    }

    .hero h1{
        font-size:48px;
    }

    .stats-grid{
        grid-template-columns:1fr 1fr;
    }

    .stat:nth-child(2){
        border-right:none;
    }

    .about-grid{
        grid-template-columns:1fr;
    }

    .course-grid{
        grid-template-columns:1fr 1fr;
    }

    .features{
        grid-template-columns:1fr 1fr;
    }
}

@media(max-width:550px){

    .hero{
        min-height:600px;
    }

    .hero h1{
        font-size:40px;
    }

    .hero h2{
        font-size:21px;
    }

    .hero p{
        font-size:16px;
    }

    .course-grid,
    .features,
    .stats-grid{
        grid-template-columns:1fr;
    }

    .stat{
        border-right:none;
        border-bottom:1px solid #e6eaf0;
    }

    .section-title h2{
        font-size:30px;
    }

    .cta h2{
        font-size:30px;
    }
}

</style>
</head>


<body>

<!-- NAVIGATION -->

<header>

<div class="navbar">

<a href="#home" class="logo">
S. R. Academy
<small>THE WAY TO SUCCESS</small>
</a>

<div class="menu" onclick="toggleMenu()">☰</div>

<ul class="nav-links" id="navLinks">
<li><a href="#home">Home</a></li>
<li><a href="#about">About</a></li>
<li><a href="#courses">Courses</a></li>
<li><a href="#why">Why Us</a></li>
<li><a href="#contact">Contact</a></li>
</ul>

</div>

</header>


<!-- HERO -->

<section class="hero" id="home">

<div class="hero-content">

<div class="tag">
🎓 Admissions & New Batches
</div>

<h1>
S. R. <span>Academy</span>
</h1>

<h2>The Way to Success</h2>

<p>
ज्ञान से सफलता तक का सफर।  
Concept Based Learning, Digital Board,
Smart Classes और बेहतर मार्गदर्शन के साथ
अपने लक्ष्य की ओर एक मजबूत कदम बढ़ाएँ।
</p>

<div class="buttons">

<a href="#courses" class="btn btn-gold">
Explore Courses →
</a>

<a href="https://wa.me/918958878452"
class="btn btn-outline"
target="_blank">
WhatsApp Us
</a>

</div>

</div>

</section>


<!-- STATS -->

<div class="stats">

<div class="stats-grid">

<div class="stat">
<strong>9–12</strong>
<span>School Classes</span>
</div>

<div class="stat">
<strong>10+</strong>
<span>Exam Categories</span>
</div>

<div class="stat">
<strong>Smart</strong>
<span>Digital Learning</span>
</div>

<div class="stat">
<strong>100%</strong>
<span>Concept Focus</span>
</div>

</div>

</div>


<!-- ABOUT -->

<section id="about">

<div class="container">

<div class="section-title">

<h2>About S. R. Academy</h2>

<p>
Education with Concept, Technology & Guidance
</p>

</div>


<div class="about-grid">

<div class="about-card">

<h3>🎓 हमारा उद्देश्य</h3>

<p>
S. R. Academy का उद्देश्य विद्यार्थियों को
गुणवत्तापूर्ण शिक्षा, मजबूत Concepts और
सही दिशा प्रदान करना है।

हम School Education के साथ-साथ
Competitive Exams की तैयारी के लिए भी
विद्यार्थियों को बेहतर learning environment
प्रदान करने का प्रयास करते हैं।
</p>

</div>


<div class="about-card">

<h3>💡 हमारी Teaching Approach</h3>

<p>
हमारा focus केवल syllabus पूरा करने पर नहीं,
बल्कि Concepts को समझने और उन्हें practical
तरीके से सीखने पर है।

Digital Board, Visual Learning, नियमित
Practice और Tests के माध्यम से विद्यार्थियों
की तैयारी को बेहतर बनाने का प्रयास किया जाता है।
</p>

</div>

</div>

</div>

</section>


<!-- COURSES -->

<section class="courses" id="courses">

<div class="container">

<div class="section-title">

<h2>Our Courses</h2>

<p>
School Education से Competitive Exams तक
</p>

</div>


<div class="course-grid">

<div class="course-card">

<div class="icon">📘</div>

<h3>Classes 9th–10th</h3>

<p>
Science और English की Concept Based
तैयारी, Regular Practice और Test के साथ।
</p>

</div>


<div class="course-card">

<div class="icon">📕</div>

<h3>Classes 11th–12th</h3>

<p>
Physics, Chemistry, Mathematics और
English की मजबूत Conceptual तैयारी।
</p>

</div>


<div class="course-card">

<div class="icon">🎯</div>

<h3>Competitive Exams</h3>

<p>
Army Agniveer, SSC GD, Railway, UPP,
UPSSSC और TET जैसी परीक्षाओं की तैयारी।
</p>

</div>


<div class="course-card">

<div class="icon">🏆</div>

<h3>Entrance Exams</h3>

<p>
NVS, KVS, Sainik School, Polytechnic
और CUET के लिए focused preparation।
</p>

</div>


<div class="course-card">

<div class="icon">🖥️</div>

<h3>Digital Classes</h3>

<p>
Digital Board, Visual Learning और
3D animations के माध्यम से smart teaching।
</p>

</div>


<div class="course-card">

<div class="icon">📝</div>

<h3>Test & Practice</h3>

<p>
Regular tests, question practice और
exam-oriented preparation।
</p>

</div>

</div>

</div>

</section>


<!-- WHY US -->

<section id="why">

<div class="container">

<div class="section-title">

<h2>Why Choose S. R. Academy?</h2>

<p>
सफलता के लिए सही दिशा और सही अभ्यास
</p>

</div>


<div class="features">

<div class="feature">

<div class="feature-icon">💡</div>

<h3>Concept Based</h3>

<p>
Concept को समझकर सीखने पर जोर।
</p>

</div>


<div class="feature">

<div class="feature-icon">🖥️</div>

<h3>Digital Board</h3>

<p>
Smart और visual classroom learning।
</p>

</div>


<div class="feature">

<div class="feature-icon">🎬</div>

<h3>3D Visual Learning</h3>

<p>
Animations और visual explanations।
</p>

</div>


<div class="feature">

<div class="feature-icon">📝</div>

<h3>Regular Tests</h3>

<p>
Practice और performance improvement।
</p>

</div>


<div class="feature">

<div class="feature-icon">👨‍🏫</div>

<h3>Guidance</h3>

<p>
विद्यार्थियों को उचित academic guidance।
</p>

</div>


<div class="feature">

<div class="feature-icon">❓</div>

<h3>Doubt Solving</h3>

<p>
Questions और doubts का समाधान।
</p>

</div>


<div class="feature">

<div class="feature-icon">🎯</div>

<h3>Exam Focus</h3>

<p>
Exam-oriented preparation strategy।
</p>

</div>


<div class="feature">

<div class="feature-icon">👥</div>

<h3>Limited Seats</h3>

<p>
Better attention के लिए limited batches।
</p>

</div>

</div>

</div>

</section>


<!-- CTA -->

<section class="cta">

<div class="container">

<h2>Your Success is Our Mission</h2>

<p>
आज ही S. R. Academy से जुड़ें और अपने
लक्ष्य की तैयारी शुरू करें।
</p>

<a href="https://wa.me/918958878452"
target="_blank"
class="btn btn-gold">

📲 Admission Enquiry

</a>

</div>

</section>


<!-- CONTACT -->

<section class="contact" id="contact">

<div class="container">

<div class="section-title">

<h2>Contact S. R. Academy</h2>

<p>
हमसे जुड़ें
</p>

</div>


<div class="contact-box">

<h3>S. R. Academy</h3>

<p>📞 <strong>8958878452</strong></p>

<p>
📱 WhatsApp पर Admission Enquiry के लिए संपर्क करें
</p>

<br>

<a href="https://wa.me/918958878452"
target="_blank"
class="btn btn-gold">

Chat on WhatsApp

</a>

</div>

</div>

</section>


<!-- FOOTER -->

<footer>

<h3>S. R. Academy</h3>

<p>The Way to Success</p>

<div class="footer-bottom">

© <span id="year"></span> S. R. Academy.
All Rights Reserved.

</div>

</footer>


<!-- WHATSAPP -->

<a href="https://wa.me/918958878452"
target="_blank"
class="whatsapp">

💬

</a>


<script>

function toggleMenu(){

    document
    .getElementById("navLinks")
    .classList
    .toggle("active");

}

document
.querySelectorAll(".nav-links a")
.forEach(function(link){

    link.addEventListener("click",function(){

        document
        .getElementById("navLinks")
        .classList
        .remove("active");

    });

});


document.getElementById("year")
.innerText = new Date().getFullYear();

</script>

</body>
</html>
