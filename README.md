<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Portfolio">
    <title>html</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Arial', sans-serif;
            line-height: 2.6;
            background-color: #000000;
            color: #ffffff;
        }
        h1, h2 {
            color: #ffffff;
        }

        .container {
            width: 100%;
            margin: 0 auto;
            background-image: url('1.webp'); 
            background-size: cover; 
            background-position: center center; 
            background-attachment: fixed; 
        }

        header {
            background-color: #313131;
            color: #ffffff;
            padding: 30px 0;
            text-align: left;
        }
        header h1 {
            font-size: 2.5em;
            margin-left: 50px;
        }
        header p {
            font-size: 1.5em;
            margin-left: 50px;
        }


        .profile {
            display: flex;
            align-items: center;  
            justify-content: center; 
            flex-direction: column;  
            gap: 30px; 
            margin-top: 40px;  
        }

        .profile img {
            width: 350px;
            height: 350px;
            object-fit: cover;
            border-radius: 50%;
        }

        .bio {
            max-width: 700px;
            font-size: 1.5em;
            line-height: 1.8;
            text-align: center;
            margin: 0 auto; 
        }

        .hobby-section, .my-section, .skills-experience-section {
            padding: 40px 50px; 
            text-align: center; 
            background-color: #000000;
            color: #ffffff; 
        }

        .hobby-section h3, .my-section h3, .skills-experience-section h3 {
            font-size: 2.5em;
            margin-bottom: 20px;
        }

        .hobby-section p, .my-section p, .skills-experience-section p {
            font-size: 1.5em;
            line-height: 1.8; 
            max-width: 700px; 
            margin: 0 auto; 
        }


        .hobby-section p, .my-section p, .skills-experience-section p {
            margin-bottom: 20px;
        }

        .pictures-section {
            padding: 40px 0;
            text-align: center;
            background-color: #000000;
        }

        .pictures-section h3 {
            font-size: 2em;
            margin-bottom: 20px;
        }

        .pictures-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            margin-top: 20px;
        }

        .picture-box {
            background: #000000;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: transform 0.3s;
        }

        .picture-box:hover {
            transform: scale(1.05);
        }

        .picture-box img {
            width: 100%;      
            height: 200px;    
            object-fit: cover; 
            border-radius: 8px;
        }

        @media (max-width: 768px) {
            .pictures-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 480px) {
            .pictures-grid {
                grid-template-columns: 1fr;
            }

            .profile img {
                width: 300px;
                height: 300px;
            }
        }

        .contact-section {
            padding: 40px 0;
            background-color: #000000;
            text-align: center;
        }

        .contact-section h3 {
            font-size: 2.5em;
            margin-bottom: 20px;
        }

        .contact-description {
            font-size: 1.8em;
            color: #ffffff;
            margin-bottom: 20px;
        }

        .contact-links {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 20px;
        }

        .contact-link {
            font-size: 1.8em;
            color: #2b2b2b;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 10px;
            transition: color 0.3s;
            font-weight: bold;  
            font-style: italic; 
        }

        .contact-link:hover {
            color: #ee41d7; 
        }

        .social-icon {
            width: 40px;
            height: 40px;
        }

        .contact-images {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 40px;
        }

        .contact-images img {
            width: 150px;
            height: 150px;
            object-fit: cover;
            border-radius: 8px;
            transition: transform 0.3s;
        }

        .contact-images img:hover {
            transform: scale(1.1);
        }

        .skills-experience-section {
            text-align: center;
            padding: 40px 0;
            background-color: #000000;
        }

        .skills-experience-section h3 {
            font-size: 2.5em;
            margin-bottom: 20px;
        }

        .skills-experience-section p {
            font-size: 2.0em;
            color: #ffffff;
            line-height: 1.5;
            margin-bottom: 20px;
        }

        .click-me-link {
            font-size: 1.8em;
            color: #646464;
            text-decoration: none;
            font-weight: bold;
            font-style: italic;
            display: block;
            margin-top: 20px;
            text-align: center; 
        }

        .click-me-link:hover {
            color: #ee41d7;
        }

        .youtube-links {
            display: flex;
            justify-content: space-between; 
            gap: 20px; 
            margin-top: 20px;
        }

        .youtube-clips h3 {
            font-size: 2em;
            margin-bottom: 20px;
            text-align: center; 
        }

      
        .youtube-box {
            flex: 1;
            max-width: 32%;
        }

        iframe {
            width: 100%;
            height: 315px; 
            border-radius: 8px;
        }

    </style>
</head>
<body>
    <div class="container">

        <header>
            <h1>Yckho Angelo</h1>
            <p style="margin-bottom: 20px;">Information Technology Student</p>
        </header>

        <section class="profile">
            <img src="IMG_9190.jpg" alt="Your Image">
            <div class="bio">
                <h2>About Me</h2>
                <p>Hey there, I’m Yckho! 🎮✨ I’m all about creating and sharing cool content with you whether it’s streaming epic gameplay or showing off my latest drawings. 🖌️🎨 I’m here to bring you a mix of entertainment, creativity, and some good vibes. Let’s hang out, have some fun, and get inspired together!</p>
            </div>
        </section>

        <section class="hobby-section">
            <h3>My Hobbies</h3>
            <p>I love exploring different creative avenues, such as photography, painting, and gaming. Whether I’m capturing a beautiful landscape, creating digital art, or playing multiplayer games, I always find joy in my hobbies. I believe hobbies are a great way to unwind, learn, and express oneself freely.</p>
        </section>

        <section class="my-section">
            <h3>About My Work</h3>
            <p>My work involves bringing creative concepts to life through the use of technology. I enjoy combining my technical skills with my artistic flair to build engaging content, whether it’s through video editing, photography, or gaming. I aim to inspire others through my work and always seek to grow and improve my craft.</p>
        </section>

        <section class="skills-experience-section">
            <h3>Skills and Experience</h3>
            <p>I have experience with editing, photography, and creating dynamic content. My skills allow me to express myself uniquely through various creative platforms.</p>
            <p>I enjoy combining my passion for gaming, drawing, and photography to produce amazing content.</p>
        </section>

        <section class="pictures-section">
            <h3>My Photography</h3>
            <div class="contact-images">
                <div class="picture-box">
                    <img src="C1DC4E2C-BF29-40C3-A84C-EF9F9CD58CFF.jpg" alt="Picture 1">
                </div>
                <div class="picture-box">
                    <img src="IMG_9344.jpg" alt="Picture 2">
                </div>
                <div class="picture-box">
                    <img src="IMG_9331.jpg" alt="Picture 3">
                </div>
                <div class="picture-box">
                    <img src="IMG_9047.jpg" alt="Picture 1">
                </div>
                <div class="picture-box">
                    <img src="IMG_6746.jpg" alt="Picture 2">
                </div>
                <div class="picture-box">
                    <img src="IMG_6379.jpg" alt="Picture 3">
                </div>
            </div>
        </section>

        <section class="youtube-clips">
            <h3>My Clips on YouTube</h3>
            <div class="youtube-links">
                <div class="youtube-box">
                    <iframe src="https://www.youtube.com/embed/ab1V21kdtdg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
                <div class="youtube-box">
                    <iframe src="https://www.youtube.com/embed/tbohVqxvZvY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
                <div class="youtube-box">
                    <iframe src="https://www.youtube.com/embed/IDroZ9IvWAw" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>
        </section>

        <section class="contact-section">
            <h3>Contact Me</h3>
            <p class="contact-description">Feel free to reach out if you have any questions or collaboration ideas! You can connect with me on social media or through email.</p>
            <div class="contact-links">
                <a href="https://www.facebook.com/yckhoangelo.pranada/" class="contact-link">Facebook!</a>
                <a href="https://twitter.com" class="contact-link">Twitter!</a>
                <a href="https://www.instagram.com" class="contact-link">Instagram!</a>
            </div>
        </section>

        <section>
            <a href="https://www.tiktok.com/@kushsapra3d/video/7440963311333854519?is_from_webapp=1&sender_device=pc&web_id=7412321938481104402" class="click-me-link">Click me to know me more!</a>
        </section>

    </div>
</body>
</html>
