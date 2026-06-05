<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>REDRROX</title>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@600;800&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Smooth scroll enable */
        html {
            scroll-behavior: smooth;
        }

        body {
            background-color: #0b0c10;
            color: #ffffff;
            font-family: 'Poppins', sans-serif;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 40px 20px;
            overflow-x: hidden;
        }

        /* Main Container with Neon Red Glow */
        .container {
            width: 100%;
            max-width: 650px;
            background: #12131c;
            padding: 35px;
            border-radius: 24px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.7);
            border: 2px solid #ff003c;
            animation: slideUp 1s ease-out forwards;
            opacity: 0;
            transform: translateY(40px);
        }

        /* Header Section (Logo + Title) */
        .header {
            display: flex;
            align-items: center;
            gap: 20px;
            margin-bottom: 30px;
        }

        .logo-box {
            width: 85px;
            height: 85px;
            border-radius: 50%;
            border: 3px solid #ff003c;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            background: #0b0c10;
            box-shadow: 0 0 15px rgba(255, 0, 60, 0.4);
        }

        .logo-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .title-box {
            flex-grow: 1;
            padding: 15px 20px;
            border: 2px solid #ff003c;
            border-radius: 16px;
            background: #0b0c10;
            text-align: center;
            box-shadow: 0 0 10px rgba(255, 0, 60, 0.2);
        }

        .title-box h1 {
            font-family: 'Cinzel', serif;
            font-size: 2.2rem;
            color: #ffffff;
            letter-spacing: 3px;
            text-shadow: 0 0 15px rgba(255, 0, 60, 0.8), 0 0 5px #ff003c;
        }

        /* Description Box (About Me) with Neon Red */
        .description-box {
            border: 2px solid #ff003c;
            border-radius: 16px;
            padding: 25px;
            background: #0b0c10;
            margin-bottom: 30px;
            box-shadow: 0 0 10px rgba(255, 0, 60, 0.2);
        }

        .description-box h2 {
            font-size: 1.3rem;
            color: #ff003c;
            margin-bottom: 15px;
            text-transform: uppercase;
            letter-spacing: 1px;
            font-weight: 600;
        }

        .description-box p {
            font-size: 0.95rem;
            line-height: 1.7;
            color: #e2e4f0;
            margin-bottom: 15px;
        }

        .description-box p:last-child {
            margin-bottom: 0;
        }

        /* Social Icons Grid */
        .social-grid {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 12px;
            margin-bottom: 30px;
        }

        .social-box {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background: #0b0c10;
            border: 2px solid #ffffff;
            border-radius: 14px;
            aspect-ratio: 1;
            text-decoration: none;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            font-size: 1.6rem;
        }

        /* Social Brand Outline Alignment */
        .social-box.youtube { border-color: #ff0000; color: #ff0000; }
        .social-box.instagram { border-color: #e1306c; color: #e1306c; }
        .social-box.tiktok { border-color: #00f2fe; color: #00f2fe; }
        .social-box.telegram { border-color: #0088cc; color: #0088cc; }
        .social-box.discord { border-color: #5865f2; color: #5865f2; }

        .social-box:hover {
            transform: translateY(-8px);
            background: #ffffff;
            color: #0b0c10;
            box-shadow: 0 8px 20px rgba(255, 255, 255, 0.25);
        }

        .social-box span {
            font-size: 0.6rem;
            margin-top: 6px;
            text-transform: uppercase;
            font-weight: 600;
            letter-spacing: 0.5px;
        }

        /* Business Email Box - Green SS styled Solid Premium Accent */
        .email-box {
            border: 2px solid #45f3ff;
            border-radius: 16px;
            padding: 22px;
            background: #0b0c10;
            text-align: center;
            transition: all 0.4s ease;
            box-shadow: 0 0 15px rgba(69, 243, 255, 0.3);
        }

        .email-box:hover {
            transform: scale(1.02);
            box-shadow: 0 0 25px rgba(69, 243, 255, 0.6);
            background: #12131c;
        }

        .email-box a {
            color: #45f3ff;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 12px;
            text-shadow: 0 0 8px rgba(69, 243, 255, 0.3);
        }

        /* White Neon Glow Footer Setup */
        .footer-glow {
            margin-top: 40px;
            text-align: center;
            font-size: 0.85rem;
            font-weight: 600;
            color: #ffffff;
            letter-spacing: 2px;
            text-transform: uppercase;
            text-shadow: 0 0 8px rgba(255, 255, 255, 0.9), 0 0 20px rgba(255, 255, 255, 0.4);
            animation: fadeIn 1.5s ease-out 0.5s forwards;
            opacity: 0;
        }

        /* Keyframe Animations for Entrance Elements */
        @keyframes slideUp {
            0% {
                opacity: 0;
                transform: translateY(50px);
            }
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeIn {
            0% { opacity: 0; }
            100% { opacity: 1; }
        }

        /* Responsive Breakpoints */
        @media (max-width: 480px) {
            .header { flex-direction: column; text-align: center; }
            .social-grid { grid-template-columns: repeat(3, 1fr); gap: 10px; }
            .title-box { width: 100%; }
            .container { padding: 20px; }
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="header">
            <div class="logo-box">
                <img src="rrp.jpg" alt="RedRrox Logo">
            </div>
            <div class="title-box">
                <h1>REDRROX</h1>
            </div>
        </div>

        <div class="description-box">
            <h2>About ME :)</h2>
            <p>Welcome to my official website!</p>
            <p>I'm a passionate gamer who loves exploring new worlds, mastering challenges, and sharing exciting gaming moments with the community. This is the central hub for all my content, social media profiles, and updates. Whether you're here for gameplay, entertainment, or collaboration opportunities, you're in the right place.</p>
            <p>Feel free to connect with me through YouTube, Instagram, Discord, Telegram, TikTok, or reach out via my business email.</p>
            <p>Thanks for stopping by, and I'll see you in the game!</p>
        </div>

        <div class="social-grid">
            <a href="http://www.youtube.com/@redrrox" class="social-box youtube" target="_blank">
                <i class="fab fa-youtube"></i>
                <span>YouTube</span>
            </a>
            <a href="https://www.instagram.com/red.rrox/" class="social-box instagram" target="_blank">
                <i class="fab fa-instagram"></i>
                <span>Instagram</span>
            </a>
            <a href="https://www.tiktok.com/@redrrox?is_from_webapp=1&sender_device=pc" class="social-box tiktok" target="_blank">
                <i class="fab fa-tiktok"></i>
                <span>TikTok</span>
            </a>
            <a href="https://t.me/+ykkZkbJB6SVjZjhl" class="social-box telegram" target="_blank">
                <i class="fab fa-telegram"></i>
                <span>Telegram</span>
            </a>
            <a href="https://discord.gg/Yp4YvTVxwr" class="social-box discord" target="_blank">
                <i class="fab fa-discord"></i>
                <span>Discord</span>
            </a>
        </div>

        <div class="email-box">
            <a href="mailto:rrxstudiosofficial@gmail.com">
                <i class="fas fa-envelope"></i>
                Business Email: rrxstudiosofficial@gmail.com
            </a>
        </div>
    </div>

    <div class="footer-glow">
        &copy; 2026 REDRROX HQ | POWERED BY RRX STUDIOS
    </div>

</body>
</html>
