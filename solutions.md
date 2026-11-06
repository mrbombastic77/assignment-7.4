HTML
<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modern Landing Page - Header & Hero</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Header Section -->
    <header class="site-header">
        <div class="header-container">
            <div class="logo">
                <a href="#">DevLaunch</a>
            </div>
            <nav class="nav-menu">
                <ul class="nav-links">
                    <li><a href="#features">Features</a></li>
                    <li><a href="#solutions">Solutions</a></li>
                    <li><a href="#pricing">Pricing</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
            <div class="header-action">
                <a href="#" class="btn btn-outline">Sign In</a>
                <a href="#" class="btn btn-primary">Get Started</a>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <main class="main-content">
        <section class="hero-section">
            <div class="hero-container">
                <div class="hero-text-content">
                    <span class="badge">Version 2.0 Live</span>
                    <h1>Build Modern Web Applications Faster</h1>
                    <p>A comprehensive platform designed for developers to craft responsive interfaces, streamline workflows, and ship projects with confidence.</p>
                    <div class="hero-buttons">
                        <a href="#" class="btn btn-primary btn-lg">Start Free Trial</a>
                        <a href="#" class="btn btn-outline btn-lg">View Documentation</a>
                    </div>
                </div>
                <div class="hero-image-wrapper">
                    <img src="images/hero-illustration.jpg" alt="Developer dashboard illustration showing responsive web design layout" class="hero-img">
                </div>
            </div>
        </section>
    </main>

    <!-- Footer Section -->
    <footer class="site-footer">
        <div class="footer-container">
            <p>&copy; 2026 DevLaunch, Invertis University. All rights reserved.</p>
            <ul class="footer-links">
                <li><a href="#">Privacy Policy</a></li>
                <li><a href="#">Terms of Service</a></li>
                <li><a href="#">Support</a></li>
            </ul>
        </div>
    </footer>
</body>
</html>
CSS
/* style.css */
:root {
    --primary-color: #0284c7;
    --primary-hover: #0369a1;
    --secondary-color: #0f172a;
    --bg-color: #f8fafc;
    --surface-color: #ffffff;
    --text-color: #334155;
    --text-muted: #64748b;
    --border-color: #e2e8f0;

    --space-sm: 8px;
    --space-md: 16px;
    --space-lg: 24px;
    --space-xl: 40px;

    --radius-md: 8px;
    --radius-lg: 12px;
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: Arial, sans-serif;
    background-color: var(--bg-color);
    color: var(--text-color);
    line-height: 1.6;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

/* Header & Navigation Styling */
.site-header {
    background-color: var(--surface-color);
    border-bottom: 1px solid var(--border-color);
    position: sticky;
    top: 0;
    z-index: 1000;
    padding: var(--space-md) var(--space-xl);
}

.header-container {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: var(--space-md);
}

.logo a {
    font-size: 1.5rem;
    font-weight: bold;
    color: var(--secondary-color);
    text-decoration: none;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: var(--space-lg);
}

.nav-links a {
    color: var(--text-muted);
    text-decoration: none;
    font-weight: 500;
    transition: color 0.2s ease;
}

.nav-links a:hover {
    color: var(--primary-color);
}

.header-action {
    display: flex;
    gap: var(--space-md);
    align-items: center;
}

/* Hero Section Styling */
.main-content {
    flex-grow: 1;
    display: flex;
    align-items: center;
}

.hero-section {
    width: 100%;
    padding: 4rem var(--space-xl);
}

.hero-container {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 3rem;
    flex-wrap: wrap;
}

.hero-text-content {
    flex: 1;
    min-width: 300px;
    max-width: 560px;
}

.badge {
    display: inline-block;
    background-color: #e0f2fe;
    color: var(--primary-color);
    font-size: 0.75rem;
    font-weight: bold;
    padding: 4px 12px;
    border-radius: 20px;
    text-transform: uppercase;
    margin-bottom: var(--space-md);
}

.hero-text-content h1 {
    font-size: 2.75rem;
    color: var(--secondary-color);
    line-height: 1.2;
    margin-bottom: var(--space-md);
}

.hero-text-content p {
    font-size: 1.125rem;
    color: var(--text-muted);
    margin-bottom: var(--space-lg);
}

.hero-buttons {
    display: flex;
    gap: var(--space-md);
    flex-wrap: wrap;
}

.hero-image-wrapper {
    flex: 1;
    min-width: 300px;
    max-width: 540px;
    background-color: var(--border-color);
    border-radius: var(--radius-lg);
    overflow: hidden;
    box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
}

.hero-img {
    width: 100%;
    height: auto;
    display: block;
    object-fit: cover;
}

/* Common Button Styles */
.btn {
    padding: 0.6rem 1.25rem;
    font-size: 0.95rem;
    font-weight: bold;
    border-radius: var(--radius-md);
    text-decoration: none;
    cursor: pointer;
    transition: background-color 0.2s ease, transform 0.1s ease;
    display: inline-block;
    text-align: center;
}

.btn-primary {
    background-color: var(--primary-color);
    color: var(--surface-color);
}

.btn-primary:hover {
    background-color: var(--primary-hover);
}

.btn-outline {
    background-color: transparent;
    border: 1px solid var(--border-color);
    color: var(--secondary-color);
}

.btn-outline:hover {
    background-color: #f1f5f9;
    border-color: var(--text-muted);
}

.btn-lg {
    padding: 0.75rem 1.5rem;
    font-size: 1rem;
}

/* Footer Section */
.site-footer {
    background-color: var(--secondary-color);
    color: var(--surface-color);
    padding: var(--space-lg) var(--space-xl);
    border-top: 1px solid var(--border-color);
}

.footer-container {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: var(--space-md);
}

.footer-links {
    list-style: none;
    display: flex;
    gap: var(--space-lg);
}

.footer-links a {
    color: var(--text-muted);
    text-decoration: none;
    font-size: 0.875rem;
    transition: color 0.2s ease;
}

.footer-links a:hover {
    color: var(--surface-color);
}