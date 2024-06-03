<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Navigation Menu</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

<header>
    <nav id="navbar">
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>

<div class="content">
    <section id="home"><h1>Home Section</h1></section>
    <section id="about"><h1>About Section</h1></section>
    <section id="services"><h1>Services Section</h1></section>
    <section id="contact"><h1>Contact Section</h1></section>
</div>

<script src="script.js"></script>
</body>
</html>
/*css.
body, html {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
}

header {
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
}

#navbar {
    background-color: #333;
    overflow: hidden;
}

#navbar ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}

#navbar ul li {
    float: left;
}

#navbar ul li a {
    display: block;
    color: white;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
    transition: background-color 0.3s;
}

#navbar ul li a:hover {
    background-color: #575757;
}

.scrolled #navbar {
    background-color: #444;
    transition: background-color 0.3s;
}

.content {
    padding: 100px 20px;
}

section {
    padding: 60px 0;
    min-height: 100vh;
}
/* js.
window.onscroll = function() {
    var navbar = document.getElementById("navbar");
    if (document.body.scrollTop > 50 || document.documentElement.scrollTop > 50) {
        navbar.classList.add("scrolled");
    } else {
        navbar.classList.remove("scrolled");
    }
};
