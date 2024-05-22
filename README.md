<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>cat</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
            color: #333;
        }

        .header, .hero, .intro, .gallery, .location, .subscribe, footer {
            text-align: center;
            padding: 20px;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #fff;
            padding: 10px 20px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        .top {
            font-size: 24px;
            font-weight: bold;
        }

        .navbar ul {
            list-style: none;
            display: flex;
            gap: 20px;
        }

        .navbar a {
            text-decoration: none;
            color: #333;
        }

        .btn {
            background-color: #e67e22;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .btn:hover {
            background-color: #d35400;
        }

        .hero {
            position: relative;
            background-color: #f0e6d2;
            padding: 50px 20px;
        }

        .hero h1 {
            margin: 0;
            color: #e67e22;
        }

        .hero-img {
            width: 100%;
            max-width: 400px;
            position: absolute;
            top: 20px;
            right: 20px;
            border-radius: 10px;
        }

        .intro {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 20px;
        }

        .intro-img {
            width: 378px;
            max-width: 300px;
            border-radius: 10px;
        }

        .intro-text {
            max-width: 400px;
        }

        .gallery {
            background-color: #fff;
            padding: 40px 20px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 10px;
            margin-top: 20px;
        }

        .gallery img {
            width: 100%;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .location {
            padding: 40px 20px;
            background-color: #f9f9f9;
        }

        #map {
            width: 100%;
            height: 300px;
            background-color: #ddd;
        }

        .subscribe {
            background-color: #333;
            color: white;
            padding: 40px 20px;
        }

        .subscribe form {
            display: flex;
            justify-content: center;
            gap: 10px;
        }

        .subscribe input {
            padding: 10px;
            font-size: 16px;
            border: none;
            border-radius: 5px;
        }

        footer {
            background-color: #fff;
            padding: 20px 0;
            box-shadow: 0 -2px 4px rgba(0, 0, 0, 0.1);
        }

        .footer-logo {
            font-size: 24px;
            font-weight: bold;
        }

        .social-links {
            margin-top: 10px;
        }

        .social-links a {
            text-decoration: none;
            color: #e67e22;
            margin: 0 10px;
        }
    </style>
</head>
<body>
<!--메뉴 만들때 header > nav > ui >li 식으로 많이 사용 , Oi/ui 아래에 자식요소로는 li만 사용 가능-->
<header>
    <div class="navbar">
        <div class="top">HODU</div>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Gallery</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
<!--        <button class="btn">Download</button>-->
        <button class="btn"><a href="./image/Download%20확인.docx"> Download </a></button>
    </div>
    <div class="hero">
        <h1>Lorem Ipsum is simply dummy text of the printing and</h1>
        <button class="btn">Show more</button>
        <img src="boxcat.jpg" alt="boxcat" class="hero-img">
    </div>
</header>

<main>
    <section class="intro">
        <img width="378px" height="378px" eight="" src="cat_intro.jpg" alt="Intro Cat" class="intro-img">
        <div class="intro-text">
            <h2>Lorem Ipsum is simply dummy text of the printing</h2>
            <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
        </div>
    </section>

    <section class="gallery">
        <h2>dummy text of the printing and dummy</h2>
        <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.
            Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown.</p>
        <div class="gallery-grid">
            <img src="./image/cat1.jpg" alt="Cat 1">
            <img src="./image/cat2.jpg" alt="Cat 2">
            <img src="./image/cat3.jpg" alt="Cat 3">
            <img src="./image/cat4.jpg" alt="Cat 4">
            <img src="./image/cat5.jpg" alt="Cat 5">
            <img src="./image/cat6.jpg" alt="Cat 6">

        </div>
        <button class="btn" id="showMoreBtn">Continue exploring HODU</button>
    </section>

    <section class="location">
        <h2>Where you'll be</h2>
        <h3>330, Cheomdan-ro, Jeju-si, Jeju-do, Republic of Korea </h3>
        <div id="map"></div>
    </section>

    <section class="subscribe">
        <h2>Subscribe to our Blog post</h2>
        <form>
            <input type="email" placeholder="Enter your email">
            <button type="submit" class="btn">Subscribe</button>
        </form>
    </section>
</main>

<footer>
    <div class="footer-logo">HODU</div>
    <div class="social-links">
        <a href="https://www.facebook.com/">Facebook</a>
        <a href="https://twitter.com/">Twitter</a>
        <a href="https://www.instagram.com/">Instagram</a>
    </div>
</footer>
</body>
</html>
