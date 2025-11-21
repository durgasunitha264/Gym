<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FitLife Gym</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navigation Bar -->
    <header>
        <nav>
            <h1 class="logo">FitLife Gym</h1>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#facilities">Facilities</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#plans">Membership</a></li>
            </ul>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home" class="section hero">
        <div class="hero-content">
            <h2>Transform Your Body & Mind</h2>
            <p>Join our state-of-the-art fitness center today!</p>
            <button onclick="scrollToSection('plans')">Join Now</button>
        </div>
    </section>

    <!-- Facilities Section -->
    <section id="facilities" class="section">
        <h2 class="section-title">Our Facilities</h2>
        <div class="cards">
            <div class="card">
                <img src="https://via.placeholder.com/300x180" alt="Gym Floor">
                <h3>Modern Gym Floor</h3>
                <p>Fully equipped with latest machines and free weights.</p>
            </div>
            <div class="card">
                <img src="https://via.placeholder.com/300x180" alt="Swimming Pool">
                <h3>Swimming Pool</h3>
                <p>Indoor heated pool for training and relaxation.</p>
            </div>
            <div class="card">
                <img src="https://via.placeholder.com/300x180" alt="Sauna">
                <h3>Sauna</h3>
                <p>Detox and relax in our premium sauna rooms.</p>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="section alt-bg">
        <h2 class="section-title">Our Services</h2>
        <div class="cards">
            <div class="card">
                <h3>Personal Training</h3>
                <p>Work with certified trainers to achieve your goals.</p>
            </div>
            <div class="card">
                <h3>Group Classes</h3>
                <p>Yoga, Zumba, HIIT, Pilates, CrossFit & more.</p>
            </div>
            <div class="card">
                <h3>Nutrition Plans</h3>
                <p>Custom diet plans designed by professional nutritionists.</p>
            </div>
        </div>
    </section>

    <!-- Membership Plans Section -->
    <section id="plans" class="section">
        <h2 class="section-title">Membership Plans</h2>

        <div class="plans">
            <div class="plan">
                <h3>Basic</h3>
                <h4>$29 / month</h4>
                <ul>
                    <li>Gym Access</li>
                    <li>Locker Facility</li>
                    <li>1 Group Class Weekly</li>
                </ul>
                <button class="btn">Choose Plan</button>
            </div>

            <div class="plan popular">
                <h3>Standard</h3>
                <h4>$49 / month</h4>
                <ul>
                    <li>Full Gym Access</li>
                    <li>Swimming Pool</li>
                    <li>Unlimited Group Classes</li>
                    <li>Sauna Access</li>
                </ul>
                <button class="btn">Choose Plan</button>
            </div>

            <div class="plan">
                <h3>Premium</h3>
                <h4>$79 / month</h4>
                <ul>
                    <li>All Standard Benefits</li>
                    <li>Personal Trainer</li>
                    <li>Nutrition Consultation</li>
                </ul>
                <button class="btn">Choose Plan</button>
            </div>
        </div>
    </section>

    <footer>
        <p>© 2025 FitLife Gym. All Rights Reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
📌 style.css
css
Copy code
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    scroll-behavior: smooth;
}

/* Navigation */
header {
    background: #111;
    padding: 15px 0;
    position: fixed;
    width: 100%;
    z-index: 1000;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 90%;
    margin: auto;
}

.logo {
    color: #fff;
    font-size: 25px;
    font-weight: bold;
}

.nav-links {
    list-style: none;
}

.nav-links li {
    display: inline-block;
    margin-left: 20px;
}

.nav-links a {
    color: #fff;
    text-decoration: none;
    transition: 0.3s;
}

.nav-links a:hover {
    color: #f4a835;
}

/* Hero Section */
.hero {
    background: url('https://via.placeholder.com/1200x600') center/cover;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: white;
}

.hero-content h2 {
    font-size: 45px;
    margin-bottom: 10px;
}

.hero button {
    padding: 12px 25px;
    margin-top: 15px;
    border: none;
    background: #f4a835;
    color: black;
    font-size: 18px;
    cursor: pointer;
    transition: 0.3s;
}

.hero button:hover {
    background: #fff;
}

/* Sections */
.section {
    padding: 80px 10%;
}

.alt-bg {
    background: #f8f8f8;
}

.section-title {
    text-align: center;
    font-size: 32px;
    margin-bottom: 40px;
}

/* Cards */
.cards {
    display: flex;
    gap: 30px;
    flex-wrap: wrap;
    justify-content: center;
}

.card {
    background: white;
    width: 300px;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    text-align: center;
}

.card img {
    width: 100%;
    border-radius: 10px;
    margin-bottom: 15px;
}

/* Membership Plans */
.plans {
    display: flex;
    justify-content: center;
    gap: 30px;
    flex-wrap: wrap;
}

.plan {
    background: white;
    padding: 25px;
    width: 260px;
    text-align: center;
    border-radius: 10px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.plan.popular {
    border: 2px solid #f4a835;
}

.plan h4 {
    margin: 10px 0;
    color: #f4a835;
}

.plan ul {
    list-style: none;
    margin: 15px 0;
}

.plan li {
    margin: 8px 0;
}

.btn {
    background: #f4a835;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
    transition: 0.3s;
}

.btn:hover {
    background: #111;
    color: white;
}

/* Footer */
footer {
    background: #111;
    color: #fff;
    text-align: center;
    padding: 20px;
}
📌 script.js
javascript
Copy code
// Smooth scroll when clicking "Join Now"
function scrollToSection(id) {
    document.getElementById(id).scrollIntoView({ behavior: "smooth" });
}

