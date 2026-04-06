<!DOCTYPE html>
<html>
<head>
<title>CODExASHU</title>

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>

body {
    background: black;
    color: white;
    font-family: Arial;
    margin: 0;
}

/* HEADER */
header {
    text-align: center;
    padding: 15px;
    font-size: 22px;
    border-bottom: 1px solid red;
}

/* NAVBAR */
nav {
    text-align: center;
    padding: 10px;
}

.btn {
    display: inline-block;
    margin: 8px;
    padding: 10px 20px;
    border: 2px solid red;
    color: red;
    border-radius: 10px;
    cursor: pointer;
}

.btn:hover {
    background: red;
    color: white;
}

/* SECTION CENTER FIX */
.container {
    max-width: 900px;
    margin: auto;
    padding: 20px;
    text-align: center;
}

section {
    display: none;
}

#home {
    display: block;
}

.glow {
    color: red;
    font-size: 32px;
    text-shadow: 0 0 10px red, 0 0 20px red;
}

.box {
    border: 1px solid red;
    padding: 20px;
    border-radius: 10px;
    margin-top: 20px;
}

img {
    width: 100%;
    max-width: 300px;
    border-radius: 10px;
}

/* FOOTER */
footer {
    text-align: center;
    margin-top: 30px;
    padding: 10px;
    border-top: 1px solid red;
}

/* RESPONSIVE */
@media (max-width: 600px) {
    .glow {
        font-size: 24px;
    }

    .btn {
        padding: 8px 12px;
        font-size: 14px;
    }
}

</style>
</head>

<body>

<header>
💻 CODExASHU
</header>

<nav>
<span class="btn" onclick="showSection('home')">HOME</span>
<span class="btn" onclick="showSection('services')">SERVICES</span>
<span class="btn" onclick="showSection('about')">ABOUT</span>
<span class="btn" onclick="showSection('contact')">CONTACT</span>
<span class="btn" onclick="showSection('careers')">STAFF</span>
</nav>

<!-- HOME -->
<section id="home">
<div class="container">

<h2>Premium Developing Service</h2>
<div class="glow">Welcome to codexashu™</div>

<div class="box">
<h2>I Create. I Secure. I Deliver.</h2>

<p>I’m a Professional Web Developer, App Developer, and Ethical Hacker.</p>
<p>I build modern websites, powerful mobile apps, and secure systems.</p>
<p>Need a website, app, or security solution? You're in the right place.</p>

</div>

</div>
</section>

<!-- SERVICES -->
<section id="services">
<div class="container">

<h1>Our Services</h1>

<div class="box" onclick="showService('web')">💻 WEB DEVELOPING</div>
<div class="box" onclick="showService('app')">📱 APP DEVELOPING</div>
<div class="box" onclick="showService('hack')">🔐 ETHICAL HACKING</div>

<div id="serviceBox" style="display:none;">
    <h2 id="title"></h2>
    <img id="image">
    <p id="desc"></p>
</div>

</div>
</section>

<!-- ABOUT -->
<section id="about">
<div class="container">

<h1>About Me</h1>

<div class="box">
<p>I build powerful websites, apps, and secure systems.</p>
<p>I don’t just create — I solve real problems.</p>
</div>

</div>
</section>

<!-- CONTACT -->
<section id="contact">
<div class="container">

<h1>Contact</h1>

<div class="box">
<p>📞 WhatsApp: 9919667539</p>
<p>📧 Email: your@email.com</p>
</div>

</div>
</section>

<!-- CAREERS -->
<section id="careers">
<div class="container">

<h1>Join Us</h1>

<div class="box">
<p>If you want to work with us, contact on WhatsApp.</p>
</div>

</div>
</section>

<footer>
© 2026 CODExASHU
</footer>

<script>

function showSection(id) {
    document.querySelectorAll("section").forEach(sec => sec.style.display = "none");
    document.getElementById(id).style.display = "block";
}

function showService(type) {
    document.getElementById("serviceBox").style.display = "block";

    if(type === 'web') {
        title.innerText = "WEB DEVELOPMENT";
        desc.innerText = "Professional websites starting from $50";
    }

    if(type === 'app') {
        title.innerText = "APP DEVELOPMENT";
        desc.innerText = "Android apps starting from $99";
    }

    if(type === 'hack') {
        title.innerText = "SECURITY SERVICES";
        desc.innerText = "Ethical hacking & security testing";
    }
}

</script>

</body>
</html>
