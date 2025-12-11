[Recreate Exp.html](https://github.com/user-attachments/files/24100977/Recreate.Exp.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Community Center - A Leading Nonprofit Organization</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            background: #fff;
        }

        /* Skip to main content */
        .skip-link {
            position: absolute;
            top: -40px;
            left: 0;
            background: #000;
            color: white;
            padding: 8px;
            text-decoration: none;
            z-index: 100;
        }

        .skip-link:focus {
            top: 0;
        }

        /* Header */
        header {
            background: #fff;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav {
            max-width: 1400px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #e31e24;
            text-decoration: none;
        }

        .main-nav {
            display: flex;
            gap: 0;
            list-style: none;
            align-items: center;
        }

        .main-nav > li {
            position: relative;
        }

        .main-nav > li > a {
            display: block;
            padding: 1rem 1.2rem;
            text-decoration: none;
            color: #333;
            font-weight: 500;
            font-size: 0.95rem;
            transition: color 0.2s;
        }

        .main-nav > li > a:hover {
            color: #e31e24;
        }

        .nav-donate {
            background: #e31e24;
            color: #fff !important;
            border-radius: 4px;
            margin-left: 1rem;
        }

        .nav-donate:hover {
            background: #c41a1f;
        }

        .utility-nav {
            display: flex;
            gap: 1.5rem;
            list-style: none;
            font-size: 0.85rem;
            padding: 0.5rem 2rem;
            background: #f8f9fa;
            max-width: 1400px;
            margin: 0 auto;
        }

        .utility-nav a {
            text-decoration: none;
            color: #666;
        }

        .utility-nav a:hover {
            color: #e31e24;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.3)), url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%23005eb8" width="1200" height="600"/></svg>');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 5rem 2rem;
            text-align: center;
        }

        .hero-badge {
            display: inline-block;
            background: rgba(227, 30, 36, 0.9);
            padding: 0.5rem 1rem;
            border-radius: 4px;
            font-size: 0.9rem;
            font-weight: 600;
            margin-bottom: 1rem;
        }

        .hero h1 {
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 1.5rem;
            max-width: 900px;
            margin-left: auto;
            margin-right: auto;
        }

        .hero-text {
            font-size: 1.1rem;
            line-height: 1.8;
            max-width: 850px;
            margin: 0 auto 2.5rem;
            font-weight: 400;
        }

        .hero-text strong {
            font-weight: 600;
        }

        .location-finder {
            max-width: 700px;
            margin: 0 auto;
            background: white;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.15);
        }

        .location-finder h3 {
            color: #333;
            margin-bottom: 1rem;
            font-size: 1.2rem;
        }

        .search-input-group {
            display: flex;
            gap: 0.5rem;
        }

        .search-input-group input {
            flex: 1;
            padding: 0.9rem;
            border: 2px solid #ddd;
            border-radius: 4px;
            font-size: 1rem;
        }

        .search-input-group button {
            background: #005eb8;
            color: white;
            border: none;
            padding: 0.9rem 2rem;
            border-radius: 4px;
            cursor: pointer;
            font-weight: 600;
            font-size: 1rem;
            white-space: nowrap;
        }

        .search-input-group button:hover {
            background: #004c99;
        }

        /* Anniversary Section */
        .anniversary {
            background: #f8f9fa;
            padding: 4rem 2rem;
        }

        .anniversary-content {
            max-width: 1000px;
            margin: 0 auto;
            text-align: center;
        }

        .anniversary h2 {
            font-size: 2.5rem;
            color: #333;
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .anniversary p {
            font-size: 1.1rem;
            color: #555;
            line-height: 1.8;
            margin-bottom: 2rem;
        }

        .btn-primary {
            display: inline-block;
            background: #005eb8;
            color: white;
            padding: 1rem 2.5rem;
            text-decoration: none;
            border-radius: 4px;
            font-weight: 600;
            font-size: 1rem;
            transition: background 0.3s;
        }

        .btn-primary:hover {
            background: #004c99;
        }

        /* Video Story Section */
        .video-story {
            padding: 4rem 2rem;
            background: #fff;
        }

        .video-story-content {
            max-width: 1000px;
            margin: 0 auto;
            text-align: center;
        }

        .video-story h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: #333;
            font-weight: 700;
        }

        .video-story h3 {
            font-size: 1.1rem;
            color: #666;
            margin-bottom: 2rem;
            font-weight: 500;
        }

        .video-placeholder {
            width: 100%;
            height: 500px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 2rem;
            position: relative;
            overflow: hidden;
        }

        .play-button {
            width: 80px;
            height: 80px;
            background: rgba(255,255,255,0.9);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            color: #005eb8;
            cursor: pointer;
            transition: transform 0.3s;
        }

        .play-button:hover {
            transform: scale(1.1);
        }

        /* Programs Section */
        .programs-section {
            padding: 5rem 2rem;
            background: #fff;
        }

        .programs-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-header {
            text-align: center;
            margin-bottom: 3rem;
        }

        .section-header h4 {
            color: #e31e24;
            font-size: 0.9rem;
            font-weight: 600;
            letter-spacing: 1px;
            text-transform: uppercase;
            margin-bottom: 0.5rem;
        }

        .section-header h2 {
            font-size: 2.5rem;
            color: #333;
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .section-header p {
            font-size: 1.1rem;
            color: #555;
            max-width: 800px;
            margin: 0 auto;
            line-height: 1.8;
        }

        .programs-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
        }

        .program-card {
            background: #fff;
            border-radius: 0;
            overflow: hidden;
            text-decoration: none;
            color: inherit;
            display: block;
            transition: transform 0.3s;
        }

        .program-card:hover {
            transform: translateY(-5px);
        }

        .program-card-image {
            width: 100%;
            height: 280px;
            background: #ddd;
            position: relative;
            overflow: hidden;
        }

        .program-card-image::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 100%;
            background: linear-gradient(to bottom, transparent 50%, rgba(0,0,0,0.3) 100%);
        }

        .program-card-content {
            padding: 1.5rem;
        }

        .program-card h3 {
            font-size: 1.5rem;
            color: #333;
            margin-bottom: 1rem;
            font-weight: 600;
        }

        .program-card h3 a {
            color: #005eb8;
            text-decoration: none;
        }

        .program-card h3 a:hover {
            text-decoration: underline;
        }

        .program-card p {
            color: #555;
            line-height: 1.7;
            font-size: 1rem;
        }

        /* Quote Section */
        .quote-section {
            padding: 5rem 2rem;
            background: linear-gradient(135deg, #005eb8 0%, #003d7a 100%);
            color: white;
            text-align: center;
        }

        .quote-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .quote-section h2 {
            font-size: 2.2rem;
            font-style: italic;
            font-weight: 400;
            margin-bottom: 2rem;
            line-height: 1.5;
        }

        .quote-section p {
            font-size: 1.1rem;
            margin-bottom: 2rem;
        }

        /* News & Stories */
        .news-section {
            padding: 5rem 2rem;
            background: #f8f9fa;
        }

        .news-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .news-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 2rem;
        }

        .news-card {
            background: white;
            border-radius: 0;
            overflow: hidden;
            text-decoration: none;
            color: inherit;
            display: block;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
            transition: box-shadow 0.3s;
        }

        .news-card:hover {
            box-shadow: 0 4px 16px rgba(0,0,0,0.15);
        }

        .news-card-image {
            width: 100%;
            height: 180px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }

        .news-card-content {
            padding: 1.5rem;
        }

        .news-card-type {
            font-size: 0.85rem;
            color: #999;
            margin-bottom: 0.5rem;
        }

        .news-card h3 {
            font-size: 1.1rem;
            color: #333;
            margin-bottom: 0.8rem;
            line-height: 1.4;
            font-weight: 600;
        }

        .news-card-meta {
            font-size: 0.85rem;
            color: #999;
        }

        /* Impact Stats */
        .impact-section {
            padding: 5rem 2rem;
            background: #fff;
        }

        .impact-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .impact-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 3rem;
        }

        .impact-stat {
            text-align: left;
        }

        .impact-stat h3 {
            font-size: 1.4rem;
            color: #333;
            margin-bottom: 1rem;
            font-weight: 600;
            line-height: 1.4;
        }

        .impact-stat p {
            color: #555;
            line-height: 1.7;
            font-size: 1rem;
        }

        .impact-link {
            text-align: center;
            margin-top: 3rem;
        }

        /* Career Section */
        .career-section {
            padding: 5rem 2rem;
            background: linear-gradient(135deg, #e31e24 0%, #b01419 100%);
            color: white;
        }

        .career-content {
            max-width: 1000px;
            margin: 0 auto;
            text-align: center;
        }

        .career-section h2 {
            font-size: 2.5rem;
            margin-bottom: 2rem;
        }

        .btn-white {
            display: inline-block;
            background: white;
            color: #e31e24;
            padding: 1rem 2.5rem;
            text-decoration: none;
            border-radius: 4px;
            font-weight: 600;
            font-size: 1rem;
        }

        .btn-white:hover {
            background: #f0f0f0;
        }

        /* Donate Section */
        .donate-section {
            padding: 5rem 2rem;
            background: #f8f9fa;
        }

        .donate-content {
            max-width: 1000px;
            margin: 0 auto;
            text-align: center;
        }

        .donate-section h2 {
            font-size: 2.5rem;
            color: #333;
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .donate-section p {
            font-size: 1.1rem;
            color: #555;
            margin-bottom: 2rem;
            line-height: 1.8;
        }

        .donate-subtitle {
            font-size: 0.95rem;
            color: #666;
            margin-bottom: 2rem;
        }

        .amount-grid {
            display: grid;
            grid-template-columns: repeat(6, 1fr);
            gap: 1rem;
            margin-bottom: 2rem;
        }

        .amount-btn {
            background: white;
            border: 2px solid #005eb8;
            color: #005eb8;
            padding: 1rem;
            border-radius: 4px;
            font-size: 1.2rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
        }

        .amount-btn:hover {
            background: #005eb8;
            color: white;
        }

        /* Footer */
        footer {
            background: #212529;
            color: #adb5bd;
            padding: 4rem 2rem 2rem;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .footer-top {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 4rem;
            margin-bottom: 3rem;
        }

        .footer-mission {
            font-size: 1rem;
            line-height: 1.8;
        }

        .footer-links {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 2rem;
        }

        .footer-section h3 {
            color: #fff;
            font-size: 1.1rem;
            margin-bottom: 1rem;
            font-weight: 600;
        }

        .footer-section ul {
            list-style: none;
        }

        .footer-section li {
            margin-bottom: 0.7rem;
        }

        .footer-section a {
            color: #adb5bd;
            text-decoration: none;
            font-size: 0.95rem;
        }

        .footer-section a:hover {
            color: #fff;
        }

        .footer-bottom {
            border-top: 1px solid #495057;
            padding-top: 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .footer-legal {
            display: flex;
            gap: 2rem;
            font-size: 0.9rem;
        }

        .social-links {
            display: flex;
            gap: 1rem;
        }

        .social-links a {
            width: 36px;
            height: 36px;
            background: #495057;
            border-radius: 4px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #adb5bd;
            text-decoration: none;
            font-size: 1.2rem;
        }

        .social-links a:hover {
            background: #6c757d;
            color: #fff;
        }

        @media (max-width: 1024px) {
            .programs-grid {
                grid-template-columns: 1fr;
            }

            .news-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .impact-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .amount-grid {
                grid-template-columns: repeat(3, 1fr);
            }
        }

        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2rem;
            }

            .main-nav {
                display: none;
            }

            .news-grid {
                grid-template-columns: 1fr;
            }

            .impact-grid {
                grid-template-columns: 1fr;
            }

            .footer-top {
                grid-template-columns: 1fr;
            }

            .footer-bottom {
                flex-direction: column;
                gap: 1rem;
            }
        }
    </style>
</head>
<body>
    <a href="#main-content" class="skip-link">Skip to main content</a>

    <!-- Utility Navigation -->
    <ul class="utility-nav">
        <li><a href="#contact">Contact</a></li>
        <li><a href="#news">News</a></li>
        <li><a href="#stories">Stories</a></li>
        <li><a href="#search">Search</a></li>
        <li><a href="#terms">Terms of Service</a></li>
        <li><a href="#privacy">Privacy Policy</a></li>
    </ul>

    <!-- Main Header -->
    <header>
        <nav>
            <a href="#" class="logo">Community Center</a>
            <ul class="main-nav">
                <li><a href="#who">Who We Are</a></li>
                <li><a href="#what">What We Do</a></li>
                <li><a href="#involved">Get Involved</a></li>
                <li><a href="#donate" class="nav-donate">Donate</a></li>
                <li><a href="#careers">Careers</a></li>
            </ul>
        </nav>
    </header>

    <!-- Main Content -->
    <main id="main-content">
        <!-- Hero Section -->
        <section class="hero">
            <div class="hero-badge">25th Anniversary: No Place Like This Place</div>
            <h1>No Place Like This Place</h1>
            <div class="hero-text">
                <p><strong>For 25 years, the Community Center has been a place where meaningful connections help build stronger communities. With locations in more than 500 neighborhoods across the country, we're part of everyday life, helping people work toward their goals, build relationships, and discover a true sense of belonging. No matter where you are, there's a place for you here.</strong></p>
                <p><strong>Ready to find your Center? Enter your zip code to explore programs, events, and resources in your community.</strong></p>
            </div>
            <div class="location-finder">
                <h3>No Place Like This Place</h3>
                <div class="search-input-group">
                    <input type="text" placeholder="Search ZIP, City or State">
                    <button onclick="alert('Location finder activated')">Search</button>
                </div>
            </div>
        </section>

        <!-- Anniversary Section -->
        <section class="anniversary">
            <div class="anniversary-content">
                <h2>Celebrating 25 Years of the Community Center</h2>
                <p>This December, the Community Center begins a year-long celebration of 25 years of strengthening communities across the United States. From our earliest days to today, the Center has been where strangers become friends, families find support, and every generation belongs. Explore the milestones that have shaped our story for nearly two decades.</p>
                <a href="#celebrate" class="btn-primary">Join the Celebration</a>
            </div>
        </section>

        <!-- Video Story Section -->
        <section class="video-story">
            <div class="video-story-content">
                <h2>The Something for Everyone Place</h2>
                <h3>Watch more Community Center stories</h3>
                <div class="video-placeholder">
                    <div class="play-button">▶</div>
                </div>
                <p style="max-width: 800px; margin: 0 auto; color: #555; line-height: 1.8;">From classes and programs to personal training and summer activities, the Center is more than programs—it's connection. It's where unlikely friendships form and unexpected support shows up. Whoever you are and whatever your goals, you'll find your place and your people here.</p>
                <a href="#find" class="btn-primary" style="margin-top: 2rem;">Find Your Local Center</a>
            </div>
        </section>

        <!-- Programs Section -->
        <section class="programs-section">
            <div class="programs-content">
                <div class="section-header">
                    <h4>WHAT WE DO</h4>
                    <h2>Our Programs</h2>
                    <p>Our programs and services are focused on our primary areas of impact that help people achieve their goals and strengthen communities. With our breadth of offerings, you can find the support you need and help your neighborhood thrive.</p>
                </div>
                <div class="programs-grid">
                    <div class="program-card">
                        <div class="program-card-image" style="background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);"></div>
                        <div class="program-card-content">
                            <h3><a href="#youth">Youth Development</a></h3>
                            <p>We help young people to grow into healthy, thriving adults by offering supportive education and leadership programs, team sports and camps.</p>
                        </div>
                    </div>
                    <div class="program-card">
                        <div class="program-card-image" style="background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);"></div>
                        <div class="program-card-content">
                            <h3><a href="#healthy">Healthy Living</a></h3>
                            <p>We support individual and community well-being. People of all ages, interests and skill levels can find the fitness classes, family activities and group interests they need to lead active, vibrant lives. The Center also collaborates with community leaders to bring healthy living within reach of all people.</p>
                        </div>
                    </div>
                    <div class="program-card">
                        <div class="program-card-image" style="background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%);"></div>
                        <div class="program-card-content">
                            <h3><a href="#social">Social Responsibility</a></h3>
                            <p>Through community programs, local outreach and global engagement, we provide support and inspire action in our communities.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Quote Section -->
        <section class="quote-section">
            <div class="quote-content">
                <h2>"The true self blooms only when we find our purpose."</h2>
                <p>At the Community Center, we strengthen communities by connecting people to their potential, purpose, and each other.</p>
                <a href="#learn" class="btn-white">Learn More and Find Your Center</a>
            </div>
        </section>

        <!-- News & Stories -->
        <section class="news-section">
            <div class="news-content">
                <div class="section-header">
                    <h2>News & Stories</h2>
                </div>
                <div class="news-grid">
                    <a href="#news1" class="news-card">
                        <div class="news-card-image" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);"></div>
                        <div class="news-card-content">
                            <div class="news-card-type">News Release</div>
                            <h3>Community Center Launches "No Place Like…</h3>
                            <div class="news-card-meta">By Staff | 12/8/2025</div>
                        </div>
                    </a>
                    <a href="#news2" class="news-card">
                        <div class="news-card-image" style="background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);"></div>
                        <div class="news-card-content">
                            <div class="news-card-type">Article</div>
                            <h3>Fueling Potential: How We're Fighting…</h3>
                            <div class="news-card-meta">By Team | 11/25/2025</div>
                        </div>
                    </a>
                    <a href="#news3" class="news-card">
                        <div class="news-card-image" style="background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);"></div>
                        <div class="news-card-content">
                            <div class="news-card-type">Article</div>
                            <h3>5 Fun Ways to Make Learning Part of Your…</h3>
                            <div class="news-card-meta">By Staff | 9/10/2025</div>
                        </div>
                    </a>
                    <a href="#news4" class="news-card">
                        <div class="news-card-image" style="background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%);"></div>
                        <div class="news-card-content">
                            <div class="news-card-type">Article</div>
                            <h3>It's That Time of Year: How to Get Kids…</h3>
                            <div class="news-card-meta">By Staff | 6/11/2025</div>
                        </div>
                    </a>
                </div>
            </div>
        </section>

        <!-- Impact Section -->
        <section class="impact-section">
            <div class="impact-content">
                <div class="section-header">
                    <h2>Our Impact</h2>
                    <p>Each year, we strive to transform lives and strengthen communities nationwide.</p>
                </div>
                <div class="impact-grid">
                    <div class="impact-stat">
                        <h3>8 million community members served annually</h3>
                        <p>Across the U.S., our Centers reach millions of people in 500+ communities.</p>
                    </div>
                    <div class="impact-stat">
                        <h3>1.2 million youths served in food programs</h3>
                        <p>We provide millions of pounds of groceries to families each month.</p>
                    </div>
                    <div class="impact-stat">
                        <h3>120,000 overnight program participants</h3>
                        <p>Our day and overnight programs empowered kids by building lifelong skills, confidence and friendships.</p>
                    </div>
                    <div class="impact-stat">
                        <h3>580 Centers across the U.S.</h3>
                        <p>Centers reach millions of people across 50 states, plus the District of Columbia and Puerto Rico.</p>
                    </div>
                </div>
                <div class="impact-link">
                    <a href="#impact" class="btn-primary">Explore Our Impact</a>
                </div>
            </div>
        </section>

        <!-- Career Section -->
        <section class="career-section">
            <div class="career-content">
                <h2>Work at the Community Center</h2>
                <p style="font-size: 1.2rem; margin-bottom: 2rem;">Find your purpose and fuel your passion with a career at the Community Center.</p>
                <a href="#careers" class="btn-white">View Careers</a>
            </div>
        </section>

        <!-- Donate Section -->
        <section class="donate-section" id="donate">
            <div class="donate-content">
                <h2>Support the Community Center</h2>
                <p>When you support the Community Center – the leading nonprofit committed to strengthening communities – you give young people a chance at a better future, foster healthy lifestyles and help build vibrant communities right where you live.</p>
                <p class="donate-subtitle">The Community Center is a nonprofit, 501(c)(3).</p>
                <div class="amount-grid">
                    <button class="amount-btn" onclick="alert('$35 selected')">$35</button>
                    <button class="amount-btn" onclick="alert('$50 selected')">$50</button>
                    <button class="amount-btn" onclick="alert('$100 selected')">$100</button>
                    <button class="amount-btn" onclick="alert('$200 selected')">$200</button>
                    <button class="amount-btn" onclick="alert('$300 selected')">$300</button>
                    <button class="amount-btn" onclick="alert('$500 selected')">$500</button>
                </div>
                <a href="#donate-form" class="btn-primary">Donate Now</a>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-top">
                <div class="footer-mission">
                    <a href="#" class="logo" style="color: #fff; font-size: 1.5rem; display: inline-block; margin-bottom: 1rem;">Community Center</a>
                    <p>The Community Center is a nonprofit organization whose mission is to strengthen communities through programs that build healthy spirit, mind and body for all.</p>
                </div>
                <div class="footer-links">
                    <div class="footer-section">
                        <h3>Helpful Links</h3>
                        <ul>
                            <li><a href="#about">About Us</a></li>
                            <li><a href="#financial">Financial Information</a></li>
                            <li><a href="#contact">Contact us</a></li>
                            <li><a href="#work">Work at the Center</a></li>
                        </ul>
                    </div>
                    <div class="footer-section">
                        <h3>Find Your Center</h3>
                        <input type="text" placeholder="Location" style="width: 100%; padding: 0.5rem; border: 1px solid #495057; background: #343a40; color: #adb5bd; border-radius: 4px; margin-top: 0.5rem;">
                    </div>
                </div>
            </div>
            <div class="footer-bottom">
                <div>
                    <p style="margin-bottom: 0.5rem;">Copyright © 2025 Community Center. All rights reserved.</p>
                    <div class="footer-legal">
                        <a href="#terms">Terms of Use</a>
                        <a href="#privacy">Privacy Notice</a>
                    </div>
                </div>
                <div class="social-links">
                    <a href="#facebook" title="Facebook">f</a>
                    <a href="#instagram" title="Instagram">📷</a>
                    <a href="#tiktok" title="TikTok">🎵</a>
                    <a href="#youtube" title="YouTube">▶</a>
                </div>
            </div>
        </div>
    </footer>
</body>
</html>
