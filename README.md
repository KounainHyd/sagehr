<!DOCTYPE html>
<html lang="en-GB">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sage | Accounting, Financial, HR & Payroll Software</title>
    <style>
        /* Global Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        
        body {
            color: #333;
            line-height: 1.6;
        }
        
        /* Header Styles */
        header {
            background-color: #00b388;
            color: white;
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 24px;
            font-weight: bold;
        }
        
        .logo a {
            color: white;
            text-decoration: none;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 20px;
            position: relative;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            padding: 5px 0;
        }
        
        nav ul li a:hover {
            border-bottom: 2px solid white;
        }
        
        .dropdown {
            position: relative;
            display: inline-block;
        }
        
        .dropdown-content {
            display: none;
            position: absolute;
            background-color: #f9f9f9;
            min-width: 200px;
            box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
            z-index: 1;
            left: 0;
            top: 100%;
        }
        
        .dropdown-content a {
            color: #333;
            padding: 12px 16px;
            text-decoration: none;
            display: block;
        }
        
        .dropdown-content a:hover {
            background-color: #f1f1f1;
        }
        
        .dropdown:hover .dropdown-content {
            display: block;
        }
        
        /* Hero Section */
        .hero {
            background-color: #f5f5f5;
            padding: 80px 0;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 36px;
            margin-bottom: 20px;
            color: #00b388;
        }
        
        .hero p {
            font-size: 18px;
            margin-bottom: 30px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }
        
        /* Buttons */
        .btn {
            display: inline-block;
            background-color: #00b388;
            color: white;
            padding: 12px 24px;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #008c6d;
        }
        
        /* Products Section */
        .products {
            padding: 60px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 40px;
            color: #00b388;
        }
        
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .product-card {
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 30px 20px;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        
        .product-card h3 {
            color: #00b388;
            margin-bottom: 15px;
        }
        
        .product-card img {
            max-width: 100px;
            margin-bottom: 20px;
        }
        
        /* Footer */
        footer {
            background-color: #333;
            color: white;
            padding: 40px 0 20px;
        }
        
        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }
        
        .footer-column h3 {
            margin-bottom: 20px;
            color: #00b388;
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 10px;
        }
        
        .footer-column ul li a {
            color: #ddd;
            text-decoration: none;
        }
        
        .footer-column ul li a:hover {
            color: white;
            text-decoration: underline;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid #555;
        }
        
        /* Page Content Styles */
        .page {
            display: none;
        }
        
        .page.active {
            display: block;
        }
        
        /* Contact Form Styles */
        .contact-form {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
        }
        
        .contact-form input,
        .contact-form select,
        .contact-form textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            margin-bottom: 20px;
        }
        
        .contact-form textarea {
            height: 150px;
        }
        
        /* About Page Styles */
        .about-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }
        
        /* Support Page Styles */
        .support-topic {
            background-color: white;
            text-align: left;
            padding: 20px;
        }
        
        .support-topic ul {
            list-style-type: disc;
            padding-left: 20px;
            margin-top: 15px;
        }
        
        .support-topic a {
            color: #333;
            text-decoration: none;
        }
    </style>
</head>
<body>
    <!-- Header Navigation -->
    <header>
        <div class="container header-container">
            <div class="logo"><a href="#home">SAGE</a></div>
            <nav>
                <ul>
                    <li class="dropdown">
                        <a href="#products">Products</a>
                        <div class="dropdown-content">
                            <a href="#accounting">Accounting</a>
                            <a href="#payroll">Payroll</a>
                            <a href="#hr">HR</a>
                        </div>
                    </li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#support">Support</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Home Page -->
    <section id="home" class="page active">
        <section class="hero">
            <div class="container">
                <h1>Accounting, Financial, HR & Payroll Software</h1>
                <p>Powerful, easy-to-use accounting software for businesses of all sizes. Trusted by millions of businesses worldwide to manage their finances, payroll, and HR needs.</p>
                <a href="#products" class="btn">Explore Our Products</a>
            </div>
        </section>
        
        <section class="products">
            <div class="container">
                <h2 class="section-title">Our Solutions</h2>
                <div class="product-grid">
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Accounting" alt="Accounting">
                        <h3>Sage Accounting</h3>
                        <p>Simple accounting software for small businesses and sole traders.</p>
                        <a href="#accounting" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Payroll" alt="Payroll">
                        <h3>Sage Payroll</h3>
                        <p>Easy-to-use payroll software that makes paying your people simple.</p>
                        <a href="#payroll" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=HR" alt="HR">
                        <h3>Sage HR</h3>
                        <p>People management software to help you manage your workforce.</p>
                        <a href="#hr" class="btn">Learn More</a>
                    </div>
                </div>
            </div>
        </section>
    </section>

    <!-- Products Page -->
    <section id="products" class="page">
        <section class="hero">
            <div class="container">
                <h1>Our Business Software Solutions</h1>
                <p>Discover the perfect software solution for your business needs, whether you're a startup, growing business, or established enterprise.</p>
            </div>
        </section>
        
        <section class="products">
            <div class="container">
                <h2 class="section-title">Our Product Range</h2>
                <div class="product-grid">
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Accounting" alt="Accounting">
                        <h3>Sage Accounting</h3>
                        <p>Comprehensive accounting solutions for businesses of all sizes.</p>
                        <a href="#accounting" class="btn">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Payroll" alt="Payroll">
                        <h3>Sage Payroll</h3>
                        <p>Streamline your payroll processes with our powerful software.</p>
                        <a href="#payroll" class="btn">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=HR" alt="HR">
                        <h3>Sage HR</h3>
                        <p>Manage your workforce efficiently with our HR solutions.</p>
                        <a href="#hr" class="btn">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Enterprise" alt="Enterprise">
                        <h3>Sage Enterprise</h3>
                        <p>Scalable solutions for large businesses with complex needs.</p>
                        <a href="#" class="btn">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=CRM" alt="CRM">
                        <h3>Sage CRM</h3>
                        <p>Customer relationship management to grow your business.</p>
                        <a href="#" class="btn">View Details</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Construction" alt="Construction">
                        <h3>Sage for Construction</h3>
                        <p>Specialized solutions for the construction industry.</p>
                        <a href="#" class="btn">View Details</a>
                    </div>
                </div>
            </div>
        </section>
    </section>

    <!-- Accounting Page -->
    <section id="accounting" class="page">
        <section class="hero">
            <div class="container">
                <h1>Sage Accounting Software</h1>
                <p>Simple, smart accounting software designed to save you time and help you make better business decisions.</p>
                <a href="#contact" class="btn">Get Started</a>
            </div>
        </section>
        
        <section class="products">
            <div class="container">
                <h2 class="section-title">Accounting Solutions for Your Business</h2>
                <div class="product-grid">
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Sage+50" alt="Sage 50">
                        <h3>Sage 50cloud</h3>
                        <p>Powerful accounting software for small and medium businesses.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Sage+200" alt="Sage 200">
                        <h3>Sage 200cloud</h3>
                        <p>Advanced accounting and business management software.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Sage+Intacct" alt="Sage Intacct">
                        <h3>Sage Intacct</h3>
                        <p>Cloud financial management for growing businesses.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                </div>
            </div>
        </section>
        
        <section class="products" style="background-color: #f5f5f5; padding: 60px 0;">
            <div class="container">
                <h2 class="section-title">Key Features</h2>
                <div class="product-grid">
                    <div class="product-card" style="background-color: white;">
                        <h3>Invoicing</h3>
                        <p>Create and send professional invoices in seconds.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Expense Tracking</h3>
                        <p>Keep track of business expenses and receipts.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Financial Reporting</h3>
                        <p>Generate detailed financial reports with ease.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Bank Reconciliation</h3>
                        <p>Automatically match transactions with your bank.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>VAT Management</h3>
                        <p>Calculate and submit VAT returns directly to HMRC.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Multi-User Access</h3>
                        <p>Collaborate with your team securely.</p>
                    </div>
                </div>
            </div>
        </section>
    </section>

    <!-- Payroll Page -->
    <section id="payroll" class="page">
        <section class="hero">
            <div class="container">
                <h1>Sage Payroll Software</h1>
                <p>Simplify your payroll processes and ensure compliance with our powerful payroll solutions.</p>
                <a href="#contact" class="btn">Get Started</a>
            </div>
        </section>
        
        <section class="products">
            <div class="container">
                <h2 class="section-title">Payroll Solutions</h2>
                <div class="product-grid">
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Sage+50+Payroll" alt="Sage 50 Payroll">
                        <h3>Sage 50 Payroll</h3>
                        <p>Comprehensive payroll software for small businesses.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Sage+200+Payroll" alt="Sage 200 Payroll">
                        <h3>Sage 200 Payroll</h3>
                        <p>Advanced payroll for medium-sized businesses.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Sage+Cloud+Payroll" alt="Sage Cloud Payroll">
                        <h3>Sage Cloud Payroll</h3>
                        <p>Flexible, cloud-based payroll solution.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                </div>
            </div>
        </section>
        
        <section class="products" style="background-color: #f5f5f5; padding: 60px 0;">
            <div class="container">
                <h2 class="section-title">Why Choose Sage Payroll?</h2>
                <div class="product-grid">
                    <div class="product-card" style="background-color: white;">
                        <h3>RTI Compliant</h3>
                        <p>Fully compliant with HMRC's Real Time Information requirements.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Auto Enrolment</h3>
                        <p>Simplified workplace pension management.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Employee Self-Service</h3>
                        <p>Employees can access payslips and documents online.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Integration</h3>
                        <p>Seamless integration with Sage Accounting software.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Support</h3>
                        <p>Dedicated payroll support when you need it.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Reporting</h3>
                        <p>Comprehensive payroll reporting at your fingertips.</p>
                    </div>
                </div>
            </div>
        </section>
    </section>

    <!-- HR Page -->
    <section id="hr" class="page">
        <section class="hero">
            <div class="container">
                <h1>Sage HR Software</h1>
                <p>Transform your people management with intuitive HR software designed for modern businesses.</p>
                <a href="#contact" class="btn">Get Started</a>
            </div>
        </section>
        
        <section class="products">
            <div class="container">
                <h2 class="section-title">HR Solutions</h2>
                <div class="product-grid">
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Sage+HR" alt="Sage HR">
                        <h3>Sage HR</h3>
                        <p>Cloud-based HR software for people management.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Sage+People" alt="Sage People">
                        <h3>Sage People</h3>
                        <p>HR and people system for medium to large businesses.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Sage+HR+Essentials" alt="Sage HR Essentials">
                        <h3>Sage HR Essentials</h3>
                        <p>Simple HR software for small businesses.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                </div>
            </div>
        </section>
        
        <section class="products" style="background-color: #f5f5f5; padding: 60px 0;">
            <div class="container">
                <h2 class="section-title">HR Features</h2>
                <div class="product-grid">
                    <div class="product-card" style="background-color: white;">
                        <h3>Employee Records</h3>
                        <p>Centralized, secure employee records management.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Leave Management</h3>
                        <p>Streamline holiday requests and approvals.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Performance Management</h3>
                        <p>Track and improve employee performance.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Recruitment</h3>
                        <p>Manage your hiring process from start to finish.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Reporting</h3>
                        <p>Generate insightful HR reports and analytics.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Integration</h3>
                        <p>Connect with payroll and accounting systems.</p>
                    </div>
                </div>
            </div>
        </section>
    </section>

    <!-- Services Page -->
    <section id="services" class="page">
        <section class="hero">
            <div class="container">
                <h1>Sage Business Services</h1>
                <p>Expert services to help you get the most from your Sage software and grow your business.</p>
            </div>
        </section>
        
        <section class="products">
            <div class="container">
                <h2 class="section-title">Our Services</h2>
                <div class="product-grid">
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Implementation" alt="Implementation">
                        <h3>Implementation</h3>
                        <p>Get your Sage software up and running quickly with our expert implementation services.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Training" alt="Training">
                        <h3>Training</h3>
                        <p>Maximize your software investment with tailored training for your team.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Consulting" alt="Consulting">
                        <h3>Consulting</h3>
                        <p>Expert advice to optimize your business processes and software usage.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Support" alt="Support">
                        <h3>Premium Support</h3>
                        <p>Get priority assistance when you need it most with our premium support plans.</p>
                        <a href="#support" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Customization" alt="Customization">
                        <h3>Customization</h3>
                        <p>Tailor your Sage software to meet your specific business requirements.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Integration" alt="Integration">
                        <h3>Integration</h3>
                        <p>Connect your Sage software with other business applications.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                </div>
            </div>
        </section>
    </section>

    <!-- Support Page -->
    <section id="support" class="page">
        <section class="hero">
            <div class="container">
                <h1>Sage Support</h1>
                <p>Get help when you need it with our comprehensive support resources and services.</p>
            </div>
        </section>
        
        <section class="products">
            <div class="container">
                <h2 class="section-title">Support Options</h2>
                <div class="product-grid">
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Help+Center" alt="Help Center">
                        <h3>Help Center</h3>
                        <p>Find answers to common questions in our comprehensive knowledge base.</p>
                        <a href="#" class="btn">Visit Help Center</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Community" alt="Community">
                        <h3>Community</h3>
                        <p>Connect with other Sage users and experts in our community forums.</p>
                        <a href="#" class="btn">Join Community</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Contact+Support" alt="Contact Support">
                        <h3>Contact Support</h3>
                        <p>Get direct assistance from our support team via phone, chat, or email.</p>
                        <a href="#contact" class="btn">Contact Us</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Training" alt="Training">
                        <h3>Training</h3>
                        <p>Attend live training sessions or watch on-demand tutorials.</p>
                        <a href="#services" class="btn">View Training</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Updates" alt="Updates">
                        <h3>Software Updates</h3>
                        <p>Download the latest updates and patches for your Sage software.</p>
                        <a href="#" class="btn">Check for Updates</a>
                    </div>
                    <div class="product-card">
                        <img src="https://via.placeholder.com/100x100?text=Premium+Support" alt="Premium Support">
                        <h3>Premium Support</h3>
                        <p>Upgrade to premium support for faster response times and dedicated help.</p>
                        <a href="#" class="btn">Learn More</a>
                    </div>
                </div>
            </div>
        </section>
        
        <section class="products" style="background-color: #f5f5f5; padding: 60px 0;">
            <div class="container">
                <h2 class="section-title">Popular Support Topics</h2>
                <div class="product-grid">
                    <div class="support-topic">
                        <h3 style="color: #00b388;">Installation & Setup</h3>
                        <ul>
                            <li><a href="#">How to install Sage software</a></li>
                            <li><a href="#">System requirements</a></li>
                            <li><a href="#">Migration from older versions</a></li>
                        </ul>
                    </div>
                    <div class="support-topic">
                        <h3 style="color: #00b388;">Troubleshooting</h3>
                        <ul>
                            <li><a href="#">Common error messages</a></li>
                            <li><a href="#">Performance issues</a></li>
                            <li><a href="#">Connectivity problems</a></li>
                        </ul>
                    </div>
                    <div class="support-topic">
                        <h3 style="color: #00b388;">How-To Guides</h3>
                        <ul>
                            <li><a href="#">Creating invoices</a></li>
                            <li><a href="#">Processing payroll</a></li>
                            <li><a href="#">Generating reports</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>
    </section>

    <!-- About Page -->
    <section id="about" class="page">
        <section class="hero">
            <div class="container">
                <h1>About Sage</h1>
                <p>Helping businesses of all sizes manage their money, people, and operations for over 40 years.</p>
            </div>
        </section>
        
        <section class="products">
            <div class="container">
                <div class="about-content">
                    <h2 class="section-title">Our Story</h2>
                    <p style="margin-bottom: 30px;">Founded in 1981, Sage has grown from a small startup to a global leader in business software. What began as a simple accounting solution has evolved into a comprehensive suite of products that help millions of businesses worldwide manage their finances, operations, and people.</p>
                    
                    <h2 class="section-title">Our Mission</h2>
                    <p style="margin-bottom: 30px;">We exist to knock down barriers so everyone can thrive. We do this by helping businesses of all sizes manage their money, people, and operations—freeing them up to focus on doing what they love.</p>
                    
                    <h2 class="section-title">By the Numbers</h2>
                    <div class="product-grid" style="margin-top: 40px;">
                        <div class="product-card">
                            <h3>13,000+</h3>
                            <p>Employees Worldwide</p>
                        </div>
                        <div class="product-card">
                            <h3>Millions</h3>
                            <p>Customers Globally</p>
                        </div>
                        <div class="product-card">
                            <h3>23</h3>
                            <p>Countries With Offices</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <section class="products" style="background-color: #f5f5f5; padding: 60px 0;">
            <div class="container">
                <h2 class="section-title">Our Values</h2>
                <div class="product-grid">
                    <div class="product-card" style="background-color: white;">
                        <h3>Human</h3>
                        <p>We treat everyone with care and respect, valuing different perspectives.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Trust</h3>
                        <p>We build trust through transparency, integrity, and delivering on our promises.</p>
                    </div>
                    <div class="product-card" style="background-color: white;">
                        <h3>Innovation</h3>
                        <p>We're curious and bold, always looking for better ways to solve problems.</p>
                    </div>
                </div>
            </div>
        </section>
    </section>

    <!-- Contact Page -->
    <section id="contact" class="page">
        <section class="hero">
            <div class="container">
                <h1>Contact Sage</h1>
                <p>We're here to help. Get in touch with our team for sales, support, or general inquiries.</p>
            </div>
        </section>
        
        <section class="products">
            <div class="container">
                <div class="contact-form">
                    <div>
                        <h2 class="section-title" style="text-align: left;">Contact Form</h2>
                        <form style="margin-top: 20px;">
                            <div style="margin-bottom: 20px;">
                                <label for="name" style="display: block; margin-bottom: 5px; font-weight: bold;">Name</label>
                                <input type="text" id="name" name="name">
                            </div>
                            <div style="margin-bottom: 20px;">
                                <label for="email" style="display: block; margin-bottom: 5px; font-weight: bold;">Email</label>
                                <input type="email" id="email" name="email">
                            </div>
                            <div style="margin-bottom: 20px;">
                                <label for="subject" style="display: block; margin-bottom: 5px; font-weight: bold;">Subject</label>
                                <select id="subject" name="subject">
                                    <option value="sales">Sales Inquiry</option>
                                    <option value="support">Support Request</option>
                                    <option value="general">General Inquiry</option>
                                </select>
                            </div>
                            <div style="margin-bottom: 20px;">
                                <label for="message" style="display: block; margin-bottom: 5px; font-weight: bold;">Message</label>
                                <textarea id="message" name="message" rows="5"></textarea>
                            </div>
                            <button type="submit" class="btn" style="border: none; cursor: pointer;">Send Message</button>
                        </form>
                    </div>
                    <div>
                        <h2 class="section-title" style="text-align: left;">Contact Information</h2>
                        <div style="margin-top: 30px;">
                            <h3 style="color: #00b388; margin-bottom: 15px;">Headquarters</h3>
                            <p style="margin-bottom: 20px;">
                                Sage Group plc<br>
                                North Park<br>
                                Newcastle upon Tyne<br>
                                NE13 9AA<br>
                                United Kingdom
                            </p>
                            
                            <h3 style="color: #00b388; margin-bottom: 15px;">Phone</h3>
                            <p style="margin-bottom: 20px;">
                                +91 6304801022<br>
                                International: +91 9948693861
                            </p>
                            
                            <h3 style="color: #00b388; margin-bottom: 15px;">Email</h3>
                            <p style="margin-bottom: 20px;">
                                General inquiries: info@sagehr.com<br>
                                Support: support@sagehr.com
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <section class="products" style="background-color: #f5f5f5; padding: 60px 0;">
            <div class="container">
                <h2 class="section-title">Regional Offices</h2>
                <div class="product-grid">
                    <div class="product-card" style="background-color: white; text-align: left;">
                        <h3 style="color: #00b388;">United States</h3>
                        <p>
                            6561 Irvine Center Drive<br>
                            Irvine, CA 92618<br>
                            Phone: +1 866-996-7243
                        </p>
                    </div>
                    <div class="product-card" style="background-color: white; text-align: left;">
                        <h3 style="color: #00b388;">Canada</h3>
                        <p>
                            2000 Argentia Road<br>
                            Plaza 1, Suite 400<br>
                            Mississauga, ON L5N 2R7<br>
                            Phone: +1 800-361-3223
                        </p>
                    </div>
                    <div class="product-card" style="background-color: white; text-align: left;">
                        <h3 style="color: #00b388;">France</h3>
                        <p>
                            10 rue de la Paix<br>
                            75002 Paris<br>
                            Phone: +33 (0)1 55 07 88 00
                        </p>
                    </div>
                </div>
            </div>
        </section>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-column">
                    <h3>Products</h3>
                    <ul>
                        <li><a href="#accounting">Accounting</a></li>
                        <li><a href="#payroll">Payroll</a></li>
                        <li><a href="#hr">HR</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Company</h3>
                    <ul>
                        <li><a href="#about">About Us</a></li>
                        <li><a href="#contact">Contact</a></li>
                        <li><a href="#">Careers</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Resources</h3>
                    <ul>
                        <li><a href="#support">Support</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#">Blog</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Legal</h3>
                    <ul>
                        <li><a href="#">Terms of Service</a></li>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Cookie Policy</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 Sage. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Simple page navigation
        document.addEventListener('DOMContentLoaded', function() {
            // Show home page by default
            showPage('home');
            
            // Handle navigation clicks
            document.querySelectorAll('nav a, .dropdown-content a, .btn[href^="#"]').forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    const pageId = this.getAttribute('href').substring(1);
                    showPage(pageId);
                    window.scrollTo(0, 0);
                });
            });
            
            // Handle initial hash in URL
            if (window.location.hash) {
                const pageId = window.location.hash.substring(1);
                showPage(pageId);
            }
        });
        
        function showPage(pageId) {
            // Hide all pages
            document.querySelectorAll('.page').forEach(page => {
                page.classList.remove('active');
            });
            
            // Show selected page
            const page = document.getElementById(pageId);
            if (page) {
                page.classList.add('active');
                window.location.hash = pageId;
            } else {
                // Default to home if page not found
                document.getElementById('home').classList.add('active');
                window.location.hash = 'home';
            }
        }
    </script>
</body>
</html>
