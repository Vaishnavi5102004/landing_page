# landing_page
This is my code of html and css used for project
#HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Creative Landing Page</title>
    <link rel="stylesheet" href="landingpage.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">InnoDesigns</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#features">Features</a></li>
                <li><a href="#gallery">Gallery</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <a href="#cta" class="cta">Sign Up</a>
        </nav>
    </header>

   <section class="hero">
        <h1>Welcome to InnoDesigns</h1>
        <p>Crafting elegance and innovation, your vision brought to life.</p>
        <a href="#features" class="cta-button">Explore More</a>
    </section>

   <section id="features" class="features">
        <h2>Our Features</h2>
        <div class="feature-grid">
            <div class="feature-item">Design Excellence</div>
            <div class="feature-item">Responsive Layouts</div>
            <div class="feature-item">Dynamic Animations</div>
            <div class="feature-item">Fast & Secure</div>
        </div>
    </section>

   <footer>
        <p>&copy; 2024 InnoDesigns | All Rights Reserved</p>
    </footer>
</body>
</html>

#CSS
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Arial', sans-serif;
}

body {
    color: #2d2d2d;
    line-height: 1.6;
}

header {
    background: linear-gradient(45deg, #FF416C, #FF4B2B);
    color: #fff;
    padding: 15px 0;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 100;
}

nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

.logo {
    font-size: 24px;
    font-weight: bold;
}

.nav-links {
    list-style: none;
    display: flex;
}

.nav-links li {
    margin-left: 20px;
}

.nav-links a, .cta {
    color: #fff;
    text-decoration: none;
    font-size: 16px;
}

.cta {
    padding: 8px 15px;
    background-color: #00C9A7;
    border-radius: 5px;
}

.hero {
    background: linear-gradient(45deg, #00C9A7, #92FE9D);
    color: #fff;
    text-align: center;
    padding: 120px 20px 100px;
    margin-top: 60px;
}

.hero h1 {
    font-size: 50px;
    font-weight: bold;
    animation: fadeInDown 1s ease-out;
}

.hero p {
    font-size: 20px;
    margin: 15px 0 20px;
}

.cta-button {
    background-color: #FF416C;
    padding: 10px 20px;
    color: #fff;
    font-size: 18px;
    border: none;
    border-radius: 5px;
    text-decoration: none;
    animation: bounce 1.5s infinite;
}

.features {
    background-color: #f9f9f9;
    padding: 60px 20px;
    text-align: center;
}

.features h2 {
    font-size: 32px;
    margin-bottom: 30px;
    color: #333;
}

.feature-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
    margin-top: 20px;
}

