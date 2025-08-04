# Landing-page-cobaa2
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Landing Page Profesional</title>
    <style>
        /* Reset CSS */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: #333;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header */
        header {
            background-color: #fff;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: fixed;
            width: 100%;
            z-index: 100;
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            font-size: 24px;
            font-weight: 700;
            color: #2c3e50;
            text-decoration: none;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 30px;
        }
        
        .nav-links a {
            text-decoration: none;
            color: #2c3e50;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: #3498db;
        }
        
        .btn {
            display: inline-block;
            background-color: #3498db;
            color: white;
            padding: 10px 20px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 500;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #2980b9;
        }
        
        /* Hero Section */
        .hero {
            padding: 150px 0 100px;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            text-align: center;
        }
        
        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            color: #2c3e50;
        }
        
        .hero p {
            font-size: 20px;
            max-width: 700px;
            margin: 0 auto 30px;
            color: #7f8c8d;
        }
        
        .cta-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
        }
        
        .btn-secondary {
            background-color: transparent;
            color: #3498db;
            border: 2px solid #3498db;
        }
        
        .btn-secondary:hover {
            background-color: #3498db;
            color: white;
        }
        
        /* Features Section */
        .features {
            padding: 80px 0;
            background-color: white;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }
        
        .section-title h2 {
            font-size: 36px;
            color: #2c3e50;
            margin-bottom: 15px;
        }
        
        .section-title p {
            color: #7f8c8d;
            max-width: 600px;
            margin: 0 auto;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .feature-card {
            background-color: #f8f9fa;
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }
        
        .feature-icon {
            font-size: 50px;
            color: #3498db;
            margin-bottom: 20px;
        }
        
        .feature-card h3 {
            font-size: 22px;
            margin-bottom: 15px;
            color: #2c3e50;
        }
        
        /* Testimonials */
        .testimonials {
            padding: 80px 0;
            background-color: #f8f9fa;
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .testimonial-card {
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .testimonial-text {
            font-style: italic;
            margin-bottom: 20px;
            color: #7f8c8d;
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
        }
        
        .author-img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            margin-right: 15px;
            object-fit: cover;
        }
        
        .author-info h4 {
            color: #2c3e50;
            margin-bottom: 5px;
        }
        
        .author-info p {
            color: #7f8c8d;
            font-size: 14px;
        }
        
        /* CTA Section */
        .cta {
            padding: 100px 0;
            background: linear-gradient(135deg, #3498db 0%, #2c3e50 100%);
            color: white;
            text-align: center;
        }
        
        .cta h2 {
            font-size: 36px;
            margin-bottom: 20px;
        }
        
        .cta p {
            max-width: 600px;
            margin: 0 auto 30px;
            font-size: 18px;
            opacity: 0.9;
        }
        
        /* Footer */
        footer {
            background-color: #2c3e50;
            color: white;
            padding: 50px 0 20px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }
        
        .footer-column h3 {
            font-size: 18px;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-column h3::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 50px;
            height: 2px;
            background-color: #3498db;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a {
            color: #bdc3c7;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: #3498db;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
        }
        
        .social-links a {
            color: white;
            font-size: 20px;
            transition: color 0.3s;
        }
        
        .social-links a:hover {
            color: #3498db;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #bdc3c7;
            font-size: 14px;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .hero h1 {
                font-size: 36px;
            }
            
            .hero p {
                font-size: 18px;
            }
            
            .cta-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .btn {
                width: 100%;
                max-width: 250px;
                margin-bottom: 10px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav>
                <a href="#" class="logo">BrandName</a>
                <ul class="nav-links">
                    <li><a href="#">Beranda</a></li>
                    <li><a href="#">Fitur</a></li>
                    <li><a href="#">Harga</a></li>
                    <li><a href="#">Tentang Kami</a></li>
                    <li><a href="#" class="btn">Masuk</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Solusi Terbaik untuk Bisnis Anda</h1>
            <p>Tingkatkan produktivitas dan efisiensi bisnis Anda dengan solusi kami yang inovatif dan mudah digunakan.</p>
            <div class="cta-buttons">
                <a href="#" class="btn">Mulai Sekarang</a>
                <a href="#" class="btn btn-secondary">Pelajari Lebih Lanjut</a>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features">
        <div class="container">
            <div class="section-title">
                <h2>Fitur Unggulan</h2>
                <p>Kami menyediakan berbagai fitur yang dirancang untuk membantu bisnis Anda tumbuh lebih cepat</p>
            </div>
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">📊</div>
                    <h3>Analisis Data</h3>
                    <p>Dapatkan wawasan mendalam tentang bisnis Anda dengan alat analisis kami yang canggih.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">🤖</div>
                    <h3>Otomatisasi</h3>
                    <p>Otomatiskan proses bisnis yang berulang untuk menghemat waktu dan sumber daya.</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">📱</div>
                    <h3>Mobile Friendly</h3>
                    <p>Akses platform kami dari perangkat apa pun, kapan pun dan di mana pun.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="testimonials">
        <div class="container">
            <div class="section-title">
                <h2>Apa Kata Mereka</h2>
                <p>Lihat apa yang pelanggan kami katakan tentang pengalaman mereka menggunakan produk kami</p>
            </div>
            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <p class="testimonial-text">"Produk ini benar-benar mengubah cara kami menjalankan bisnis. Sangat mudah digunakan dan memberikan hasil yang luar biasa!"</p>
                    <div class="testimonial-author">
                        <img src="https://randomuser.me/api/portraits/women/32.jpg" alt="Author" class="author-img">
                        <div class="author-info">
                            <h4>Sarah Johnson</h4>
                            <p>CEO, TechCorp</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <p class="testimonial-text">"Dukungan pelanggan mereka luar biasa. Setiap pertanyaan dijawab dengan cepat dan solutif."</p>
                    <div class="testimonial-author">
                        <img src="https://randomuser.me/api/portraits/men/45.jpg" alt="Author" class="author-img">
                        <div class="author-info">
                            <h4>Michael Tan</h4>
                            <p>Direktur, Finansia</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <p class="testimonial-text">"Sejak menggunakan produk ini, efisiensi tim kami meningkat lebih dari 40%. Sangat direkomendasikan!"</p>
                    <div class="testimonial-author">
                        <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Author" class="author-img">
                        <div class="author-info">
                            <h4>Lisa Wang</h4>
                            <p>Manajer, RetailPlus</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="cta">
        <div class="container">
            <h2>Siap Mengubah Bisnis Anda?</h2>
            <p>Daftar sekarang dan dapatkan uji coba gratis selama 14 hari tanpa perlu kartu kredit.</p>
            <a href="#" class="btn">Daftar Sekarang</a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>BrandName</h3>
                    <p>Solusi inovatif untuk membantu bisnis Anda tumbuh lebih cepat dan lebih efisien.</p>
                    <div class="social-links">
                        <a href="#">📱</a>
                        <a href="#">📘</a>
                        <a href="#">📸</a>
                        <a href="#">🔗</a>
                    </div>
                </div>
                <div class="footer-column">
                    <h3>Perusahaan</h3>
                    <ul class="footer-links">
                        <li><a href="#">Tentang Kami</a></li>
                        <li><a href="#">Karir</a></li>
                        <li><a href="#">Blog</a></li>
                        <li><a href="#">Partner</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Produk</h3>
                    <ul class="footer-links">
                        <li><a href="#">Fitur</a></li>
                        <li><a href="#">Harga</a></li>
                        <li><a href="#">Integrasi</a></li>
                        <li><a href="#">Pembaruan</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Dukungan</h3>
                    <ul class="footer-links">
                        <li><a href="#">Bantuan</a></li>
                        <li><a href="#">Dokumentasi</a></li>
                        <li><a href="#">API</a></li>
                        <li><a href="#">Status</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 BrandName. Seluruh hak cipta dilindungi.</p>
            </div>
        </div>
    </footer>
</body>
</html>
