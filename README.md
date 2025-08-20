# tirupatigold.com
website 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tirupati Gold - Exquisite Gold Jewelry Collection</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Georgia', serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #f5f3f0 0%, #fff9f5 100%);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        header {
            background: linear-gradient(135deg, #b8860b 0%, #daa520 50%, #ffd700 100%);
            color: white;
            padding: 1rem 0;
            box-shadow: 0 4px 20px rgba(184, 134, 11, 0.3);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        .logo {
            font-size: 2.5rem;
            font-weight: bold;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            background: linear-gradient(45deg, #fff, #fffacd);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .gst-info {
            font-size: 0.9rem;
            opacity: 0.9;
            text-align: right;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 2rem;
            margin-top: 1rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            padding: 0.5rem 1rem;
            border-radius: 25px;
        }

        nav a:hover {
            background: rgba(255,255,255,0.2);
            transform: translateY(-2px);
        }

        .hero {
            text-align: center;
            padding: 4rem 0;
            background: radial-gradient(ellipse at center, #fff9e6 0%, #f5f3f0 70%);
        }

        .hero h1 {
            font-size: 3rem;
            color: #b8860b;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
        }

        .hero p {
            font-size: 1.3rem;
            color: #666;
            max-width: 600px;
            margin: 0 auto 2rem;
        }

        .section {
            padding: 4rem 0;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            color: #b8860b;
            margin-bottom: 3rem;
            position: relative;
        }

        .section-title::after {
            content: '';
            width: 100px;
            height: 3px;
            background: linear-gradient(45deg, #b8860b, #daa520);
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .jewelry-card {
            background: white;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(184, 134, 11, 0.1);
            transition: all 0.3s ease;
            position: relative;
        }

        .jewelry-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(184, 134, 11, 0.2);
        }

        .jewelry-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(135deg, transparent 0%, rgba(184, 134, 11, 0.05) 100%);
            pointer-events: none;
        }

        .card-image {
            width: 100%;
            height: 300px;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .jewelry-card:hover .card-image {
            transform: scale(1.05);
        }

        .card-content {
            padding: 1.5rem;
        }

        .card-title {
            font-size: 1.3rem;
            color: #b8860b;
            margin-bottom: 0.5rem;
            font-weight: 600;
        }

        .card-description {
            color: #666;
            font-size: 0.95rem;
            line-height: 1.5;
        }

        .about {
            background: linear-gradient(135deg, #fff 0%, #f9f7f4 100%);
            border-radius: 20px;
            padding: 3rem;
            margin: 2rem 0;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        .about-text {
            font-size: 1.1rem;
            line-height: 1.8;
            color: #555;
        }

        .features {
            list-style: none;
            margin-top: 1rem;
        }

        .features li {
            padding: 0.5rem 0;
            position: relative;
            padding-left: 2rem;
            color: #666;
        }

        .features li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: #b8860b;
            font-weight: bold;
            font-size: 1.2rem;
        }

        .contact {
            background: linear-gradient(135deg, #b8860b 0%, #daa520 100%);
            color: white;
            text-align: center;
            border-radius: 20px;
            margin: 2rem 0;
            padding: 3rem;
        }

        .contact h2 {
            font-size: 2rem;
            margin-bottom: 1rem;
        }

        .contact-info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .contact-item {
            background: rgba(255,255,255,0.1);
            padding: 1.5rem;
            border-radius: 15px;
            backdrop-filter: blur(10px);
        }

        footer {
            background: #2c2c2c;
            color: white;
            text-align: center;
            padding: 2rem 0;
            margin-top: 2rem;
        }

        .gst-footer {
            margin-top: 1rem;
            font-size: 0.9rem;
            opacity: 0.8;
            border-top: 1px solid #444;
            padding-top: 1rem;
        }

        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .hero p {
                font-size: 1.1rem;
            }
            
            .gallery {
                grid-template-columns: 1fr;
            }
            
            .about-content {
                grid-template-columns: 1fr;
            }
            
            nav ul {
                flex-direction: column;
                gap: 1rem;
            }
            
            .header-content {
                text-align: center;
            }
        }

        .floating-elements {
            position: fixed;
            pointer-events: none;
            z-index: -1;
        }

        .floating-gold {
            position: absolute;
            width: 20px;
            height: 20px;
            background: radial-gradient(circle, #ffd700, #b8860b);
            border-radius: 50%;
            opacity: 0.1;
            animation: float 6s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(180deg); }
        }

        .specialty-section {
            background: linear-gradient(45deg, #fff8e1 0%, #f3e5ab 100%);
            border-radius: 20px;
            padding: 3rem;
            margin: 2rem 0;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="floating-elements">
        <div class="floating-gold" style="top: 10%; left: 10%; animation-delay: 0s;"></div>
        <div class="floating-gold" style="top: 20%; right: 15%; animation-delay: 1s;"></div>
        <div class="floating-gold" style="top: 60%; left: 20%; animation-delay: 2s;"></div>
        <div class="floating-gold" style="bottom: 20%; right: 10%; animation-delay: 3s;"></div>
    </div>

    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">Tirupati Gold</div>
                <div class="gst-info">
                    GST: 27EEAPM1945A1ZV<br>
                    Premium Gold Jewelry
                </div>
            </div>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#collection">Collection</a></li>
                    <li><a href="#about">About Us</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="home" class="hero">
        <div class="container">
            <h1>Exquisite Gold Jewelry</h1>
            <p>Discover our premium collection of traditional and contemporary gold jewelry, crafted with precision and passion for over generations.</p>
        </div>
    </section>

    <section id="collection" class="section">
        <div class="container">
            <h2 class="section-title">Our Premium Collection</h2>
            
            <div class="gallery">
                <div class="jewelry-card">
                    <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDAwIiBoZWlnaHQ9IjMwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48ZGVmcz48bGluZWFyR3JhZGllbnQgaWQ9ImdvbGRHcmFkaWVudCIgeDE9IjAlIiB5MT0iMCUiIHgyPSIxMDAlIiB5Mj0iMTAwJSI+PHN0b3Agb2Zmc2V0PSIwJSIgc3R5bGU9InN0b3AtY29sb3I6I2ZmZDcwMDtzdG9wLW9wYWNpdHk6MSIgLz48c3RvcCBvZmZzZXQ9IjEwMCUiIHN0eWxlPSJzdG9wLWNvbG9yOiNiODg2MGI7c3RvcC1vcGFjaXR5OjEiIC8+PC9saW5lYXJHcmFkaWVudD48L2RlZnM+PHJlY3Qgd2lkdGg9IjEwMCUiIGhlaWdodD0iMTAwJSIgZmlsbD0idXJsKCNnb2xkR3JhZGllbnQpIi8+PGNpcmNsZSBjeD0iMjAwIiBjeT0iMTUwIiByPSI4MCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjZmZmIiBzdHJva2Utd2lkdGg9IjMiLz48Y2lyY2xlIGN4PSIyMDAiIGN5PSIxNTAiIHI9IjMwIiBmaWxsPSIjZmZmIi8+PC9zdmc+" alt="Elegant Mangalsutra" class="card-image">
                    <div class="card-content">
                        <h3 class="card-title">Traditional Mangalsutra</h3>
                        <p class="card-description">Elegant black bead mangalsutra with intricate gold leaf pendant, perfect for modern brides who appreciate traditional craftsmanship.</p>
                    </div>
                </div>

                <div class="jewelry-card">
                    <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDAwIiBoZWlnaHQ9IjMwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48ZGVmcz48bGluZWFyR3JhZGllbnQgaWQ9ImdvbGRHcmFkaWVudDIiIHgxPSIwJSIgeTE9IjAlIiB4Mj0iMTAwJSIgeTI9IjEwMCUiPjxzdG9wIG9mZnNldD0iMCUiIHN0eWxlPSJzdG9wLWNvbG9yOiNkYWE1MjA7c3RvcC1vcGFjaXR5OjEiIC8+PHN0b3Agb2Zmc2V0PSIxMDAlIiBzdHlsZT0ic3RvcC1jb2xvcjojYjg4NjBiO3N0b3Atb3BhY2l0eToxIiAvPjwvbGluZWFyR3JhZGllbnQ+PC9kZWZzPjxyZWN0IHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiIGZpbGw9InVybCgjZ29sZEdyYWRpZW50MikiLz48Y2lyY2xlIGN4PSIxNTAiIGN5PSIxMjAiIHI9IjI1IiBmaWxsPSIjZmZmIiBzdHJva2U9IiNmZmQiIHN0cm9rZS13aWR0aD0iMiIvPjxjaXJjbGUgY3g9IjI1MCIgY3k9IjEyMCIgcj0iMjUiIGZpbGw9IiNmZmYiIHN0cm9rZT0iI2ZmZCIgc3Ryb2tlLXdpZHRoPSIyIi8+PGxpbmUgeDE9IjUwIiB5MT0iMTgwIiB4Mj0iMzUwIiB5Mj0iMTgwIiBzdHJva2U9IiNmZmYiIHN0cm9rZS13aWR0aD0iNCIvPjwvc3ZnPg==" alt="Gold Chain Collection" class="card-image">
                    <div class="card-content">
                        <h3 class="card-title">Premium Gold Chains</h3>
                        <p class="card-description">Stunning collection of gold chains with decorative beads and intricate patterns, showcasing exceptional craftsmanship.</p>
                    </div>
                </div>

                <div class="jewelry-card">
                    <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDAwIiBoZWlnaHQ9IjMwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48ZGVmcz48bGluZWFyR3JhZGllbnQgaWQ9ImdvbGRHcmFkaWVudDMiIHgxPSIwJSIgeTE9IjAlIiB4Mj0iMTAwJSIgeTI9IjEwMCUiPjxzdG9wIG9mZnNldD0iMCUiIHN0eWxlPSJzdG9wLWNvbG9yOiNmZmQ3MDA7c3RvcC1vcGFjaXR5OjEiIC8+PHN0b3Agb2Zmc2V0PSIxMDAlIiBzdHlsZT0ic3RvcC1jb2xvcjojZGFhNTIwO3N0b3Atb3BhY2l0eToxIiAvPjwvbGluZWFyR3JhZGllbnQ+PC9kZWZzPjxyZWN0IHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiIGZpbGw9InVybCgjZ29sZEdyYWRpZW50MykiLz48cGF0aCBkPSJNMjAwIDgwIEwxNzAgMTIwIEwxNDAgMTAwIEwxNzAgMTQwIEwxNDAgMTgwIEwxNzAgMTYwIEwyMDAgMjAwIEwyMzAgMTYwIEwyNjAgMTgwIEwyMzAgMTQwIEwyNjAgMTAwIEwyMzAgMTIwIFoiIGZpbGw9IiNmZmYiIHN0cm9rZT0iI2ZmZiIgc3Ryb2tlLXdpZHRoPSIyIi8+PC9zdmc+" alt="Floral Pendant" class="card-image">
                    <div class="card-content">
                        <h3 class="card-title">Designer Floral Pendant</h3>
                        <p class="card-description">Beautiful floral design pendant with delicate hanging elements, perfect for special occasions and daily elegance.</p>
                    </div>
                </div>

                <div class="jewelry-card">
                    <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDAwIiBoZWlnaHQ9IjMwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48ZGVmcz48bGluZWFyR3JhZGllbnQgaWQ9ImdvbGRHcmFkaWVudDQiIHgxPSIwJSIgeTE9IjAlIiB4Mj0iMTAwJSIgeTI9IjEwMCUiPjxzdG9wIG9mZnNldD0iMCUiIHN0eWxlPSJzdG9wLWNvbG9yOiNmZmQ3MDA7c3RvcC1vcGFjaXR5OjEiIC8+PHN0b3Agb2Zmc2V0PSIxMDAlIiBzdHlsZT0ic3RvcC1jb2xvcjojYjg4NjBiO3N0b3Atb3BhY2l0eToxIiAvPjwvbGluZWFyR3JhZGllbnQ+PC9kZWZzPjxyZWN0IHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiIGZpbGw9InVybCgjZ29sZEdyYWRpZW50NCkiLz48cGF0aCBkPSJNMTYwIDEyMCBDMTYwIDEwMCAxODAgODAgMjAwIDgwIEMyMjAgODAgMjQwIDEwMCAyNDAgMTIwIEMyNDAgMTQwIDIyMCAxNjAgMjAwIDE4MCBDMTU1IDE2NSAxNTUgMTM1IDE2MCAxMjBaIiBmaWxsPSJub25lIiBzdHJva2U9IiNmZmYiIHN0cm9rZS13aWR0aD0iNCIvPjxwYXRoIGQ9Ik0yNDAgMTIwIEMyNjAgMTIwIDI4MCAxMDAgMzAwIDEyMCBDMjgwIDE0MCAyNjAgMTYwIDI0MCAxNDAiIGZpbGw9Im5vbmUiIHN0cm9rZT0iI2ZmZiIgc3Ryb2tlLXdpZHRoPSI0Ii8+PC9zdmc+" alt="Heart Pendant Collection" class="card-image">
                    <div class="card-content">
                        <h3 class="card-title">Diamond Heart Pendant</h3>
                        <p class="card-description">Romantic heart-shaped pendant adorned with sparkling cubic zirconia, symbolizing love and elegance in perfect harmony.</p>
                    </div>
                </div>

                <div class="jewelry-card">
                    <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDAwIiBoZWlnaHQ9IjMwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48ZGVmcz48bGluZWFyR3JhZGllbnQgaWQ9ImdvbGRHcmFkaWVudDUiIHgxPSIwJSIgeTE9IjAlIiB4Mj0iMTAwJSIgeTI9IjEwMCUiPjxzdG9wIG9mZnNldD0iMCUiIHN0eWxlPSJzdG9wLWNvbG9yOiNkYWE1MjA7c3RvcC1vcGFjaXR5OjEiIC8+PHN0b3Agb2Zmc2V0PSIxMDAlIiBzdHlsZT0ic3RvcC1jb2xvcjojYjg4NjBiO3N0b3Atb3BhY2l0eToxIiAvPjwvbGluZWFyR3JhZGllbnQ+PC9kZWZzPjxyZWN0IHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiIGZpbGw9InVybCgjZ29sZEdyYWRpZW50NSkiLz48ZWxsaXBzZSBjeD0iMjAwIiBjeT0iMTIwIiByeD0iODAiIHJ5PSI0MCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjZmZmIiBzdHJva2Utd2lkdGg9IjMiLz48Y2lyY2xlIGN4PSIxNTAiIGN5PSIxMjAiIHI9IjE1IiBmaWxsPSIjZmZmIi8+PGNpcmNsZSBjeD0iMjUwIiBjeT0iMTIwIiByPSIxNSIgZmlsbD0iI2ZmZiIvPjxjaXJjbGUgY3g9IjIwMCIgY3k9IjE4MCIgcj0iMjAiIGZpbGw9IiNmZmYiLz48L3N2Zz4=" alt="Traditional Necklace" class="card-image">
                    <div class="card-content">
                        <h3 class="card-title">Royal Necklace Set</h3>
                        <p class="card-description">Exquisite traditional necklace with matching elements, featuring intricate goldwork and precious stone accents for royal occasions.</p>
                    </div>
                </div>

                <div class="jewelry-card">
                    <img src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDAwIiBoZWlnaHQ9IjMwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48ZGVmcz48bGluZWFyR3JhZGllbnQgaWQ9InNpbHZlckdyYWRpZW50IiB4MT0iMCUiIHkxPSIwJSIgeDI9IjEwMCUiIHkyPSIxMDAlIj48c3RvcCBvZmZzZXQ9IjAlIiBzdHlsZT0ic3RvcC1jb2xvcjojZjVmNWY1O3N0b3Atb3BhY2l0eToxIiAvPjxzdG9wIG9mZnNldD0iMTAwJSIgc3R5bGU9InN0b3AtY29sb3I6I2NjY2NjYztzdG9wLW9wYWNpdHk6MSIgLz48L2xpbmVhckdyYWRpZW50PjwvZGVmcz48cmVjdCB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDAlIiBmaWxsPSJ1cmwoI3NpbHZlckdyYWRpZW50KSIvPjxyZWN0IHg9IjEwMCIgeT0iNzAiIHdpZHRoPSIyMDAiIGhlaWdodD0iMTYwIiByeD0iMjAiIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzY2NiIgc3Ryb2tlLXdpZHRoPSIzIi8+PGNpcmNsZSBjeD0iMTUwIiBjeT0iMTMwIiByPSIyNSIgZmlsbD0iI2Y1ZjVmNSIgc3Ryb2tlPSIjNjY2IiBzdHJva2Utd2lkdGg9IjIiLz48Y2lyY2xlIGN4PSIyNTAiIGN5PSIxMzAiIHI9IjI1IiBmaWxsPSIjZjVmNWY1IiBzdHJva2U9IiM2NjYiIHN0cm9rZS13aWR0aD0iMiIvPjx0ZXh0IHg9IjIwMCIgeT0iMjAwIiB0ZXh0LWFuY2hvcj0ibWlkZGxlIiBmaWxsPSIjNjY2IiBmb250LXNpemU9IjE0Ij45OTkgU2lsdmVyPC90ZXh0Pjx0ZXh0IHg9IjIwMCIgeT0iMjIwIiB0ZXh0LWFuY2hvcj0ibWlkZGxlIiBmaWxsPSIjNjY2IiBmb250LXNpemU9IjEyIj4xMDBnbXM8L3RleHQ+PC9zdmc+" alt="Silver Collection" class="card-image">
                    <div class="card-content">
                        <h3 class="card-title">Silver Collectibles</h3>
                        <p class="card-description">Pure 999 silver coins and bars featuring traditional motifs including Lakshmi and Ganesha designs for investment and gifting.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="about" class="section">
        <div class="container">
            <div class="about">
                <h2 class="section-title">About Tirupati Gold</h2>
                <div class="about-content">
                    <div class="about-text">
                        <p>At Tirupati Gold, we have been crafting exquisite jewelry for generations, combining traditional artistry with contemporary designs. Our commitment to quality and craftsmanship has made
