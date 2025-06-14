<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>charity: water - Landing Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --yellow: #FFC907;
      --blue: #77A8BB;
      --cream: #FFF7E1;
      --light-gray: #CBCCD1;
      --navy: #003366;
      --black: #1A1A1A;
      --peach: #FED8C1;
      --orange: #BF6C46;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Montserrat', 'Proxima Nova', sans-serif;
      background-color: var(--cream);
      color: var(--black);
    }

    a {
      text-decoration: none;
      transition: all 0.3s ease;
      font-weight: 700;
    }

    /* NAVIGATION */
    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      background-color: var(--cream);
      border-bottom: 1px solid var(--light-gray);
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    .logo-icon {
      height: 40px;
    }

    .nav-links {
      display: flex;
      gap: 1.2rem;
      align-items: center;
      flex-wrap: wrap;
    }

    .nav-links a {
      color: var(--black);
      font-size: 0.95rem;
      padding: 0.4rem 0.6rem;
      border-radius: 4px;
    }

    .nav-links a:hover {
      background-color: var(--peach);
      color: var(--navy);
    }

    .donate-btn {
      background-color: var(--yellow);
      color: var(--black);
      font-weight: 700;
      padding: 0.5rem 1rem;
      border-radius: 6px;
      font-size: 0.95rem;
      border: 2px solid transparent;
    }

    .donate-btn:hover {
      background-color: var(--peach);
      border-color: var(--yellow);
    }

    /* MAIN CONTENT */
    .container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      max-width: 1200px;
      margin: auto;
      padding: 2rem 1rem;
    }

    .hero-image {
      flex: 1 1 600px;
      position: relative;
      min-width: 300px;
    }

    .hero-image img {
      width: 100%;
      height: auto;
      border-radius: 8px;
      display: block;
    } 
    
    .overlay-text {
        position: absolute; 
        bottom: 5%;           /* Lower it so it's not covering the woman */ 
        left: 60%;          /* Center horizontally */ 
        transform: translateX(-50%); 
        background-color: rgba(0, 0, 0, 0.5); 
        color: white; 
        padding: 1rem 1.5rem;
        border-radius: 8px; 
        max-width: 80%; 
        text-align: center;
    }

    .headline {
      font-size: 2.2rem;
      font-weight: 700;
      color: var(--yellow);
      margin-bottom: 1rem;
    }

    .description {
      font-size: 1rem;
      color: var(--cream);
      line-height: 1.6;
    }

    /* RESPONSIVE DESIGN */
    @media (max-width: 768px) {
      .overlay-text {
        transform: translate(-50%, -50%);
        padding: 1rem;
      }

      .headline {
        font-size: 1.6rem;
      }

      .description {
        font-size: 0.95rem;
      }

      .nav-links {
        justify-content: center;
        gap: 0.8rem;
        margin-top: 0.5rem;
      }
    }

    @media (max-width: 480px) {
      .nav-links {
        flex-direction: column;
        align-items: center;
      }
    }
  </style>
</head>
<body>

  <!-- NAVIGATION -->
  <nav class="navbar">
    <div class="nav-left">
      <img src="https://raw.githubusercontent.com/bluegrassnellie/my-website/refs/heads/main/charity-water-logo.png" alt="Charity Water Icon" class="logo-icon" />
    </div>
    <div class="nav-links">
      <a href="#">Home</a>
      <a href="#">About</a>
      <a href="#">Our Impact</a>
      <a href="#">The Jerry Can</a>
      <a href="#" class="donate-btn">Donate Now</a>
    </div>
  </nav>

  <!-- MAIN CONTENT -->
  <main class="container">
    <div class="hero-image">
      <img src="https://raw.githubusercontent.com/bluegrassnellie/my-website/refs/heads/main/Madagascar_2019_CG-0318.jpg" alt="Water collection scene" />
      <div class="overlay-text">
        <div class="headline">Clean Water, Lead Locally. Funded Transparently</div>
        <p class="description">
          Your donation powers sustainable community-driven clean water solutions—and you’ll see the impact through GPS coordinates and authentic images from the ground.
        </p>
      </div>
    </div>
  </main>

</body>
</html>