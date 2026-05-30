# Ex02 Commercial Website
### Name: Aaron H
### Register Number: 212223040001

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM

#### HTML:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Nova Essentials — Minimalist Shop</title>
  <link rel="stylesheet" href="style.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
  <header>
    <nav>
      <a href="#home" class="logo">Nova.</a>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#products">Products</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#account">Account</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>
  <section id="home" class="hero">
    <div class="hero-text">
      <h1>Designed for mindful living.</h1>
      <p>Nova Essentials designs premium, minimalist products crafted to elevate your daily routine using sustainable materials.</p>
      <a href="#products" class="btn">Explore Products</a>
    </div>
    <img class="hero-img" src="https://images.unsplash.com/photo-1513519245088-0e12902e5a38?auto=format&fit=crop&w=600&q=80" alt="Hero Image">
  </section>

  <section id="products">
    <div class="section-title">
      <h2>Curated Essentials</h2>
      <p>Everyday essentials that marry utility with timeless aesthetics.</p>
    </div>
    <div class="products-grid">
      <article class="product-card">
        <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?auto=format&fit=crop&w=500&q=80" alt="Headphones">
        <div class="product-info">
          <div class="product-meta"><span>Headphones</span><span>$249</span></div>
          <p class="product-desc">Studio-grade acoustics with lightweight sustainable aluminum body.</p>
          <button class="btn" type="button">Add to Cart</button>
        </div>
      </article>

      <article class="product-card">
        <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?auto=format&fit=crop&w=500&q=80" alt="Watch">
        <div class="product-info">
          <div class="product-meta"><span>Ceramic Watch</span><span>$185</span></div>
          <p class="product-desc">Swiss movement and custom recycled ocean plastic strap.</p>
          <button class="btn" type="button">Add to Cart</button>
        </div>
      </article>

      <article class="product-card">
        <img src="https://images.unsplash.com/photo-1526170375885-4d8ecf77b99f?auto=format&fit=crop&w=500&q=80" alt="Camera">
        <div class="product-info">
          <div class="product-meta"><span>Mirrorless Camera</span><span>$899</span></div>
          <p class="product-desc">Capture raw details with a full-frame sensor and classic controls.</p>
          <button class="btn" type="button">Add to Cart</button>
        </div>
      </article>
    </div>
  </section>


  <section id="about" class="about">
    <img class="about-img" src="https://images.unsplash.com/photo-1497366216548-37526070297c?auto=format&fit=crop&w=600&q=80" alt="Our Studio">
    <div class="about-content">
      <h2>Our Story</h2>
      <p>We believe in owning fewer things, but of much higher quality. Our products are co-designed with engineers and crafted by local artisans.</p>
      <p>Every material is intentionally chosen to create items that age beautifully with use.</p>
    </div>
  </section>
  <section id="account">
    <div class="section-title">
      <h2>User Account</h2>
      <p>Manage your orders, profile details, and rewards.</p>
    </div>
    <div class="account-card">
      <aside class="account-sidebar">
        <img class="account-avatar" src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=150&q=80" alt="Avatar">
        <h3>Clarissa Vance</h3>
        <p>Gold Member</p>
        <ul class="account-links">
          <li><a href="#account">Profile Overview</a></li>
          <li><a href="#account">Order History</a></li>
          <li><a href="#account">Saved Items</a></li>
        </ul>
      </aside>
      <div class="account-main">
        <div class="account-stats">
          <div class="stat-box"><span>Points Balance</span><h4>1,240</h4></div>
          <div class="stat-box"><span>Saved Items</span><h4>8 items</h4></div>
        </div>
        <div>
          <h4>Recent Orders</h4>
          <p style="margin-top:0.5rem; color:var(--text-muted); font-size:0.9rem;">Order #N-98402 — Delivered ($434.00)</p>
          <p style="margin-top:0.3rem; color:var(--text-muted); font-size:0.9rem;">Order #N-97391 — Delivered ($185.00)</p>
        </div>
      </div>
    </div>
  </section>
  <section id="contact" class="contact">
    <div class="contact-details">
      <h2>Let's Connect</h2>
      <p>Have questions about our products or custom orders? Reach out to us.</p>
      <div class="contact-item">
        <h4>Headquarters</h4>
        <p>58 SoHo St, Suite 400, New York, NY 10012</p>
      </div>
      <div class="contact-item">
        <h4>Email Us</h4>
        <p>concierge@novaessentials.co</p>
      </div>
    </div>
    <form class="contact-form" onsubmit="event.preventDefault(); alert('Message sent!');">
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Email Address" required>
      <textarea placeholder="How can we help you?" required></textarea>
      <button type="submit" class="btn">Send Message</button>
    </form>
  </section>

  <footer>
    <div class="footer-content">
      <p>&copy; 2026 Nova Essentials. All rights reserved.</p>
      <div class="footer-socials">
        <a href="https://instagram.com" target="_blank" aria-label="Instagram"><i class="fa-brands fa-instagram"></i></a>
        <a href="https://twitter.com" target="_blank" aria-label="Twitter"><i class="fa-brands fa-x-twitter"></i></a>
        <a href="https://pinterest.com" target="_blank" aria-label="Pinterest"><i class="fa-brands fa-pinterest"></i></a>
      </div>
    </div>
  </footer>

</body>
</html>


```

#### CSS:

```css
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600&display=swap');

:root {
  --bg: #FBFBFB;
  --panel: #FFFFFF;
  --text: #1A1A1A;
  --text-muted: #666666;
  --accent: #B38E5D;
  --border: #EEEEEE;
  --transition: all 0.2s ease;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Outfit', sans-serif;
  background-color: var(--bg);
  color: var(--text);
  line-height: 1.6;
}

header {
  position: sticky;
  top: 0;
  background: rgba(251, 251, 251, 0.9);
  backdrop-filter: blur(10px);
  border-bottom: 1px solid var(--border);
  padding: 1.2rem 5%;
  z-index: 10;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1100px;
  margin: 0 auto;
}

.logo {
  font-size: 1.3rem;
  font-weight: 600;
  text-decoration: none;
  color: var(--text);
}

.nav-links {
  display: flex;
  gap: 2rem;
  list-style: none;
}

.nav-links a {
  text-decoration: none;
  color: var(--text-muted);
  font-size: 0.9rem;
  font-weight: 400;
  transition: var(--transition);
}

.nav-links a:hover {
  color: var(--text);
}

section {
  padding: 5rem 5%;
  max-width: 1100px;
  margin: 0 auto;
}

.section-title {
  text-align: center;
  margin-bottom: 3rem;
}

.section-title h2 {
  font-size: 2rem;
  font-weight: 600;
  margin-bottom: 0.5rem;
}

.section-title p {
  color: var(--text-muted);
}

.btn {
  display: inline-block;
  padding: 0.75rem 1.5rem;
  background: var(--text);
  color: #FFF;
  text-decoration: none;
  border-radius: 4px;
  font-size: 0.9rem;
  transition: var(--transition);
  border: none;
  cursor: pointer;
}

.btn:hover {
  background: var(--accent);
}

/* Flexbox Layouts for Sections */

/* Homepage Hero */
.hero {
  display: flex;
  align-items: center;
  gap: 3rem;
  min-height: 70vh;
}

.hero-text {
  flex: 1;
}

.hero-text h1 {
  font-size: 3rem;
  line-height: 1.2;
  margin-bottom: 1rem;
}

.hero-text p {
  color: var(--text-muted);
  margin-bottom: 2rem;
}

.hero-img {
  flex: 1;
  max-height: 450px;
  object-fit: cover;
  border-radius: 6px;
}

/* Products Cards */
.products-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
}

.product-card {
  flex: 1 1 calc(33.333% - 1.34rem);
  min-width: 280px;
  background: var(--panel);
  border: 1px solid var(--border);
  border-radius: 6px;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  transition: var(--transition);
}

.product-card:hover {
  transform: translateY(-5px);
  border-color: var(--accent);
}

.product-card img {
  width: 100%;
  height: 220px;
  object-fit: cover;
}

.product-info {
  padding: 1.5rem;
  display: flex;
  flex-direction: column;
  flex-grow: 1;
  gap: 0.8rem;
}

.product-meta {
  display: flex;
  justify-content: space-between;
  font-weight: 600;
}

.product-desc {
  color: var(--text-muted);
  font-size: 0.9rem;
  flex-grow: 1;
}

/* About Us Section */
.about {
  display: flex;
  align-items: center;
  gap: 3rem;
}

.about-img {
  flex: 1;
  max-height: 400px;
  object-fit: cover;
  border-radius: 6px;
}

.about-content {
  flex: 1.2;
}

.about-content p {
  color: var(--text-muted);
  margin-bottom: 1.5rem;
}

/* User Account Section */
.account-card {
  display: flex;
  background: var(--panel);
  border: 1px solid var(--border);
  border-radius: 8px;
  overflow: hidden;
  max-width: 800px;
  margin: 0 auto;
}

.account-sidebar {
  flex: 1;
  background: #FAF9F6;
  padding: 2rem;
  border-right: 1px solid var(--border);
  text-align: center;
}

.account-avatar {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 1rem;
}

.account-sidebar h3 {
  font-size: 1.1rem;
}

.account-sidebar p {
  font-size: 0.85rem;
  color: var(--accent);
  margin-bottom: 1.5rem;
}

.account-links {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  text-align: left;
}

.account-links a {
  font-size: 0.9rem;
  color: var(--text-muted);
  text-decoration: none;
}

.account-links a:hover {
  color: var(--text);
}

.account-main {
  flex: 2;
  padding: 2rem;
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.account-stats {
  display: flex;
  gap: 1.5rem;
}

.stat-box {
  flex: 1;
  background: var(--bg);
  padding: 1rem;
  border-radius: 4px;
}

.stat-box span {
  font-size: 0.8rem;
  color: var(--text-muted);
}

.stat-box h4 {
  font-size: 1.2rem;
  margin-top: 0.2rem;
}

/* Contact Section */
.contact {
  display: flex;
  gap: 3rem;
}

.contact-details {
  flex: 1;
}

.contact-details p {
  color: var(--text-muted);
  margin-bottom: 1.5rem;
}

.contact-item {
  margin-bottom: 1rem;
}

.contact-item h4 {
  font-size: 0.9rem;
  color: var(--accent);
}

.contact-form {
  flex: 1.2;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.contact-form input, .contact-form textarea {
  width: 100%;
  padding: 0.8rem;
  border: 1px solid var(--border);
  border-radius: 4px;
  background: var(--panel);
}

.contact-form input:focus, .contact-form textarea:focus {
  outline: none;
  border-color: var(--accent);
}

/* Footer */
footer {
  background: var(--text);
  color: #FFF;
  padding: 3rem 5%;
  text-align: center;
}

.footer-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1100px;
  margin: 0 auto;
}

.footer-socials {
  display: flex;
  gap: 1.5rem;
}

.footer-socials a {
  color: #888;
  font-size: 1.2rem;
  transition: var(--transition);
}

.footer-socials a:hover {
  color: #FFF;
  transform: translateY(-2px);
}

/* Responsive */
@media (max-width: 768px) {
  .hero, .about, .contact, .account-card {
    flex-direction: column;
  }
  
  .hero-img, .about-img {
    width: 100%;
    max-height: 300px;
  }
  
  .account-sidebar {
    border-right: none;
    border-bottom: 1px solid var(--border);
  }
  
  .footer-content {
    flex-direction: column;
    gap: 1rem;
  }
}


```

## OUTPUT
<img width="1912" height="1190" alt="Screenshot 2026-05-30 at 8 14 16 AM" src="https://github.com/user-attachments/assets/2ad44aeb-8a0f-496a-a5bd-599e9117eed4" />

<img width="1912" height="1190" alt="Screenshot 2026-05-30 at 8 14 20 AM" src="https://github.com/user-attachments/assets/485cc6d4-72bf-4cc9-8bc7-afe0268973db" />

<img width="1912" height="1190" alt="Screenshot 2026-05-30 at 8 14 26 AM" src="https://github.com/user-attachments/assets/866456c7-01e3-45c7-9f50-d1d8383f56f2" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
