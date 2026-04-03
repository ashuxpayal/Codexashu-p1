<!DOCTYPE html>
<html>
<head>
    <title>CODExASHU</title>

    <style>
        body {
            background: WHITE;
            color: BLACK;
            text-align: center;
            font-family: Arial;
            margin: 0;
        }

        header {
            background: WHITE;
            padding: 15px;
            font-size: 22px;
            border-bottom: 1px solid BLUE;
        }

        nav {
            margin-top: 10px;
        }

        .btn {
            display: inline-block;
            margin: 10px;
            padding: 10px 20px;
            border: 2px solid BLUE;
            color: BLUE;
            text-decoration: none;
            border-radius: 10px;
            cursor: pointer;
        }

        .btn:hover {
            background: BLUE;
            color: WHITE;
        }

        section {
            display: none;
            padding: 20px;
        }

        #home {
            display: block;
        }

        .glow {
            color: BLUE;
            font-size: 35px;
            text-shadow: 0 0 10px BLUE, 0 0 20px BLUE;
        }

        .box {
            border: 1px solid BLUE;
            margin: 20px;
            padding: 20px;
            border-radius: 10px;
        }

        img {
            width: 250px;
            margin-top: 10px;
            border-radius: 10px;
        }

        footer {
            margin-top: 30px;
            padding: 10px;
            border-top: 1px solid BLUE;
        }
    </style>
</head>

<body>

<header>
    💻CODExASHU
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
    <h1>Premium developing servicE</h1>
    <div class="glow">Welcome to codexashu™</div>
    <p><h1> I Create. I Secure. I Deliver.</h1><p>
(1) I’m a Professional Web Developer, App Developer, and Ethical Hacker.
I build modern websites, powerful mobile apps, and secure digital systems that people trust.
</p><p>
(2) From idea to execution — I turn concepts into reality with clean design, smooth performance, and strong security.
</p><p>
(3) Need a website, app, or security solution? You’re in the right place.
</p>   </p>
</section>

<!-- SERVICES -->
<section id="services">
    <h1>Our Services</h1>

    <div class="box">
        <p onclick="showService('web')">💻WEB DEVELOPING </p>
        <p onclick="showService('hack')">💻APP DEVELOPING </p>
        <p onclick="showService('data')">💻ETHICAL HACKING </p>
    </div>

    <!-- Service Details -->
    <div id="serviceBox" style="display:none;">
        <h2 id="title"></h2>
        <img id="image">
        <p id="desc"></p>
    </div>
</section>

<!-- ABOUT -->
<section id="about">
    <h1>About Us</h1>
    <p>👉 I build powerful websites, smart mobile apps, and secure systems.

I’m a Web Developer, App Developer, and Ethical Hacker who doesn’t just create — I solve real problems. From designing modern websites to developing smooth apps and securing digital platforms, I handle it all.

If you want your project done right, fast, and secure — you come to me.</p>
</section>

<!-- CONTACT -->
<section id="contact">
    <h1>Contact Us</h1>
    <p>📞 whatsapp:- 9919667539</p>
    <p>📧 Email: ashutosh.8887.my@email.com</p>
</section>

<!-- CAREERS -->
<section id="careers">
    <h1>NEED</h1>
    <p>👉  Staff Need:- If you want to work with us then message us on 
WhatsApp:- 9919667539</p>
</section>

<footer>
    © 2026 CODExASHU
</footer>

<script>
function showSection(id) {
    let sections = document.querySelectorAll("section");
    sections.forEach(sec => sec.style.display = "none");

    document.getElementById(id).style.display = "block";
}

function showService(type) {
    document.getElementById("serviceBox").style.display = "block";

    if(type === 'web') {
        title.innerText = "50% OFF";
        image.src = "WEB.jpg";
        desc.innerText = "I AM CREATING BEST AND SMOOTH WEBSITE WITH CLEAR AND BEST DESIGN     [START :- $50]";
    }

    if(type === 'hack') {
        title.innerText = "APP DEVELOPE";
        image.src = "APP.jpg";
        desc.innerText = "I AM CREATING BEST AND SMOOTH ANDROID APP AND APK             [START :- $99]";
    }

    if(type === 'data') {
        title.innerText = "ethical hacker";
        image.src = "ETHICAL HACKING.jpg";
        desc.innerText = "per work charge         [startig :- $99]";
    }
}
</script>

</body>
</html>
