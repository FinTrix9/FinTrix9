# FinTrix9
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Responsive Header</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css"/>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    .header {
        background-color: #2511d4;
      color: white;
      padding: 15px 5px;
      display: flex;
      align-items: center;
      justify-content: space-around;
      margin: 10px auto;
      width: 95vw;
      border-radius: 75px;
      position: sticky;
      top: 0; /* This makes the header stick to the top */
      z-index: 1000;
    }

    .header h1 {
      margin: 0;
      font-size: 2rem;
    }

    .nav {
      display: flex;
      gap: 20px;
    }

    .nav a {
      text-decoration: none;
      color: white;
      font-weight: bold;
      padding: 10px 15px;
      border-radius: 10px;
      transition: background-color 0.3s;
      font-size: 15px;
    }

    .nav a:hover {
      background-color: #45a049;
    }

    /* Mobile responsive header */
    @media (max-width: 600px) {
  .header {
    flex-direction: column; /* Stack the logo and nav vertically */
    align-items: center; /* Center them */
    margin: auto;
  }

  .header h1 {
    margin-bottom: 10px; /* Space between the logo and the nav */
  }

  .nav {
    display: flex;
    flex-direction: row; /* Keep the nav links in a single row */
    gap: 0px;
    margin-top: 7px; /* Add space above the nav links */
  }

  .nav a {
    font-size: 14px;
    padding: 4px 8px;
  }
}



    main {
      padding: 20px;
    }

    .autotab {
      width: 100%;
      height: 30vh;
      background-color: #ffffff;
      border-radius: 10px;
      margin-top: 20px;
    }

    .info {
      width: 100%;
      background-color: #ffffff;
      border-radius: 10px;
      margin-top: 20px;
    }

    .swiper {
      width: 100%;
      height: 100%;
    }

    .swiper-slide {
      display: flex;
      justify-content: center;
      align-items: center;
      background: #eee;
    }

    .swiper-slide img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      border-radius: 10px;
    }

    .boxes {
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 20px;
      padding: 20px;
    }

    .box {
      display: flex;
      flex-direction: column;
      width: 220px;
      height: 330px;
      background: linear-gradient(135deg, #1e1e2f, #3b3b5c);
      justify-content: space-between;
      align-items: center;
      border-radius: 20px;
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      padding: 15px;
    }

    .box:hover {
      transform: translateY(-5px);
      box-shadow: 0 12px 24px rgba(0, 0, 0, 0.4);
    }

    .box img {
      width: 80px;
      height: 80px;
      border-radius: 50%;
      border: 3px solid white;
      margin-bottom: 10px;
    }

    .box h2 {
      color: #ffffff;
      text-align: center;
      margin: 10px 0 5px;
      font-size: 1.2rem;
    }

    .tags {
      display: flex;
      gap: 8px;
      flex-wrap: wrap;
      justify-content: center;
      margin-bottom: 10px;
    }

    .tag {
      background-color: #45a049;
      color: white;
      font-size: 12px;
      padding: 3px 8px;
      border-radius: 12px;
    }

    .box p {
      color: #dcdcdc;
      text-align: center;
      margin: 0 10px;
      font-size: 0.9rem;
      flex-grow: 1;
    }

    .join-btn {
      padding: 12px 24px;
      background-color: #4CAF50;
      color: white;
      font-size: 16px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: transform 0.3s ease, background-color 0.3s ease;
      margin-top: 15px;
    }

    .join-btn:hover {
      background-color: #45a049;
      transform: scale(1.1);
    }

    .join-btn:focus {
      animation: pulse 1s infinite;
    }

    @keyframes pulse {
      0% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.2);
      }
      100% {
        transform: scale(1);
      }
    }

    /* Media query for smaller screens */
    @media (max-width: 600px) {
      .boxes {
        justify-content: center;
      }

      .box {
        width: 90%;
        margin-bottom: 20px;
        height: auto;
        padding: 20px;
      }

      .nav a {
        font-size: 14px;
        padding: 8px 12px;
      }

      /* Increased slider height for small screens */
      .autotab {
        height: 50vh;
      }
    }

  </style>
</head>
<body>
  <header class="header">
    <h1>FinTrix9</h1>
    <nav class="nav">
      <a href="#home">Home</a>
      <a href="#airdrops">Airdrops</a>
      <a href="#news">News</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
      <a href="#donate">Donate</a>
    </nav>
  </header>

  <main>
    <div class="autotab">
      <div class="swiper image-slider">
        <div class="swiper-wrapper">
          <div class="swiper-slide"><img src="images/img1.jpg" alt="Image 1"></div>
          <div class="swiper-slide"><img src="images/img2.png" alt="Image 2"></div>
          <div class="swiper-slide"><img src="images/img3.webp" alt="Image 3"></div>
          <div class="swiper-slide"><img src="images/img4.png" alt="Image 4"></div>
          <div class="swiper-slide"><img src="images/img5.jpg" alt="Image 5"></div>
          <div class="swiper-slide"><img src="images/img6.jpg" alt="Image 6"></div>
        </div>
        <div class="swiper-pagination"></div>
        <div class="swiper-button-prev" aria-label="Previous slide"></div>
        <div class="swiper-button-next" aria-label="Next slide"></div>
      </div>
    </div>

    <div class="info">
      <div class="boxes">
        <div class="box">
          <img src="imggradient.jpg" alt="Gradient">
          <h2>GRADIENT</h2>
          <div class="tags">
            <span class="tag">CSS</span>
            <span class="tag">Color</span>
          </div>
          <p>A smooth transition between two or more colors.</p>
          <button class="join-btn">Join Airdrop</button>
        </div>
        <div class="box">
          <img src="imggradient.jpg" alt="Design">
          <h2>DESIGN</h2>
          <div class="tags">
            <span class="tag">UI</span>
            <span class="tag">UX</span>
          </div>
          <p>Combines creativity and logic for stunning visuals.</p>
          <button class="join-btn">Join Airdrop</button>
        </div>
        <div class="box">
          <img src="imggradient.jpg" alt="Develop">
          <h2>DEVELOP</h2>
          <div class="tags">
            <span class="tag">Code</span>
            <span class="tag">Web</span>
          </div>
          <p>Transforms ideas into functional web solutions.</p>
          <button class="join-btn">Join</button>
        </div>
        <div class="box">
          <img src="imggradient.jpg" alt="Strategy">
          <h2>STRATEGY</h2>
          <div class="tags">
            <span class="tag">Plan</span>
            <span class="tag">Marketing</span>
          </div>
          <p>Blueprint for achieving long-term success online.</p>
          <button class="join-btn">Join</button>
        </div>
        <div class="box">
          <img src="imggradient.jpg" alt="Branding">
          <h2>BRANDING</h2>
          <div class="tags">
            <span class="tag">Logo</span>
            <span class="tag">Identity</span>
          </div>
          <p>Shapes the perception of your product or service.</p>
          <button class="join-btn">Join</button>
        </div>
        <div class="box">
          <img src="imggradient.jpg" alt="Analytics">
          <h2>ANALYTICS</h2>
          <div class="tags">
            <span class="tag">Data</span>
            <span class="tag">Reports</span>
          </div>
          <p>Gathers insights from user data and performance.</p>
          <button class="join-btn">Join</button>
        </div>
      </div>
    </div>
  </main>

  <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
  <script>
    const swiper = new Swiper('.image-slider', {
      loop: true,
      autoplay: {
        delay: 3000,
        disableOnInteraction: false,
      },
      pagination: {
        el: '.swiper-pagination',
        clickable: true,
      },
      navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
      },
      breakpoints: {
        0: {
          slidesPerView: 1,
        },
        768: {
          slidesPerView: 2,
        },
        1024: {
          slidesPerView: 3,
        },
      },
    });
  </script>
</body>
</html>
