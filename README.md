<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AFRICAN CLAWS - Premium Nail Designs</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #e2cfd5;
            --secondary: #5a575f;
            --accent: #7e796f;
            --light: #fff5f9;
            --dark: #2a2a2a;
            --success: #848f89;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }

        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: grey;
            padding: 1rem 0;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            display: flex;
            align-items: center;
        }

        .logo i {
            margin-right: 10px;
            color: var(--accent);
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 2rem;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            padding: 0.5rem 0;
            border-bottom: 2px solid transparent;
        }

        nav ul li a:hover {
            color: var(--accent);
            border-bottom: 2px solid var(--accent);
        }

        .cart-icon {
            position: relative;
            cursor: pointer;
        }

        .cart-count {
            position: absolute;
            top: -10px;
            right: -10px;
            background: var(--accent);
            color: var(--dark);
            border-radius: 50%;
            width: 20px;
            height: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 0.7rem;
            font-weight: bold;
        }

        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('https://images.unsplash.com/photo-1590845947676-fa2576f401d2?ixlib=rb-4.0.3');
            background-size: cover;
            background-position: center;
            height: 80vh;
            display: flex;
            align-items: center;
            text-align: center;
            color: white;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            background: linear-gradient(to right, var(--primary), var(--accent));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }

        .btn {
            display: inline-block;
            background: linear-gradient(to right, var(--primary), var(--secondary));
            color: white;
            padding: 0.8rem 2rem;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(255, 107, 157, 0.4);
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(255, 107, 157, 0.6);
        }

        .btn-outline {
            background: transparent;
            border: 2px solid white;
            margin-left: 1rem;
        }

        .btn-outline:hover {
            background: white;
            color: var(--primary);
        }

        .section-title {
            text-align: center;
            margin: 4rem 0 2rem;
            font-size: 2.5rem;
            color: var(--dark);
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: linear-gradient(to right, var(--primary), var(--secondary));
            margin: 0.5rem auto;
            border-radius: 2px;
        }

        .categories {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin: 3rem 0;
        }

        .category-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .category-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }

        .category-img {
            height: 200px;
            overflow: hidden;
        }

        .category-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .category-card:hover .category-img img {
            transform: scale(1.1);
        }

        .category-info {
            padding: 1.5rem;
            text-align: center;
        }

        .category-info h3 {
            margin-bottom: 0.5rem;
            color: var(--dark);
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 1.5rem;
            margin: 3rem 0;
        }

        .gallery-item {
            position: relative;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }

        .gallery-item:hover {
            transform: scale(1.03);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
        }

        .gallery-img {
            height: 300px;
            overflow: hidden;
        }

        .gallery-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .gallery-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(to top, rgba(0, 0, 0, 0.8), transparent);
            padding: 1.5rem;
            color: white;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .gallery-item:hover .gallery-overlay {
            opacity: 1;
        }

        .gallery-actions {
            display: flex;
            justify-content: space-between;
            margin-top: 1rem;
        }

        .like-btn, .cart-btn {
            background: rgba(255, 255, 255, 0.2);
            border: none;
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 50px;
            cursor: pointer;
            display: flex;
            align-items: center;
            transition: all 0.3s ease;
        }

        .like-btn:hover, .cart-btn:hover {
            background: var(--primary);
        }

        .like-btn i, .cart-btn i {
            margin-right: 5px;
        }

        .price {
            font-weight: bold;
            font-size: 1.2rem;
            color: var(--accent);
        }

        .testimonials {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            padding: 4rem 0;
            color: white;
            margin: 4rem 0;
        }

        .testimonial-slider {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        .testimonial {
            padding: 2rem;
        }

        .testimonial-text {
            font-size: 1.2rem;
            font-style: italic;
            margin-bottom: 1.5rem;
        }

        .testimonial-author {
            font-weight: bold;
            margin-bottom: 0.5rem;
        }

        .testimonial-rating {
            color: var(--accent);
        }

        .community {
            background: white;
            padding: 4rem 0;
            text-align: center;
        }

        .community p {
            max-width: 700px;
            margin: 0 auto 2rem;
        }

        .upload-btn {
            background: linear-gradient(to right, var(--primary), var(--secondary));
            color: white;
            padding: 1rem 2rem;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(255, 107, 157, 0.4);
            display: inline-flex;
            align-items: center;
        }

        .upload-btn i {
            margin-right: 10px;
        }

        .upload-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(255, 107, 157, 0.6);
        }

        footer {
            background: var(--dark);
            color: white;
            padding: 4rem 0 2rem;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .footer-column h3 {
            margin-bottom: 1.5rem;
            font-size: 1.2rem;
            position: relative;
            padding-bottom: 10px;
        }

        .footer-column h3::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 40px;
            height: 2px;
            background: var(--primary);
        }

        .footer-column ul {
            list-style: none;
        }

        .footer-column ul li {
            margin-bottom: 0.8rem;
        }

        .footer-column ul li a {
            color: #ccc;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-column ul li a:hover {
            color: var(--primary);
        }

        .social-links {
            display: flex;
            gap: 1rem;
            margin-top: 1rem;
        }

        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            transition: all 0.3s ease;
        }

        .social-links a:hover {
            background: var(--primary);
            transform: translateY(-3px);
        }

        .copyright {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #aaa;
            font-size: 0.9rem;
        }

        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            z-index: 1000;
            overflow-y: auto;
        }

        .modal-content {
            background: white;
            width: 90%;
            max-width: 800px;
            margin: 2rem auto;
            border-radius: 10px;
            overflow: hidden;
            animation: modalFadeIn 0.3s ease;
        }

        @keyframes modalFadeIn {
            from {
                opacity: 0;
                transform: translateY(-50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 1.5rem;
            background: linear-gradient(to right, var(--primary), var(--secondary));
            color: white;
        }

        .modal-header h2 {
            font-size: 1.5rem;
        }

        .close-btn {
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }

        .modal-body {
            padding: 1.5rem;
        }

        /* Upload Form */
        .upload-form {
            display: grid;
            gap: 1.5rem;
        }

        .form-group {
            margin-bottom: 1rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
        }

        .form-control {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
            transition: border 0.3s ease;
        }

        .form-control:focus {
            outline: none;
            border-color: var(--primary);
        }

        textarea.form-control {
            min-height: 120px;
            resize: vertical;
        }

        .file-upload {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 2rem;
            border: 2px dashed #ddd;
            border-radius: 5px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .file-upload:hover {
            border-color: var(--primary);
            background: rgba(255, 107, 157, 0.05);
        }

        .file-upload i {
            font-size: 2rem;
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .file-upload p {
            margin-bottom: 0.5rem;
        }

        .file-upload small {
            color: #777;
        }

        /* Responsive Styles */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }

            nav ul {
                margin-top: 1rem;
                justify-content: center;
            }

            nav ul li {
                margin: 0 0.5rem;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .hero-btns {
                display: flex;
                flex-direction: column;
                gap: 1rem;
            }

            .btn-outline {
                margin-left: 0;
            }
        }

        /* Cart Modal */
        .cart-items {
            max-height: 400px;
            overflow-y: auto;
        }

        .cart-item {
            display: flex;
            align-items: center;
            padding: 1rem;
            border-bottom: 1px solid #eee;
        }

        .cart-item-img {
            width: 80px;
            height: 80px;
            border-radius: 5px;
            overflow: hidden;
            margin-right: 1rem;
        }

        .cart-item-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .cart-item-details {
            flex: 1;
        }

        .cart-item-title {
            font-weight: 600;
            margin-bottom: 0.3rem;
        }

        .cart-item-price {
            color: var(--primary);
            font-weight: 600;
        }

        .cart-item-remove {
            background: none;
            border: none;
            color: #ff6b6b;
            cursor: pointer;
            font-size: 1.2rem;
        }

        .cart-total {
            display: flex;
            justify-content: space-between;
            padding: 1.5rem;
            font-size: 1.2rem;
            font-weight: 600;
            border-top: 1px solid #eee;
        }

        .cart-actions {
            display: flex;
            justify-content: flex-end;
            gap: 1rem;
            padding: 0 1.5rem 1.5rem;
        }

        /* Community Gallery */
        .community-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 1.5rem;
            margin: 3rem 0;
        }

        .community-item {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .community-item-img {
            height: 200px;
            overflow: hidden;
        }

        .community-item-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .community-item:hover .community-item-img img {
            transform: scale(1.1);
        }

        .community-item-info {
            padding: 1rem;
        }

        .community-item-user {
            display: flex;
            align-items: center;
            margin-bottom: 0.5rem;
        }

        .user-avatar {
            width: 30px;
            height: 30px;
            border-radius: 50%;
            overflow: hidden;
            margin-right: 10px;
        }

        .user-avatar img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .user-name {
            font-weight: 500;
            font-size: 0.9rem;
        }

        .community-item-actions {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 1rem;
        }

        .like-count {
            display: flex;
            align-items: center;
            color: #777;
            font-size: 0.9rem;
        }

        .like-count i {
            margin-right: 5px;
            color: var(--primary);
        }

        .order-btn {
            background: var(--primary);
            color: white;
            border: none;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            font-size: 0.8rem;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .order-btn:hover {
            background: var(--secondary);
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <i class="fas fa-spa"></i>
                    AFRICAN CLAWS
                </div>
                <nav>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#gallery">Gallery</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#community">Community</a></li>
                        <li><a href="#about">About</a></li>
                        <li><a href="#contact">Contact</a></li>
                        <li>
                            <div class="cart-icon" id="cartIcon">
                                <i class="fas fa-shopping-cart"></i>
                                <span class="cart-count" id="cartCount">0</span>
                            </div>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <section class="hero" id="home">
        <div class="hero-content">
            <h1>Express Your Style</h1>
            <p>Discover our premium nail designs and create your unique look with our custom nail art services.</p>
            <div class="hero-btns">
                <a href="#gallery" class="btn">Explore Designs</a>
                <a href="#community" class="btn btn-outline">Upload Your Design</a>
            </div>
        </div>
    </section>

    <section class="container">
        <h2 class="section-title">Our Services</h2>
        <div class="categories">
            <div class="category-card">
                <div class="category-img">
                    <img src="https://images.unsplash.com/photo-1596704017256-17961a3685a0?ixlib=rb-4.0.3" alt="Acrylic Nails">
                </div>
                <div class="category-info">
                    <h3>Acrylic Nails</h3>
                    <p>Durable and long-lasting nail extensions</p>
                </div>
            </div>
            <div class="category-card">
                <div class="category-img">
                    <img src="https://images.unsplash.com/photo-1604658243844-5e0c1e1a2f1b?ixlib=rb-4.0.3" alt="Gel Nails">
                </div>
                <div class="category-info">
                    <h3>Gel Nails</h3>
                    <p>Natural-looking with a glossy finish</p>
                </div>
            </div>
            <div class="category-card">
                <div class="category-img">
                    <img src="https://images.unsplash.com/photo-1600334129128-685c5582fd35?ixlib=rb-4.0.3" alt="Nail Art">
                </div>
                <div class="category-info">
                    <h3>Nail Art</h3>
                    <p>Custom designs to match your style</p>
                </div>
            </div>
            <div class="category-card">
                <div class="category-img">
                    <img src="https://images.unsplash.com/photo-1518640467707-6811f4a6ab73?ixlib=rb-4.0.3" alt="Nail Care">
                </div>
                <div class="category-info">
                    <h3>Nail Care</h3>
                    <p>Keep your nails healthy and beautiful</p>
                </div>
            </div>
        </div>
    </section>

    <section class="container" id="gallery">
        <h2 class="section-title">Popular Designs</h2>
        <div class="gallery">
            <div class="gallery-item">
                <div class="gallery-img">
                    <img src="https://images.unsplash.com/photo-1596703264021-0d9675d1e4a0?ixlib=rb-4.0.3" alt="Floral Nail Design">
                </div>
                <div class="gallery-overlay">
                    <h3>Floral Elegance</h3>
                    <p>Delicate flower patterns for a feminine touch</p>
                    <div class="gallery-actions">
                        <button class="like-btn"><i class="far fa-heart"></i> Like</button>
                        <span class="price">KES 650</span>
                        <button class="cart-btn" data-id="1" data-title="Floral Elegance" data-price="650"><i class="fas fa-shopping-cart"></i> Add</button>
                    </div>
                </div>
            </div>
            <div class="gallery-item">
                <div class="gallery-img">
                    <img src="https://images.unsplash.com/photo-1604658243844-5e0c1e1a2f1b?ixlib=rb-4.0.3" alt="French Tips">
                </div>
                <div class="gallery-overlay">
                    <h3>Classic French</h3>
                    <p>Timeless white tips for a clean look</p>
                    <div class="gallery-actions">
                        <button class="like-btn"><i class="far fa-heart"></i> Like</button>
                        <span class="price">KES700</span>
                        <button class="cart-btn" data-id="2" data-title="Classic French" data-price="700"><i class="fas fa-shopping-cart"></i> Add</button>
                    </div>
                </div>
            </div>
            <div class="gallery-item">
                <div class="gallery-img">
                    <img src="https://images.unsplash.com/photo-1600334129128-685c5582fd35?ixlib=rb-4.0.3" alt="Geometric Design">
                </div>
                <div class="gallery-overlay">
                    <h3>Geometric Art</h3>
                    <p>Modern patterns for a bold statement</p>
                    <div class="gallery-actions">
                        <button class="like-btn"><i class="far fa-heart"></i> Like</button>
                        <span class="price">KES 650</span>
                        <button class="cart-btn" data-id="3" data-title="Geometric Art" data-price="650"><i class="fas fa-shopping-cart"></i> Add</button>
                    </div>
                </div>
            </div>
            <div class="gallery-item">
                <div class="gallery-img">
                    <img src="https://images.unsplash.com/photo-1596704017256-17961a3685a0?ixlib=rb-4.0.3" alt="Glitter Nails">
                </div>
                <div class="gallery-overlay">
                    <h3>Glitter Glam</h3>
                    <p>Sparkle and shine for special occasions</p>
                    <div class="gallery-actions">
                        <button class="like-btn"><i class="far fa-heart"></i> Like</button>
                        <span class="price">$45</span>
                        <button class="cart-btn" data-id="4" data-title="Glitter Glam" data-price="45"><i class="fas fa-shopping-cart"></i> Add</button>
                    </div>
                </div>
            </div>
            <div class="gallery-item">
                <div class="gallery-img">
                    <img src="https://images.unsplash.com/photo-1598558545395-6f731a0e9a44?ixlib=rb-4.0.3" alt="Marble Nails">
                </div>
                <div class="gallery-overlay">
                    <h3>Marble Effect</h3>
                    <p>Elegant swirls inspired by natural stone</p>
                    <div class="gallery-actions">
                        <button class="like-btn"><i class="far fa-heart"></i> Like</button>
                        <span class="price">$38</span>
                        <button class="cart-btn" data-id="5" data-title="Marble Effect" data-price="38"><i class="fas fa-shopping-cart"></i> Add</button>
                    </div>
                </div>
            </div>
            <div class="gallery-item">
                <div class="gallery-img">
                    <img src="https://images.unsplash.com/photo-1596703264021-0d9675d1e4a0?ixlib=rb-4.0.3" alt="Ombre Nails">
                </div>
                <div class="gallery-overlay">
                    <h3>Ombre Blend</h3>
                    <p>Seamless color transitions for a gradient effect</p>
                    <div class="gallery-actions">
                        <button class="like-btn"><i class="far fa-heart"></i> Like</button>
                        <span class="price">$42</span>
                        <button class="cart-btn" data-id="6" data-title="Ombre Blend" data-price="42"><i class="fas fa-shopping-cart"></i> Add</button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="testimonials">
        <div class="container">
            <h2 class="section-title" style="color: white;">What Our Clients Say</h2>
            <div class="testimonial-slider">
                <div class="testimonial">
                    <p class="testimonial-text">"I'm obsessed with my new nails! The quality is amazing and they lasted over 3 weeks without chipping. Will definitely be ordering again!"</p>
                    <p class="testimonial-author">- CATHERINE KARANJA</p>
                    <div class="testimonial-rating">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="community" id="community">
        <div class="container">
            <h2 class="section-title">Community Designs</h2>
            <p>Our community of nail art enthusiasts shares their creations. Get inspired or upload your own design for others to order!</p>
            <button class="upload-btn" id="uploadBtn"><i class="fas fa-upload"></i> Upload Your Design</button>
            
            <div class="community-gallery" id="communityGallery">
                <!-- Community designs will be loaded here -->
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>GlamNails</h3>
                    <p>Premium nail designs and custom nail art services to express your unique style.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-pinterest-p"></i></a>
                        <a href="#"><i class="fab fa-tiktok"></i></a>
                    </div>
                </div>
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#gallery">Gallery</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#community">Community</a></li>
                        <li><a href="#about">About Us</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Services</h3>
                    <ul>
                        <li><a href="#">Acrylic Nails</a></li>
                        <li><a href="#">Gel Nails</a></li>
                        <li><a href="#">Nail Art</a></li>
                        <li><a href="#">Nail Care</a></li>
                        <li><a href="#">Custom Designs</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Contact</h3>
                    <ul>
                        <li><i class="fas fa-map-marker-alt"></i>NAIROBI,KENYA</li>
                        <li><i class="fas fa-phone"></i> (+254) 762-322483</li>
                        <li><i class="fas fa-envelope"></i> info@africanclaws.com</li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2025 AFRICAN CLAWS. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Upload Modal -->
    <div class="modal" id="uploadModal">
        <div class="modal-content">
            <div class="modal-header">
                <h2>Upload Your Design</h2>
                <button class="close-btn" id="closeUploadModal">&times;</button>
            </div>
            <div class="modal-body">
                <form class="upload-form" id="designForm">
                    <div class="form-group">
                        <label for="designTitle">Design Title</label>
                        <input type="text" id="designTitle" class="form-control" required>
                    </div>
                    <div class="form-group">
                        <label for="designDescription">Description</label>
                        <textarea id="designDescription" class="form-control" required></textarea>
                    </div>
                    <div class="form-group">
                        <label for="designPrice">Price (KES)</label>
                        <input type="number" id="designPrice" class="form-control" min="10" step="5" value="30" required>
                    </div>
                    <div class="form-group">
                        <label>Upload Images</label>
                        <div class="file-upload" id="fileUpload">
                            <i class="fas fa-cloud-upload-alt"></i>
                            <p>Drag & drop your images here</p>
                            <p>or</p>
                            <small>Click to browse files (Max 5MB each)</small>
                            <input type="file" id="designImages" accept="image/*" multiple style="display: none;">
                        </div>
                        <div id="previewContainer" style="display: none; margin-top: 1rem;">
                            <p>Selected images:</p>
                            <div id="imagePreviews" style="display: flex; gap: 10px; margin-top: 10px; flex-wrap: wrap;"></div>
                        </div>
                    </div>
                    <button type="submit" class="btn">Submit Design</button>
                </form>
            </div>
        </div>
    </div>

    <!-- Cart Modal -->
    <div class="modal" id="cartModal">
        <div class="modal-content">
            <div class="modal-header">
                <h2>Your Cart</h2>
                <button class="close-btn" id="closeCartModal">&times;</button>
            </div>
            <div class="modal-body">
                <div class="cart-items" id="cartItems">
                    <!-- Cart items will be loaded here -->
                    <p style="text-align: center; padding: 2rem;">Your cart is empty</p>
                </div>
                <div class="cart-total">
                    <span>Total:</span>
                    <span id="cartTotal">$0</span>
                </div>
                <div class="cart-actions">
                    <button class="btn btn-outline" id="continueShopping">Continue Shopping</button>
                    <button class="btn" id="checkoutBtn">Checkout</button>
                </div>
            </div>
        </div>
    </div>

    <script>
        // DOM Elements
        const uploadBtn = document.getElementById('uploadBtn');
        const uploadModal = document.getElementById('uploadModal');
        const closeUploadModal = document.getElementById('closeUpload
