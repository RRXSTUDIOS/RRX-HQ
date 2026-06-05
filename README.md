<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RedRrox Portfolio</title>
    <!-- Google Fonts for Premium look -->
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@600;800&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <!-- FontAwesome for Social Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: #0b0c10;
            color: #ffffff;
            font-family: 'Poppins', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            width: 100%;
            max-width: 650px;
            background: #1f2833;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
            border: 1px solid #45f3ff;
        }

        /* Header Section (Logo + Title) */
        .header {
            display: flex;
            align-items: center;
            gap: 20px;
            margin-bottom: 30px;
        }

        .logo-box {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            border: 3px solid #45f3ff;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            background: #0b0c10;
        }

        .logo-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .title-box {
            flex-grow: 1;
            padding: 10px 20px;
            border: 2px solid #45f3ff;
            border-radius: 15px;
            background: #0b0c10;
            text-align: center;
        }

        .title-box h1 {
            font-family: 'Cinzel', serif; /* Premium Font */
            font-size: 2rem;
            color: #45f3ff;
            letter-spacing: 2px;
            text-shadow: 0 0 10px rgba(69, 243, 255, 0.5);
        }

        /* Description Box (About Me) */
        .description-box {
            border: 2px solid #45f3ff;
            border-radius: 15px;
            padding: 25px;
            background: #0b0c10;
            margin-bottom: 30px;
            min-height: 120px;
        }

        .description-box h2 {
            font-size: 1.2rem;
            color: #45f3ff;
            margin-bottom: 10px;
            border-bottom: 1px dashed #45f3ff;
            padding-bottom: 5px;
        }

        .description-box p {
            font-size: 0.95rem;
            line-height: 1.6;
            color: #c5a880; /* Elegant soft color */
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
            border-radius: 12px;
            aspect-ratio: 1;
            text-decoration: none;
            color: #ffffff;
            transition: all 0.3s ease;
            font-size: 1.5rem;
        }

        /* Hover & Custom Border Colors based on your image */
        .social-box.youtube { border-color: #ff0000; color: #ff0000; }
        .social-box.instagram { border-color: #e1306c; color: #e1306c; }
        .social-box.tiktok { border-color: #00f2fe; color: #00f2fe; }
        .social-box.telegram { border-color: #0088cc; color: #0088cc; }
        .social-box.discord { border-color: #5865f2; color: #5865f2; }

        .social-box:hover {
            transform: translateY(-5px);
            background: #ffffff;
            color: #0b0c10;
            box-shadow: 0 5px 15px rgba(255, 255, 255, 0.2);
        }

        .social-box span {
            font-size: 0.65rem;
            margin-top: 5px;
            text-transform: uppercase;
            font-weight: 600;
        }

        /* Business Email Box */
        .email-box {
            border: 2px dashed #45f3ff;
            border-radius: 15px;
            padding: 20px;
            background: #0b0c10;
            text-align: center;
            transition: all 0.3s ease;
        }

        .email-box:hover {
            border-style: solid;
            box-shadow: 0 0 15px rgba(69, 243, 255, 0.3);
        }

        .email-box a {
            color: #ffffff;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
        }

        .email-box a:hover {
            color: #45f3ff;
        }

        /* Responsive Design */
        @media (max-width: 480px) {
            .header { flex-direction: column; text-align: center; }
            .social-grid { grid-template-columns: repeat(3, 1fr); }
            .title-box { width: 100%; }
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- Upore logo abong RedRrox name -->
        <div class="header">
            <div class="logo-box">
                <!-- Tomar logo file rrp.jpg ekhane load hobe -->
                <img src="rrp.jpg" alt="RedRrox Logo">
            </div>
            <div class="title-box">
                <h1>RedRrox</h1>
            </div>
        </div>

        <!-- Boro Description Box -->
        <div class="description-box">
            <h2>About ME :)</h2>
            <!-- Ekhane tumi je discription dibe seta bosiye nio -->
            <p>Welcome to my official page! I am a content creator and developer. Write your custom high-quality description here to attract your audience.</p>
        </div>

        <!-- 5ta Social Icons (Horizontal Grid) -->
        <div class="social-grid">
            <a href="YOUR_YOUTUBE_LINK" class="social-box youtube" target="_blank">
                <i class="fab fa-youtube"></i>
                <span>YouTube</span>
            </a>
            <a href="YOUR_INSTAGRAM_LINK" class="social-box instagram" target="_blank">
                <i class="fab fa-instagram"></i>
                <span>Instagram</span>
            </a>
            <a href="YOUR_TIKTOK_LINK" class="social-box tiktok" target="_blank">
                <i class="fab fa-tiktok"></i>
                <span>TikTok</span>
            </a>
            <a href="YOUR_TELEGRAM_LINK" class="social-box telegram" target="_blank">
                <i class="fab fa-telegram"></i>
                <span>Telegram</span>
            </a>
            <a href="YOUR_DISCORD_LINK" class="social-box discord" target="_blank">
                <i class="fab fa-discord"></i>
                <span>Discord</span>
            </a>
        </div>

        <!-- Shobcheye niche Business Email Box -->
        <div class="email-box">
            <a href="mailto:yourbusiness@email.com">
                <i class="fas fa-envelope" style="color: #45f3ff;"></i>
                Business Email: yourbusiness@email.com
            </a>
        </div>
    </div>

</body>
</html>
