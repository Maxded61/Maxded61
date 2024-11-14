<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ömer Türkay - Portföy</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <!-- Navbar -->
    <nav>
        <div class="container">
            <h1 class="logo">Ömer Türkay</h1>
            <ul>
                <li><a href="#about">Hakkımda</a></li>
                <li><a href="#services">Hizmetler</a></li>
                <li><a href="#contact">İletişim</a></li>
            </ul>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1>Merhaba, Ben Ömer Türkay</h1>
            <p>Web Geliştirici ve Yazılım Mühendisi</p>
            <a href="#services" class="cta-btn">Hizmetlerimi Gör</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="section">
        <div class="container">
            <h2>Hakkımda</h2>
            <p>Ben, web teknolojileri ve yazılım geliştirme alanında deneyimli bir profesyonelim. Yaratıcı projeler üzerinde çalışmayı seviyorum ve her zaman yeni şeyler öğrenmeye açığım. Takım çalışmasına yatkınım ve verimli çözümler üretmeye odaklanırım.</p>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="section services-section">
        <div class="container">
            <h2>Hizmetlerim</h2>
            <div class="services">
                <div class="service">
                    <h3>Web Geliştirme</h3>
                    <p>Modern, kullanıcı dostu ve mobil uyumlu web siteleri geliştiriyorum.</p>
                </div>
                <div class="service">
                    <h3>Uygulama Geliştirme</h3>
                    <p>Mobil ve masaüstü uygulama geliştirme konusunda derinlemesine deneyime sahibim.</p>
                </div>
                <div class="service">
                    <h3>SEO Optimizasyonu</h3>
                    <p>Web sitenizin arama motorlarında üst sıralara çıkmasına yardımcı olacak SEO çözümleri sunuyorum.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section contact-section">
        <div class="container">
            <h2>İletişim</h2>
            <form action="#">
                <label for="name">Adınız:</label>
                <input type="text" id="name" name="name" required>

                <label for="email">E-posta:</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Mesajınız:</label>
                <textarea id="message" name="message" required></textarea>

                <button type="submit" class="cta-btn">Gönder</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>© 2024 Ömer Türkay. Tüm Hakları Saklıdır.</p>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>
/* Genel stil ayarları */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Arial', sans-serif;
}

body {
    background-color: #f7f7f7;
    color: #333;
    line-height: 1.6;
}

/* Navbar stil ayarları */
nav {
    background-color: #007BFF;
    color: white;
    padding: 20px 0;
}

nav .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

nav .logo {
    font-size: 26px;
    font-weight: bold;
}

nav ul {
    list-style: none;
    display: flex;
}

nav ul li {
    margin: 0 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
    transition: color 0.3s ease;
}

nav ul li a:hover {
    color: #FFD700;
}

/* Hero Section */
.hero {
    background: url('https://source.unsplash.com/1600x900/?technology,web') center/cover no-repeat;
    color: white;
    height: 80vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    position: relative;
}

.hero-content {
    position: absolute;
    z-index: 1;
}

.hero h1 {
    font-size: 48px;
    margin-bottom: 20px;
}

.hero p {
    font-size: 24px;
    margin-bottom: 20px;
}

.cta-btn {
    background-color: #FFD700;
    color: #333;
    padding: 12px 30px;
    text-decoration: none;
    border-radius: 25px;
    font-size: 18px;
    transition: background-color 0.3s ease;
}

.cta-btn:hover {
    background-color: #ffbf00;
}

/* Section stil ayarları */
.section {
    padding: 60px 0;
    text-align: center;
}

.section h2 {
    font-size: 36px;
    margin-bottom: 40px;
    color: #333;
}

/* About Section */
#about p {
    max-width: 800px;
    margin: 0 auto;
    font-size: 18px;
    line-height: 1.6;
}

/* Hizmetler Section */
.services-section {
    background-color: #f2f2f2;
}

.services {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    gap: 30px;
}

.service {
    background-color: #fff;
    padding: 30px;
    border-radius: 8px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    width: 30%;
    min-width: 250px;
    transition: transform 0.3s ease;
}

.service:hover {
    transform: translateY(-10px);
}

.service h3 {
    font-size: 24px;
    margin-bottom: 15px;
}

.service p {
    font-size: 16px;
    color: #555;
}

/* İletişim Bölümü */
.contact-section {
    background-color: #007BFF;
    color: white;
}

form {
    display: grid;
    grid-gap: 20px;
    max-width: 600px;
    margin: 0 auto;
}

form label {
    font-size: 18px;
}

form input, form textarea {
    padding: 15px;
    font-size: 16px;
    border: 1px solid #ddd;
    border-radius: 5px;
    width: 100%;
}

form button {
    background-color: #FFD700;
    color: #333;
    padding: 12px 30px;
    font-size: 18px;
    border: none;
    border-radius: 25px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

form button:hover {
    background-color: #ffbf00;
}

/* Footer */
footer {
    background-color: #333;
    color: white;
    padding: 20px 0;
    text-align: center;
}
