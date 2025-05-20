# Ex.07 Restaurant Website
## Date: 20.05.2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:

### Home.html
 ```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Sushi Zen</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500&family=Inter:wght@300;500;700&display=swap" rel="stylesheet" />
  <style>
    :root {
      --primary: #c8102e;
      --dark: #0f0f0f;
      --light: #ffffff;
      --muted: #dddddd;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: url('rest.jpg') no-repeat center center fixed;
      background-size: cover;
      color: var(--light);
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }

    .overlay {
      background: rgba(0, 0, 0, 0.6);
      width: 100%;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }

    header {
      padding: 60px 20px 30px;
      text-align: center;
      border-bottom: 1px solid #333;
    }

    header h1 {
      font-family: 'Playfair Display', serif;
      font-size: 3.5rem;
      color: var(--light);
      letter-spacing: 2px;
    }

    nav {
      display: flex;
      justify-content: center;
      gap: 30px;
      padding: 20px 0;
      background-color: rgba(0, 0, 0, 0.7);
      border-bottom: 1px solid #222;
    }

    nav a {
      text-decoration: none;
      color: var(--muted);
      font-weight: 500;
      font-size: 1rem;
      transition: 0.3s ease;
      padding: 8px 12px;
    }

    nav a:hover {
      color: var(--light);
      background-color: var(--primary);
      border-radius: 5px;
    }

    main {
      flex: 1;
      max-width: 800px;
      margin: 60px auto;
      padding: 20px;
      text-align: center;
    }

    main h2 {
      font-family: 'Playfair Display', serif;
      font-size: 2rem;
      margin-bottom: 20px;
      color: var(--primary);
    }

    main p {
      font-size: 1.1rem;
      line-height: 1.8;
      color: var(--muted);
      max-width: 700px;
      margin: 0 auto;
    }

    footer {
      background-color: rgba(0, 0, 0, 0.7);
      color: #999;
      text-align: center;
      padding: 20px 10px;
      font-size: 0.9rem;
      border-top: 1px solid #222;
    }

    footer a {
      color: var(--primary);
      text-decoration: none;
      margin: 0 10px;
    }

    footer a:hover {
      text-decoration: underline;
    }

    @media (max-width: 768px) {
      header h1 {
        font-size: 2.5rem;
      }

      nav {
        flex-direction: column;
        gap: 10px;
      }

      main {
        margin: 30px 15px;
      }
    }
  </style>
</head>
<body>
  <div class="overlay">
    <header>
      <h1>Sushi Zen</h1>
    </header>

    <nav>
      <a href="#">Home</a>
      <a href="menu.html">Menu</a>
      <a href="people.html">Admin</a>
      <a href="contact.html">Contact</a>
    </nav>

    <main>
      <h2>Welcome to Sushi Zen</h2>
      <p>
        Discover the harmony of tradition and modernity with every bite. At Sushi Zen, we serve handcrafted Japanese sushi with precision and grace in a minimalist, tranquil setting.
      </p>
    </main>

    <footer>
      <p>&copy; 2025 Sushi Zen | Designed by <strong>Adithya Sivakumar</strong></p>
      <p>
        <a href="#">Instagram</a> •
        <a href="#">Facebook</a> •
        <a href="#">Twitter</a>
      </p>
    </footer>
  </div>
</body>
</html>

 ```

### Menu.html

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Sushi Zen Menu</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500&family=Inter:wght@300;500;700&display=swap" rel="stylesheet" />
  <style>
    :root {
      --primary: #c8102e;
      --dark: #0f0f0f;
      --light: #ffffff;
      --muted: #dddddd;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: url('') no-repeat center center fixed;
      background-size: cover;
      color: var(--light);
    }

    .overlay {
      background: rgba(0, 0, 0, 0.7);
      min-height: 100vh;
      padding-bottom: 40px;
    }

    header {
      text-align: center;
      padding: 60px 20px 30px;
    }

    header h1 {
      font-family: 'Playfair Display', serif;
      font-size: 3rem;
      color: var(--light);
      letter-spacing: 2px;
    }

    header p {
      color: var(--muted);
      font-size: 1.1rem;
      margin-top: 10px;
    }

    .menu-section {
      max-width: 1100px;
      margin: 40px auto;
      padding: 0 20px;
    }

    .menu-section h2 {
      font-family: 'Playfair Display', serif;
      font-size: 2rem;
      color: var(--primary);
      border-bottom: 1px solid var(--muted);
      display: inline-block;
      margin-bottom: 20px;
    }

    .menu-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 25px;
    }

    .menu-item {
      background-color: rgba(255, 255, 255, 0.08);
      border-radius: 12px;
      overflow: hidden;
      text-align: center;
      transition: all 0.3s ease;
      border: 1px solid rgba(255, 255, 255, 0.1);
    }

    .menu-item:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.25);
    }

    .menu-item img {
      width: 100%;
      height: 180px;
      object-fit: cover;
    }

    .menu-item h3 {
      color: var(--light);
      margin: 15px 0 5px;
      font-size: 1.3rem;
    }

    .menu-item p {
      color: var(--muted);
      font-size: 0.95rem;
      margin: 0 10px 15px;
    }

    .menu-item .price {
      color: var(--primary);
      font-weight: bold;
      font-size: 1.1rem;
      margin-bottom: 15px;
    }

    footer {
      text-align: center;
      padding: 20px 0;
      background-color: rgba(0, 0, 0, 0.6);
      color: #aaa;
      font-size: 0.9rem;
      margin-top: 40px;
    }

    @media (max-width: 768px) {
      header h1 {
        font-size: 2.4rem;
      }

      .menu-item img {
        height: 150px;
      }
    }
  </style>
</head>
<body>
  <div class="overlay">
    <header>
      <h1>Sushi Zen Menu</h1>
      <p>Artisan Sushi • Authentic Japanese Cuisine</p>
    </header>

    <div class="menu-section">
      <h2>Signature Rolls</h2>
      <div class="menu-grid">
        <div class="menu-item">
          <img src="DragonRoll.jpg" alt="Dragon Roll">
          <h3>Dragon Roll</h3>
          <p>Shrimp tempura, avocado, eel sauce.</p>
          <div class="price">₹650</div>
        </div>
        <div class="menu-item">
          <img src="californiarolls.jpg" alt="California Roll">
          <h3>California Roll</h3>
          <p>Crab, cucumber, avocado, sesame seeds.</p>
          <div class="price">₹450</div>
        </div>
        <div class="menu-item">
          <img src="SpicyTunaRoll.jpg" alt="Spicy Tuna Roll">
          <h3>Spicy Tuna Roll</h3>
          <p>Tuna, chili mayo, cucumber.</p>
          <div class="price">₹500</div>
        </div>
        <div class="menu-item">
          <img src="vegroll.jpg" alt="Vegetarian Roll">
          <h3>Vegetarian Roll</h3>
          <p>Avocado, cucumber, carrot, cream cheese.</p>
          <div class="price">₹400</div>
        </div>
      </div>
    </div>

    <div class="menu-section">
      <h2>Nigiri & Sashimi</h2>
      <div class="menu-grid">
        <div class="menu-item">
          <img src="salmonnigiri.jpg" alt="Salmon Nigiri">
          <h3>Salmon Nigiri</h3>
          <p>Fresh salmon over vinegared rice.</p>
          <div class="price">₹300</div>
        </div>
        <div class="menu-item">
          <img src="tunaShashimi.jpg" alt="Tuna Sashimi">
          <h3>Tuna Sashimi</h3>
          <p>Delicate cuts of premium tuna.</p>
          <div class="price">₹550</div>
        </div>
        <div class="menu-item">
          <img src="EbiNigiri.jpg" alt="Ebi Nigiri">
          <h3>Ebi Nigiri</h3>
          <p>Sweet shrimp served over sushi rice.</p>
          <div class="price">₹320</div>
        </div>
        <div class="menu-item">
          <img src="octopus-sashimi-recipe.jpg" alt="Octopus Sashimi">
          <h3>Octopus Sashimi</h3>
          <p>Thinly sliced boiled octopus with wasabi.</p>
          <div class="price">₹480</div>
        </div>
      </div>
    </div>

    <div class="menu-section">
      <h2>Hot Dishes</h2>
      <div class="menu-grid">
        <div class="menu-item">
          <img src="miso-soup.jpg" alt="Miso Soup">
          <h3>Miso Soup</h3>
          <p>Traditional soy-based broth with tofu and seaweed.</p>
          <div class="price">₹150</div>
        </div>
        <div class="menu-item">
          <img src="Dinko-Tuna-Tempura-Prawn-recipe.jpg" alt="Prawn Tempura">
          <h3>Prawn Tempura</h3>
          <p>Lightly battered deep-fried prawns with dipping sauce.</p>
          <div class="price">₹360</div>
        </div>
        <div class="menu-item">
          <img src="Yakitori-7831-I.jpg" alt="Chicken Yakitori">
          <h3>Chicken Yakitori</h3>
          <p>Grilled skewered chicken glazed with tare sauce.</p>
          <div class="price">₹300</div>
        </div>
      </div>
    </div>

    <footer>
      <p>&copy; 2025 Sushi Zen | Crafted with harmony and taste.</p>
    </footer>
  </div>
</body>
</html>

```

### People.html

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Our Chefs</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500&family=Inter:wght@300;500;700&display=swap" rel="stylesheet" />
  <style>
    :root {
      --primary: #c8102e;
      --dark: #0f0f0f;
      --light: #ffffff;
      --muted: #dddddd;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: url('') no-repeat center center fixed;
      background-size: cover;
      color: var(--light);
    }

    .overlay {
      background: rgba(0, 0, 0, 0.7);
      min-height: 100vh;
      padding-bottom: 40px;
    }

    header {
      text-align: center;
      padding: 60px 20px 30px;
    }

    header h1 {
      font-family: 'Playfair Display', serif;
      font-size: 3rem;
      color: var(--light);
      letter-spacing: 2px;
    }

    .chefs-container {
      max-width: 1100px;
      margin: 40px auto;
      padding: 0 20px;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 25px;
    }

    .chef-card {
      background-color: rgba(255, 255, 255, 0.08);
      border-radius: 12px;
      overflow: hidden;
      text-align: center;
      transition: all 0.3s ease;
      border: 1px solid rgba(255, 255, 255, 0.1);
    }

    .chef-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.25);
    }

    .chef-card img {
      width: 100%;
      height: 180px;
      object-fit: cover;
    }

    .chef-details {
      padding: 20px;
    }

    .chef-details h1 {
      font-size: 1.3rem;
      color: var(--light);
      margin-bottom: 10px;
    }

    .chef-details h2,
    .chef-details h3 {
      font-size: 1rem;
      color: var(--muted);
      margin: 5px 0;
    }

    footer {
      text-align: center;
      padding: 20px 0;
      background-color: rgba(0, 0, 0, 0.6);
      color: #aaa;
      font-size: 0.9rem;
      margin-top: 40px;
    }

    @media (max-width: 768px) {
      header h1 {
        font-size: 2.4rem;
      }

      .chef-card img {
        height: 150px;
      }
    }
  </style>
</head>
<body>
  <div class="overlay">
    <header>
      <h1>Our Sushi Chefs</h1>
    </header>

    <div class="chefs-container">
      <div class="chef-card">
        <img src="1.jpg" alt="Chef Sato">
        <div class="chef-details">
          <h1>Chef Haruki Sato</h1>
          <h2>Designation: Executive Sushi Chef</h2>
          <h3>Experience: 15 years</h3>
        </div>
      </div>
      <div class="chef-card">
        <img src="2.jpg" alt="Chef Aiko Tanaka">
        <div class="chef-details">
          <h1>Chef Aiko Tanaka</h1>
          <h2>Designation: Nigiri Specialist</h2>
          <h3>Experience: 8 years</h3>
        </div>
      </div>
      <div class="chef-card">
        <img src="3.jpg" alt="Chef Kenji Yamamoto">
        <div class="chef-details">
          <h1>Chef Kenji Yamamoto</h1>
          <h2>Designation: Sashimi Artist</h2>
          <h3>Experience: 10 years</h3>
        </div>
      </div>
      <div class="chef-card">
        <img src="4.jpg" alt="Chef Yuki Nakamura">
        <div class="chef-details">
          <h1>Chef Yuki Nakamura</h1>
          <h2>Designation: Tempura & Hot Dish Chef</h2>
          <h3>Experience: 6 years</h3>
        </div>
      </div>
      <div class="chef-card">
        <img src="5.jpg" alt="Chef Daichi Fujiwara">
        <div class="chef-details">
          <h1>Chef Daichi Fujiwara</h1>
          <h2>Designation: Rolls & Fusion Expert</h2>
          <h3>Experience: 5 years</h3>
        </div>
      </div>
      <div class="chef-card">
        <img src="6.jpg" alt="Chef Hana Kobayashi">
        <div class="chef-details">
          <h1>Chef Hana Kobayashi</h1>
          <h2>Designation: Dessert & Presentation Chef</h2>
          <h3>Experience: 4 years</h3>
        </div>
      </div>
    </div>

    <footer>
      <p>&copy; 2025 Sushi Zen | Crafted with harmony and taste.</p>
    </footer>
  </div>
</body>
</html>

```

### Contact.html

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Contact | Sushi Zen</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500&family=Inter:wght@300;500;700&display=swap" rel="stylesheet" />
  <style>
    :root {
      --primary: #c8102e;
      --dark: #0f0f0f;
      --light: #ffffff;
      --muted: #dddddd;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: url('rest.jpg') no-repeat center center fixed;
      background-size: cover;
      color: var(--light);
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }

    .overlay {
      background: rgba(0, 0, 0, 0.6);
      width: 100%;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }

    header {
      padding: 60px 20px 30px;
      text-align: center;
      border-bottom: 1px solid #333;
    }

    header h1 {
      font-family: 'Playfair Display', serif;
      font-size: 3.5rem;
      color: var(--light);
      letter-spacing: 2px;
    }

    nav {
      display: flex;
      justify-content: center;
      gap: 30px;
      padding: 20px 0;
      background-color: rgba(0, 0, 0, 0.7);
      border-bottom: 1px solid #222;
    }

    nav a {
      text-decoration: none;
      color: var(--muted);
      font-weight: 500;
      font-size: 1rem;
      transition: 0.3s ease;
      padding: 8px 12px;
    }

    nav a:hover {
      color: var(--light);
      background-color: var(--primary);
      border-radius: 5px;
    }

    main {
      flex: 1;
      max-width: 800px;
      margin: 60px auto;
      padding: 20px;
      text-align: center;
    }

    main h2 {
      font-family: 'Playfair Display', serif;
      font-size: 2.5rem;
      margin-bottom: 20px;
      color: var(--primary);
    }

    .contact-info {
      font-size: 1.2rem;
      line-height: 2;
      color: var(--muted);
    }

    .contact-info a {
      color: var(--primary);
      text-decoration: none;
    }

    .contact-info a:hover {
      text-decoration: underline;
    }

    footer {
      background-color: rgba(0, 0, 0, 0.7);
      color: #999;
      text-align: center;
      padding: 20px 10px;
      font-size: 0.9rem;
      border-top: 1px solid #222;
    }

    footer a {
      color: var(--primary);
      text-decoration: none;
      margin: 0 10px;
    }

    footer a:hover {
      text-decoration: underline;
    }

    @media (max-width: 768px) {
      header h1 {
        font-size: 2.5rem;
      }

      nav {
        flex-direction: column;
        gap: 10px;
      }

      main {
        margin: 30px 15px;
      }
    }
  </style>
</head>
<body>
  <div class="overlay">
    <header>
      <h1>Sushi Zen</h1>
    </header>

    <nav>
      <a href="index.html">Home</a>
      <a href="menu.html">Menu</a>
      <a href="administration.html">Admin</a>
      <a href="contact.html">Contact</a>
    </nav>

    <main>
      <h2>Contact Us</h2>
      <div class="contact-info">
        <p><strong>Phone:</strong> <a href="tel:+914415443595">+91 4415443595</a></p>
        <p><strong>Email:</strong> <a href="mailto:sushi.zen@restaurant.com">sushi.zen@restaurant.com</a></p>
        <p><strong>Location:</strong> <a href="https://www.google.com/maps?q=1,+Sushi+Zen,+OMR+Street,+Perungudi">1, Sushi Zen, OMR Street, Perungudi</a></p>
      </div>
    </main>

    <footer>
      <p>&copy; 2025 Sushi Zen | Designed by <strong>Adithya Sivakumar</strong></p>
      <p>
        <a href="#">Instagram</a> •
        <a href="#">Facebook</a> •
        <a href="#">Twitter</a>
      </p>
    </footer>
  </div>
</body>
</html>

```

## OUTPUT:

![alt text](<Screenshot (449).png>)
![alt text](<Screenshot (450).png>)
![alt text](<Screenshot (451).png>)
![alt text](<Screenshot (452).png>)
![alt text](<Screenshot (453).png>)
![alt text](<Screenshot (454).png>)
![alt text](<Screenshot (455).png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
