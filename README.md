<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>KAYD Technologies | Technology. Strategy. Solutions.</title>

    <meta name="description"
        content="KAYD Technologies delivers technology consulting, digital transformation, data and analytics, IT infrastructure, cybersecurity and workplace technology solutions.">

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Manrope:wght@600;700;800&display=swap"
        rel="stylesheet">

    <style>

        :root {
            --navy: #061b38;
            --deep-blue: #082d63;
            --blue: #0b5ed7;
            --bright-blue: #1477ff;
            --light-blue: #eaf3ff;
            --pale-blue: #f5f9ff;
            --white: #ffffff;
            --text: #17233c;
            --muted: #667085;
            --border: #e3eaf3;
            --shadow: 0 18px 50px rgba(7, 42, 87, 0.10);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: "Inter", sans-serif;
            color: var(--text);
            background: var(--white);
            line-height: 1.6;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        img {
            max-width: 100%;
            display: block;
        }

        .container {
            width: min(1160px, 90%);
            margin: auto;
        }

        /* ================= NAVBAR ================= */

        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            background: rgba(255,255,255,0.90);
            backdrop-filter: blur(18px);
            border-bottom: 1px solid rgba(225,232,241,0.7);
        }

        .navbar {
            height: 76px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 11px;
            font-weight: 800;
            letter-spacing: -0.4px;
            color: var(--navy);
        }

        .logo-mark {
            width: 38px;
            height: 38px;
            background: linear-gradient(135deg, var(--blue), var(--bright-blue));
            border-radius: 10px;
            position: relative;
            box-shadow: 0 8px 20px rgba(20,119,255,0.25);
        }

        .logo-mark::before,
        .logo-mark::after {
            content: "";
            position: absolute;
            background: white;
            border-radius: 2px;
        }

        .logo-mark::before {
            width: 20px;
            height: 5px;
            left: 9px;
            top: 16px;
        }

        .logo-mark::after {
            width: 5px;
            height: 20px;
            left: 16px;
            top: 9px;
        }

        .nav-links {
            display: flex;
            gap: 30px;
            align-items: center;
            font-size: 14px;
            font-weight: 600;
        }

        .nav-links a {
            color: #475467;
            transition: 0.25s;
        }

        .nav-links a:hover {
            color: var(--blue);
        }

        .nav-contact {
            padding: 11px 18px;
            border-radius: 8px;
            background: var(--navy);
            color: white !important;
        }

        .menu-btn {
            display: none;
            border: none;
            background: transparent;
            font-size: 27px;
            cursor: pointer;
            color: var(--navy);
        }

        /* ================= HERO ================= */

        .hero {
            min-height: 100vh;
            padding-top: 76px;
            background:
                linear-gradient(90deg, rgba(3,20,43,0.90), rgba(3,28,61,0.62)),
                url("https://www.theimpulsedigital.com/why%20chooose%20us%20section%20576%20x%20400%202.jpg")
                center/cover no-repeat;
            display: flex;
            align-items: center;
            color: white;
        }

        .hero-content {
            max-width: 780px;
            padding: 90px 0;
        }

        .eyebrow {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: rgba(255,255,255,0.10);
            border: 1px solid rgba(255,255,255,0.18);
            padding: 8px 14px;
            border-radius: 30px;
            font-size: 13px;
            font-weight: 600;
            margin-bottom: 25px;
        }

        .eyebrow-dot {
            width: 7px;
            height: 7px;
            background: #61a5ff;
            border-radius: 50%;
        }

        .hero h1 {
            font-family: "Manrope", sans-serif;
            font-size: clamp(42px, 6vw, 78px);
            line-height: 1.02;
            letter-spacing: -3px;
            margin-bottom: 24px;
        }

        .hero h1 span {
            color: #67a9ff;
        }

        .hero-brand {
            font-size: 18px;
            font-weight: 800;
            letter-spacing: 4px;
            margin-bottom: 18px;
        }

        .hero p {
            max-width: 650px;
            color: rgba(255,255,255,0.78);
            font-size: 18px;
            margin-bottom: 35px;
        }

        .hero-buttons {
            display: flex;
            gap: 14px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 13px 21px;
            border-radius: 8px;
            font-size: 14px;
            font-weight: 700;
            border: none;
            cursor: pointer;
            transition: 0.25s;
        }

        .btn-primary {
            background: var(--bright-blue);
            color: white;
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 12px 25px rgba(20,119,255,0.25);
        }

        .btn-outline {
            color: white;
            border: 1px solid rgba(255,255,255,0.35);
            background: rgba(255,255,255,0.06);
        }

        .btn-outline:hover {
            background: white;
            color: var(--navy);
        }

        /* ================= GENERAL ================= */

        section {
            padding: 95px 0;
        }

        .section-header {
            max-width: 700px;
            margin-bottom: 50px;
        }

        .section-label {
            color: var(--blue);
            text-transform: uppercase;
            font-size: 12px;
            font-weight: 800;
            letter-spacing: 1.7px;
            margin-bottom: 10px;
        }

        .section-title {
            font-family: "Manrope", sans-serif;
            font-size: clamp(30px, 4vw, 45px);
            line-height: 1.15;
            letter-spacing: -1.5px;
            color: var(--navy);
            margin-bottom: 15px;
        }

        .section-description {
            color: var(--muted);
            font-size: 16px;
        }

        /* ================= ABOUT ================= */

        .about {
            background: white;
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 70px;
            align-items: center;
        }

        .about-image {
            border-radius: 18px;
            overflow: hidden;
            box-shadow: var(--shadow);
        }

        .about-image img {
            width: 100%;
            height: 430px;
            object-fit: cover;
        }

        .about-text p {
            color: var(--muted);
            margin-bottom: 18px;
        }

        .about-points {
            display: grid;
            gap: 15px;
            margin-top: 28px;
        }

        .about-point {
            display: flex;
            gap: 14px;
            align-items: flex-start;
        }

        .check {
            width: 25px;
            height: 25px;
            min-width: 25px;
            border-radius: 50%;
            background: var(--light-blue);
            color: var(--blue);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 13px;
            font-weight: 800;
        }

        .about-point strong {
            display: block;
            color: var(--navy);
            margin-bottom: 2px;
        }

        .about-point span {
            color: var(--muted);
            font-size: 14px;
        }

        /* ================= SOLUTIONS ================= */

        .solutions {
            background: var(--pale-blue);
        }

        .solution-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .solution-card {
            background: white;
            padding: 30px;
            border: 1px solid var(--border);
            border-radius: 15px;
            transition: 0.3s;
        }

        .solution-card:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow);
            border-color: #cbdcf5;
        }

        .solution-icon {
            width: 48px;
            height: 48px;
            border-radius: 11px;
            background: var(--light-blue);
            color: var(--blue);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 21px;
            font-weight: 800;
            margin-bottom: 20px;
        }

        .solution-card h3 {
            font-size: 18px;
            color: var(--navy);
            margin-bottom: 9px;
        }

        .solution-card p {
            font-size: 14px;
            color: var(--muted);
        }

        /* ================= TECHNOLOGY PORTFOLIO ================= */

        .portfolio {
            background: white;
        }

        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .portfolio-card {
            border: 1px solid var(--border);
            border-radius: 14px;
            padding: 28px;
            background: #fff;
        }

        .portfolio-card h3 {
            color: var(--navy);
            font-size: 18px;
            margin-bottom: 12px;
        }

        .portfolio-card p {
            color: var(--muted);
            font-size: 14px;
            margin-bottom: 18px;
        }

        .portfolio-card ul {
            list-style: none;
            display: grid;
            gap: 8px;
        }

        .portfolio-card li {
            font-size: 13px;
            color: #475467;
            padding-left: 17px;
            position: relative;
        }

        .portfolio-card li::before {
            content: "";
            width: 5px;
            height: 5px;
            background: var(--bright-blue);
            border-radius: 50%;
            position: absolute;
            left: 0;
            top: 9px;
        }

        /* ================= INDUSTRIES ================= */

        .industries {
            background: var(--navy);
            color: white;
        }

        .industries .section-title {
            color: white;
        }

        .industries .section-description {
            color: rgba(255,255,255,0.65);
        }

        .industry-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 15px;
        }

        .industry {
            padding: 25px 20px;
            border: 1px solid rgba(255,255,255,0.12);
            border-radius: 12px;
            background: rgba(255,255,255,0.045);
        }

        .industry h3 {
            font-size: 16px;
            margin-bottom: 7px;
        }

        .industry p {
            font-size: 13px;
            color: rgba(255,255,255,0.58);
        }

        /* ================= WHY KAYD ================= */

        .why-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 65px;
            align-items: center;
        }

        .why-image {
            border-radius: 18px;
            overflow: hidden;
            box-shadow: var(--shadow);
        }

        .why-image img {
            width: 100%;
            height: 430px;
            object-fit: cover;
        }

        .why-list {
            display: grid;
            gap: 22px;
        }

        .why-item {
            display: flex;
            gap: 16px;
        }

        .why-number {
            width: 38px;
            height: 38px;
            min-width: 38px;
            border-radius: 9px;
            background: var(--light-blue);
            color: var(--blue);
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 13px;
            font-weight: 800;
        }

        .why-item h3 {
            font-size: 17px;
            color: var(--navy);
            margin-bottom: 4px;
        }

        .why-item p {
            font-size: 14px;
            color: var(--muted);
        }

        /* ================= REVIEWS ================= */

        .reviews {
            background: var(--pale-blue);
        }

        .review-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        .review-card {
            background: white;
            border: 1px solid var(--border);
            padding: 28px;
            border-radius: 15px;
        }

        .stars {
            color: #f59e0b;
            letter-spacing: 2px;
            margin-bottom: 18px;
        }

        .review-card p {
            font-size: 14px;
            color: #475467;
            margin-bottom: 22px;
        }

        .review-author strong {
            display: block;
            font-size: 14px;
            color: var(--navy);
        }

        .review-author span {
            color: var(--muted);
            font-size: 12px;
        }

        .sample-note {
            font-size: 12px;
            color: var(--muted);
            margin-top: 30px;
        }

        /* ================= CTA ================= */

        .cta {
            background: linear-gradient(135deg, var(--deep-blue), var(--blue));
            color: white;
            text-align: center;
        }

        .cta h2 {
            font-family: "Manrope", sans-serif;
            font-size: clamp(30px, 4vw, 45px);
            margin-bottom: 15px;
        }

        .cta p {
            color: rgba(255,255,255,0.75);
            max-width: 650px;
            margin: 0 auto 28px;
        }

        /* ================= CONTACT ================= */

        .contact {
            background: white;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: 0.8fr 1.2fr;
            gap: 70px;
        }

        .contact-info {
            display: grid;
            gap: 22px;
            margin-top: 25px;
        }

        .contact-item {
            display: flex;
            gap: 14px;
        }

        .contact-icon {
            width: 40px;
            height: 40px;
            border-radius: 9px;
            background: var(--light-blue);
            color: var(--blue);
            display: flex;
            justify-content: center;
            align-items: center;
            font-weight: 800;
        }

        .contact-item strong {
            display: block;
            color: var(--navy);
            font-size: 14px;
        }

        .contact-item span,
        .contact-item a {
            font-size: 14px;
            color: var(--muted);
        }

        .contact-form {
            padding: 35px;
            border: 1px solid var(--border);
            border-radius: 16px;
            box-shadow: var(--shadow);
        }

        .form-row {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 16px;
        }

        .form-group {
            margin-bottom: 18px;
        }

        .form-group label {
            display: block;
            font-size: 13px;
            font-weight: 600;
            color: var(--navy);
            margin-bottom: 7px;
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            border: 1px solid var(--border);
            border-radius: 8px;
            padding: 12px 13px;
            font-family: inherit;
            font-size: 13px;
            outline: none;
            transition: 0.2s;
            background: white;
        }

        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            border-color: var(--bright-blue);
            box-shadow: 0 0 0 3px rgba(20,119,255,0.08);
        }

        .form-group textarea {
            height: 120px;
            resize: vertical;
        }

        .form-submit {
            width: 100%;
        }

        .success-message,
        .error-message {
            display: none;
            padding: 12px 14px;
            border-radius: 8px;
            margin-bottom: 18px;
            font-size: 13px;
        }

        .success-message {
            background: #ecfdf3;
            color: #027a48;
        }

        .error-message {
            background: #fef3f2;
            color: #b42318;
        }

        /* ================= FOOTER ================= */

        footer {
            background: #031326;
            color: white;
            padding: 55px 0 25px;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: 1.3fr 1fr 1fr;
            gap: 50px;
            padding-bottom: 40px;
        }

        .footer-logo {
            color: white;
            margin-bottom: 16px;
        }

        .footer-about {
            color: rgba(255,255,255,0.55);
            font-size: 13px;
            max-width: 360px;
        }

        .footer-column h4 {
            font-size: 13px;
            margin-bottom: 17px;
        }

        .footer-column a {
            display: block;
            color: rgba(255,255,255,0.55);
            font-size: 13px;
            margin-bottom: 9px;
        }

        .footer-column a:hover {
            color: white;
        }

        .footer-bottom {
            border-top: 1px solid rgba(255,255,255,0.09);
            padding-top: 22px;
            display: flex;
            justify-content: space-between;
            color: rgba(255,255,255,0.42);
            font-size: 12px;
        }

        /* ================= RESPONSIVE ================= */

        @media (max-width: 900px) {

            .nav-links {
                position: absolute;
                top: 76px;
                left: 0;
                width: 100%;
                background: white;
                flex-direction: column;
                align-items: flex-start;
                padding: 25px 5%;
                gap: 18px;
                display: none;
                box-shadow: 0 15px 25px rgba(0,0,0,0.08);
            }

            .nav-links.active {
                display: flex;
            }

            .menu-btn {
                display: block;
            }

            .about-grid,
            .why-grid,
            .contact-grid {
                grid-template-columns: 1fr;
            }

            .solution-grid,
            .portfolio-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .industry-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .review-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .footer-grid {
                grid-template-columns: 1fr 1fr;
            }
        }

        @media (max-width: 600px) {

            section {
                padding: 70px 0;
            }

            .hero h1 {
                letter-spacing: -2px;
            }

            .solution-grid,
            .portfolio-grid,
            .industry-grid,
            .review-grid,
            .footer-grid {
                grid-template-columns: 1fr;
            }

            .form-row {
                grid-template-columns: 1fr;
            }

            .contact-form {
                padding: 25px;
            }

            .footer-bottom {
                flex-direction: column;
                gap: 8px;
            }

            .about-image img,
            .why-image img {
                height: 300px;
            }
        }

    </style>
</head>

<body>

<!-- ================= NAVBAR ================= -->

<header>
    <div class="container navbar">

        <a href="#home" class="logo">
            <div class="logo-mark"></div>
            <span>KAYD TECHNOLOGIES</span>
        </a>

        <button class="menu-btn" id="menuBtn">☰</button>

        <nav class="nav-links" id="navLinks">
            <a href="#home">Home</a>
            <a href="#about">About Us</a>
            <a href="#solutions">Solutions</a>
            <a href="#portfolio">Expertise</a>
            <a href="#industries">Industries</a>
            <a href="#reviews">Perspectives</a>
            <a href="#contact" class="nav-contact">Contact</a>
        </nav>

    </div>
</header>


<!-- ================= HERO ================= -->

<section class="hero" id="home">

    <div class="container">

        <div class="hero-content">

            <div class="hero-brand">
                KAYD TECHNOLOGIES
            </div>

            <div class="eyebrow">
                <span class="eyebrow-dot"></span>
                Technology • Strategy • Transformation
            </div>

            <h1>
                Technology that<br>
                <span>moves business.</span>
            </h1>

            <p>
                We help organizations turn technology into a practical
                business advantage through thoughtful strategy, digital
                solutions and technology-driven transformation.
            </p>

            <div class="hero-buttons">
                <a href="#solutions" class="btn btn-primary">
                    Explore Solutions
                </a>

                <a href="#contact" class="btn btn-outline">
                    Start a Conversation
                </a>
            </div>

        </div>

    </div>

</section>


<!-- ================= ABOUT ================= -->

<section class="about" id="about">

    <div class="container">

        <div class="about-grid">

            <div class="about-image">
                <img
                    src="https://www.ddfintechsolutions.com/indian-corporate-team-meeting-in-modern-glass-offi.jpg"
                    alt="Business technology team">
            </div>

            <div class="about-text">

                <div class="section-label">About KAYD</div>

                <h2 class="section-title">
                    Bridging business needs with technology.
                </h2>

                <p>
                    KAYD Technologies is a technology solutions company
                    focused on helping businesses understand, adopt and
                    effectively use technology.
                </p>

                <p>
                    Our approach combines business thinking with technology
                    to create solutions that are practical, scalable and
                    aligned with organizational goals.
                </p>

                <div class="about-points">

                    <div class="about-point">
                        <div class="check">✓</div>
                        <div>
                            <strong>Business-first thinking</strong>
                            <span>
                                Technology decisions connected to real business objectives.
                            </span>
                        </div>
                    </div>

                    <div class="about-point">
                        <div class="check">✓</div>
                        <div>
                            <strong>Practical solutions</strong>
                            <span>
                                Simple, relevant and scalable approaches to technology challenges.
                            </span>
                        </div>
                    </div>

                    <div class="about-point">
                        <div class="check">✓</div>
                        <div>
                            <strong>Future-ready approach</strong>
                            <span>
                                Helping organizations prepare for changing technology environments.
                            </span>
                        </div>
                    </div>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- ================= SOLUTIONS ================= -->

<section class="solutions" id="solutions">

    <div class="container">

        <div class="section-header">

            <div class="section-label">Our Solutions</div>

            <h2 class="section-title">
                Technology solutions designed around business challenges.
            </h2>

            <p class="section-description">
                From technology strategy to digital transformation, we focus
                on solving business problems rather than simply implementing technology.
            </p>

        </div>


        <div class="solution-grid">

            <div class="solution-card">
                <div class="solution-icon">01</div>
                <h3>Technology Consulting</h3>
                <p>
                    Helping organizations evaluate technology opportunities,
                    define priorities and make informed technology decisions.
                </p>
            </div>

            <div class="solution-card">
                <div class="solution-icon">02</div>
                <h3>Digital Transformation</h3>
                <p>
                    Supporting organizations as they modernize processes,
                    adopt digital tools and improve operational efficiency.
                </p>
            </div>

            <div class="solution-card">
                <div class="solution-icon">03</div>
                <h3>Data & Analytics</h3>
                <p>
                    Turning business data into useful insights that support
                    better decisions and measurable outcomes.
                </p>
            </div>

            <div class="solution-card">
                <div class="solution-icon">04</div>
                <h3>IT Infrastructure</h3>
                <p>
                    Helping businesses plan reliable computing, networking,
                    cloud and workplace technology environments.
                </p>
            </div>

            <div class="solution-card">
                <div class="solution-icon">05</div>
                <h3>Cybersecurity</h3>
                <p>
                    Supporting organizations in understanding technology
                    risks and strengthening their digital security posture.
                </p>
            </div>

            <div class="solution-card">
                <div class="solution-icon">06</div>
                <h3>Workplace Technology</h3>
                <p>
                    Enabling productive, connected and collaborative
                    workplaces through thoughtful technology solutions.
                </p>
            </div>

        </div>

    </div>

</section>


<!-- ================= TECHNOLOGY PORTFOLIO ================= -->

<section class="portfolio" id="portfolio">

    <div class="container">

        <div class="section-header">

            <div class="section-label">Technology Expertise</div>

            <h2 class="section-title">
                Areas where technology creates business value.
            </h2>

            <p class="section-description">
                Our technology portfolio represents the domains we work
                across to understand business requirements and develop
                suitable technology strategies.
            </p>

        </div>


        <div class="portfolio-grid">

            <div class="portfolio-card">

                <h3>Computing & End-User Technology</h3>

                <p>
                    Technology environments that support employees and
                    everyday business operations.
                </p>

                <ul>
                    <li>End-user computing</li>
                    <li>Workplace devices</li>
                    <li>Device management</li>
                    <li>Digital workplace</li>
                </ul>

            </div>


            <div class="portfolio-card">

                <h3>Networking & Connectivity</h3>

                <p>
                    Connected technology environments designed for
                    reliable communication and collaboration.
                </p>

                <ul>
                    <li>Network infrastructure</li>
                    <li>Connectivity strategy</li>
                    <li>Wireless environments</li>
                    <li>Network planning</li>
                </ul>

            </div>


            <div class="portfolio-card">

                <h3>Cloud & Infrastructure</h3>

                <p>
                    Modern infrastructure approaches that support
                    scalability, availability and business continuity.
                </p>

                <ul>
                    <li>Cloud strategy</li>
                    <li>Infrastructure planning</li>
                    <li>Storage environments</li>
                    <li>Business continuity</li>
                </ul>

            </div>


            <div class="portfolio-card">

                <h3>Data & Analytics</h3>

                <p>
                    Data-driven approaches that help organizations
                    understand performance and make better decisions.
                </p>

                <ul>
                    <li>Business intelligence</li>
                    <li>Data visualization</li>
                    <li>Analytics solutions</li>
                    <li>Decision support</li>
                </ul>

            </div>


            <div class="portfolio-card">

                <h3>Cybersecurity</h3>

                <p>
                    Technology and processes designed to help organizations
                    manage digital risks.
                </p>

                <ul>
                    <li>Security awareness</li>
                    <li>Risk assessment</li>
                    <li>Access management</li>
                    <li>Security planning</li>
                </ul>

            </div>


            <div class="portfolio-card">

                <h3>Collaboration Technology</h3>

                <p>
                    Enabling teams to communicate and collaborate effectively
                    across modern work environments.
                </p>

                <ul>
                    <li>Video collaboration</li>
                    <li>Meeting technology</li>
                    <li>Digital communication</li>
                    <li>Hybrid workplace</li>
                </ul>

            </div>

        </div>

    </div>

</section>


<!-- ================= INDUSTRIES ================= -->

<section class="industries" id="industries">

    <div class="container">

        <div class="section-header">

            <div class="section-label">Industries</div>

            <h2 class="section-title">
                Technology for different business environments.
            </h2>

            <p class="section-description">
                Our approach can be adapted to the technology needs of
                organizations across multiple industries.
            </p>

        </div>


        <div class="industry-grid">

            <div class="industry">
                <h3>Education</h3>
                <p>Digital learning and connected campus environments.</p>
            </div>

            <div class="industry">
                <h3>Healthcare</h3>
                <p>Technology supporting efficient and connected operations.</p>
            </div>

            <div class="industry">
                <h3>Retail</h3>
                <p>Technology supporting customer and operational experiences.</p>
            </div>

            <div class="industry">
                <h3>Manufacturing</h3>
                <p>Digital operations and technology-enabled processes.</p>
            </div>

            <div class="industry">
                <h3>Financial Services</h3>
                <p>Technology, data and digital process environments.</p>
            </div>

            <div class="industry">
                <h3>Professional Services</h3>
                <p>Technology for productive and connected teams.</p>
            </div>

            <div class="industry">
                <h3>Startups</h3>
                <p>Scalable technology foundations for growing businesses.</p>
            </div>

            <div class="industry">
                <h3>Corporate</h3>
                <p>Technology strategy for modern business environments.</p>
            </div>

        </div>

    </div>

</section>


<!-- ================= WHY KAYD ================= -->

<section id="why">

    <div class="container">

        <div class="why-grid">

            <div class="why-image">
                <img
                    src="https://shotroom.in/pages/careers/ai-startup-team-indian-fashion-tech-office.webp"
                    alt="Technology team working together">
            </div>


            <div>

                <div class="section-label">Why KAYD</div>

                <h2 class="section-title">
                    Technology with a clear business purpose.
                </h2>

                <div class="why-list">

                    <div class="why-item">
                        <div class="why-number">01</div>

                        <div>
                            <h3>Business Understanding</h3>
                            <p>
                                We begin by understanding the business
                                challenge before thinking about technology.
                            </p>
                        </div>
                    </div>


                    <div class="why-item">
                        <div class="why-number">02</div>

                        <div>
                            <h3>Practical Thinking</h3>
                            <p>
                                Our solutions focus on what is useful,
                                achievable and relevant to the organization.
                            </p>
                        </div>
                    </div>


                    <div class="why-item">
                        <div class="why-number">03</div>

                        <div>
                            <h3>Technology Agility</h3>
                            <p>
                                We keep the approach flexible as business
                                requirements and technology evolve.
                            </p>
                        </div>
                    </div>


                    <div class="why-item">
                        <div class="why-number">04</div>

                        <div>
                            <h3>Long-Term Perspective</h3>
                            <p>
                                Technology decisions are considered with
                                scalability and future business needs in mind.
                            </p>
                        </div>
                    </div>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- ================= REVIEWS ================= -->

<section class="reviews" id="reviews">

    <div class="container">

        <div class="section-header">

            <div class="section-label">Client Perspectives</div>

            <h2 class="section-title">
                What a technology partnership should feel like.
            </h2>

            <p class="section-description">
                A few sample perspectives representing the kind of
                experience KAYD aims to create.
            </p>

        </div>


        <div class="review-grid">

            <div class="review-card">
                <div class="stars">★★★★★</div>
                <p>
                    “KAYD's approach focuses on understanding the business
                    requirement first, which made the technology discussion
                    much more meaningful.”
                </p>

                <div class="review-author">
                    <strong>Priya Menon</strong>
                    <span>Operations Manager</span>
                </div>
            </div>


            <div class="review-card">
                <div class="stars">★★★★★</div>
                <p>
                    “The team presented technology concepts in a simple and
                    practical way. It made the decision-making process easier.”
                </p>

                <div class="review-author">
                    <strong>Arun Kumar</strong>
                    <span>IT Administrator</span>
                </div>
            </div>


            <div class="review-card">
                <div class="stars">★★★★☆</div>
                <p>
                    “A business-focused approach to technology rather than
                    simply recommending technology for the sake of it.”
                </p>

                <div class="review-author">
                    <strong>Rahul Sharma</strong>
                    <span>Business Operations Lead</span>
                </div>
            </div>


            <div class="review-card">
                <div class="stars">★★★★★</div>
                <p>
                    “KAYD brings together business thinking and technology
                    in a way that feels relevant to modern organizations.”
                </p>

                <div class="review-author">
                    <strong>Sneha Iyer</strong>
                    <span>Project Manager</span>
                </div>
            </div>


            <div class="review-card">
                <div class="stars">★★★★☆</div>
                <p>
                    “Their focus on practical technology solutions makes the
                    conversation much easier for non-technical stakeholders.”
                </p>

                <div class="review-author">
                    <strong>Karthik R</strong>
                    <span>Technology Manager</span>
                </div>
            </div>


            <div class="review-card">
                <div class="stars">★★★★★</div>
                <p>
                    “A modern approach to technology strategy with a clear
                    focus on business outcomes.”
                </p>

                <div class="review-author">
                    <strong>Ananya Krishnan</strong>
                    <span>Administration Head</span>
                </div>
            </div>

        </div>

        <p class="sample-note">
            * Sample testimonials created for academic/mock-company website purposes.
        </p>

    </div>

</section>


<!-- ================= CTA ================= -->

<section class="cta">

    <div class="container">

        <h2>Have a technology challenge?</h2>

        <p>
            Tell us what you are trying to solve. Let's explore how
            technology can support your business objectives.
        </p>

        <a href="#contact" class="btn btn-outline">
            Start a Conversation
        </a>

    </div>

</section>


<!-- ================= CONTACT ================= -->

<section class="contact" id="contact">

    <div class="container">

        <div class="contact-grid">

            <div>

                <div class="section-label">Contact</div>

                <h2 class="section-title">
                    Let's talk about your business challenge.
                </h2>

                <p class="section-description">
                    Whether you are exploring digital transformation,
                    analytics, infrastructure or technology strategy,
                    we'd be happy to understand your requirement.
                </p>


                <div class="contact-info">

                    <div class="contact-item">

                        <div class="contact-icon">E</div>

                        <div>
                            <strong>Email</strong>
                            <a href="mailto:kayd.tech@gmail.com">
                                kayd.tech@gmail.com
                            </a>
                        </div>

                    </div>


                    <div class="contact-item">

                        <div class="contact-icon">L</div>

                        <div>
                            <strong>Location</strong>
                            <span>
                                Chennai, Tamil Nadu, India
                            </span>
                        </div>

                    </div>


                    <div class="contact-item">

                        <div class="contact-icon">A</div>

                        <div>
                            <strong>Address</strong>
                            <span>
                                No. 18, Tech Park Road,<br>
                                Guindy Industrial Estate,<br>
                                Chennai - 600032, India
                            </span>
                        </div>

                    </div>

                </div>

            </div>


            <!-- CONTACT FORM -->

            <form
                class="contact-form"
                id="contactForm"
                action="https://api.web3forms.com/submit"
                method="POST"
            >

                <!-- REPLACE THIS WITH YOUR WEB3FORMS ACCESS KEY -->
                <input
                    type="hidden"
                    name="access_key"
                    value="YOUR_ACCESS_KEY_HERE"
                >

                <input
                    type="hidden"
                    name="subject"
                    value="New Business Enquiry - KAYD Technologies"
                >

                <input
                    type="hidden"
                    name="from_name"
                    value="KAYD Technologies Website"
                >

                <input
                    type="checkbox"
                    name="botcheck"
                    style="display:none;"
                >


                <div
                    class="success-message"
                    id="successMessage"
                >
                    Thank you. Your enquiry has been received.
                </div>

                <div
                    class="error-message"
                    id="errorMessage"
                >
                    Something went wrong. Please try again.
                </div>


                <div class="form-row">

                    <div class="form-group">
                        <label for="name">
                            Full Name
                        </label>

                        <input
                            type="text"
                            id="name"
                            name="name"
                            placeholder="Your name"
                            required
                        >
                    </div>


                    <div class="form-group">
                        <label for="company">
                            Organization
                        </label>

                        <input
                            type="text"
                            id="company"
                            name="company"
                            placeholder="Organization name"
                        >
                    </div>

                </div>


                <div class="form-row">

                    <div class="form-group">
                        <label for="email">
                            Email
                        </label>

                        <input
                            type="email"
                            id="email"
                            name="email"
                            placeholder="you@company.com"
                            required
                        >
                    </div>


                    <div class="form-group">
                        <label for="phone">
                            Phone
                        </label>

                        <input
                            type="tel"
                            id="phone"
                            name="phone"
                            placeholder="+91"
                        >
                    </div>

                </div>


                <div class="form-group">

                    <label for="requirement">
                        Area of Interest
                    </label>

                    <select
                        id="requirement"
                        name="area_of_interest"
                    >

                        <option value="">
                            Select an area
                        </option>

                        <option>
                            Technology Consulting
                        </option>

                        <option>
                            Digital Transformation
                        </option>

                        <option>
                            Data & Analytics
                        </option>

                        <option>
                            IT Infrastructure
                        </option>

                        <option>
                            Cybersecurity
                        </option>

                        <option>
                            Workplace Technology
                        </option>

                        <option>
                            General Enquiry
                        </option>

                    </select>

                </div>


                <div class="form-group">

                    <label for="message">
                        Business Challenge
                    </label>

                    <textarea
                        id="message"
                        name="message"
                        placeholder="Tell us about your business challenge or requirement..."
                        required
                    ></textarea>

                </div>


                <button
                    type="submit"
                    class="btn btn-primary form-submit"
                >
                    Send Enquiry
                </button>

            </form>

        </div>

    </div>

</section>


<!-- ================= FOOTER ================= -->

<footer>

    <div class="container">

        <div class="footer-grid">

            <div>

                <div class="logo footer-logo">
                    <div class="logo-mark"></div>
                    <span>KAYD TECHNOLOGIES</span>
                </div>

                <p class="footer-about">
                    Technology, strategy and digital solutions designed
                    to help organizations navigate a changing business environment.
                </p>

            </div>


            <div class="footer-column">

                <h4>Explore</h4>

                <a href="#about">About Us</a>
                <a href="#solutions">Solutions</a>
                <a href="#portfolio">Technology Expertise</a>
                <a href="#industries">Industries</a>

            </div>


            <div class="footer-column">

                <h4>Connect</h4>

                <a href="#contact">Contact</a>

                <a href="mailto:kayd.tech@gmail.com">
                    kayd.tech@gmail.com
                </a>

                <a href="#home">
                    Chennai, India
                </a>

            </div>

        </div>


        <div class="footer-bottom">

            <span>
                © 2026 KAYD Technologies. All rights reserved.
            </span>

            <span>
                Academic / Mock Company Website
            </span>

        </div>

    </div>

</footer>


<!-- ================= JAVASCRIPT ================= -->

<script>

    /* MOBILE MENU */

    const menuBtn = document.getElementById("menuBtn");
    const navLinks = document.getElementById("navLinks");

    menuBtn.addEventListener("click", function () {

        navLinks.classList.toggle("active");

    });


    /* CLOSE MOBILE MENU AFTER CLICK */

    document.querySelectorAll(".nav-links a").forEach(function(link) {

        link.addEventListener("click", function() {

            navLinks.classList.remove("active");

        });

    });


    /* CONTACT FORM */

    const contactForm =
        document.getElementById("contactForm");

    const successMessage =
        document.getElementById("successMessage");

    const errorMessage =
        document.getElementById("errorMessage");


    contactForm.addEventListener("submit", async function(event) {

        event.preventDefault();

        successMessage.style.display = "none";
        errorMessage.style.display = "none";

        const submitButton =
            contactForm.querySelector("button[type='submit']");

        submitButton.disabled = true;
        submitButton.textContent = "Sending...";


        const formData =
            new FormData(contactForm);


        try {

            const response = await fetch(
                contactForm.action,
                {
                    method: "POST",
                    body: formData
                }
            );


            const result = await response.json();


            if (result.success) {

                successMessage.style.display = "block";

                contactForm.reset();

                submitButton.textContent = "Message Sent";

                setTimeout(function() {

                    submitButton.disabled = false;
                    submitButton.textContent = "Send Enquiry";

                }, 3000);

            } else {

                throw new Error("Submission failed");

            }

        } catch (error) {

            errorMessage.style.display = "block";

            submitButton.disabled = false;
            submitButton.textContent = "Send Enquiry";

        }

    });

</script>

</body>
</html>