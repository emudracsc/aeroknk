<!DOCTYPE html>
<html lang="mr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>मतदान केंद्र माहिती प्रणाली</title>
    
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Nirmala UI', 'Segoe UI', 'Arial', sans-serif;
            background: #0f0c29;
            background: linear-gradient(135deg, #0f0c29 0%, #302b63 50%, #24243e 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
            position: relative;
            overflow-x: hidden;
        }

        /* Animated Background */
        .circles {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: 0;
        }

        .circles li {
            position: absolute;
            display: block;
            list-style: none;
            width: 20px;
            height: 20px;
            background: rgba(255, 255, 255, 0.05);
            animation: animate 25s linear infinite;
            bottom: -150px;
            border-radius: 50%;
        }

        .circles li:nth-child(1) {
            left: 25%;
            width: 80px;
            height: 80px;
            animation-delay: 0s;
            background: rgba(255, 255, 255, 0.02);
        }

        .circles li:nth-child(2) {
            left: 10%;
            width: 20px;
            height: 20px;
            animation-delay: 2s;
            animation-duration: 12s;
            background: rgba(255, 255, 255, 0.03);
        }

        .circles li:nth-child(3) {
            left: 70%;
            width: 20px;
            height: 20px;
            animation-delay: 4s;
            background: rgba(255, 255, 255, 0.02);
        }

        .circles li:nth-child(4) {
            left: 40%;
            width: 60px;
            height: 60px;
            animation-delay: 0s;
            animation-duration: 18s;
            background: rgba(255, 255, 255, 0.03);
        }

        .circles li:nth-child(5) {
            left: 65%;
            width: 20px;
            height: 20px;
            animation-delay: 0s;
            background: rgba(255, 255, 255, 0.02);
        }

        .circles li:nth-child(6) {
            left: 75%;
            width: 110px;
            height: 110px;
            animation-delay: 3s;
            background: rgba(255, 255, 255, 0.02);
        }

        .circles li:nth-child(7) {
            left: 35%;
            width: 150px;
            height: 150px;
            animation-delay: 7s;
            background: rgba(255, 255, 255, 0.02);
        }

        .circles li:nth-child(8) {
            left: 50%;
            width: 25px;
            height: 25px;
            animation-delay: 15s;
            animation-duration: 45s;
            background: rgba(255, 255, 255, 0.03);
        }

        .circles li:nth-child(9) {
            left: 20%;
            width: 15px;
            height: 15px;
            animation-delay: 2s;
            animation-duration: 35s;
            background: rgba(255, 255, 255, 0.02);
        }

        .circles li:nth-child(10) {
            left: 85%;
            width: 150px;
            height: 150px;
            animation-delay: 0s;
            animation-duration: 11s;
            background: rgba(255, 255, 255, 0.02);
        }

        @keyframes animate {
            0% {
                transform: translateY(0) rotate(0deg);
                opacity: 1;
                border-radius: 50%;
            }

            100% {
                transform: translateY(-1000px) rotate(720deg);
                opacity: 0;
                border-radius: 50%;
            }
        }

        /* Floating Particles */
        .particles {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 0;
            background: radial-gradient(circle at 50% 50%, rgba(255,255,255,0.1) 0%, transparent 50%);
            animation: pulse 4s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% { opacity: 0.5; }
            50% { opacity: 1; }
        }

        /* Main Container */
        .container {
            position: relative;
            z-index: 1;
            max-width: 1100px;
            width: 100%;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border-radius: 40px;
            padding: 60px;
            box-shadow: 0 25px 45px rgba(0, 0, 0, 0.2),
                        0 0 0 2px rgba(255, 255, 255, 0.1) inset;
            animation: slideInUp 1s ease-out;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        @keyframes slideInUp {
            from {
                transform: translateY(100px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }

        /* Header Section */
        .header {
            text-align: center;
            margin-bottom: 50px;
        }

        .floating-icon {
            font-size: 100px;
            color: white;
            margin-bottom: 25px;
            filter: drop-shadow(0 10px 20px rgba(0, 0, 0, 0.3));
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-15px); }
        }

        /* Main Heading */
        .header h1 {
            font-size: 64px;
            font-weight: 700;
            background: linear-gradient(135deg, #fff, #a8b8ff, #c3a8ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 20px;
            text-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            letter-spacing: 1px;
            white-space: nowrap;
            line-height: 1.3;
        }

        .header p {
            font-size: 24px;
            color: rgba(255, 255, 255, 0.9);
            font-weight: 400;
            letter-spacing: 2px;
        }

        /* Main Button */
        .button-wrapper {
            text-align: center;
            margin: 40px 0 50px 0;
            position: relative;
        }

        .launch-btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 20px;
            background: linear-gradient(135deg, #667eea, #764ba2, #9f7aea);
            background-size: 200% 200%;
            color: white;
            border: none;
            padding: 30px 70px;
            border-radius: 70px;
            font-size: 28px;
            font-weight: 600;
            cursor: pointer;
            text-decoration: none;
            transition: all 0.4s ease;
            box-shadow: 0 20px 40px rgba(102, 126, 234, 0.4),
                        0 0 0 2px rgba(255, 255, 255, 0.2) inset;
            border: 1px solid rgba(255, 255, 255, 0.3);
            animation: gradientBG 3s ease infinite;
            position: relative;
            overflow: hidden;
        }

        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .launch-btn:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 30px 60px rgba(102, 126, 234, 0.6),
                        0 0 0 3px rgba(255, 255, 255, 0.3) inset;
        }

        .launch-btn:active {
            transform: translateY(0) scale(1);
        }

        .launch-btn i {
            font-size: 32px;
            transition: transform 0.3s ease;
        }

        .launch-btn:hover i {
            transform: rotate(360deg) scale(1.2);
        }

        .btn-shine {
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
            animation: shine 3s infinite;
        }

        @keyframes shine {
            to {
                left: 100%;
            }
        }

        /* Stats Grid */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
            margin-bottom: 50px;
        }

        .stat-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(5px);
            -webkit-backdrop-filter: blur(5px);
            border-radius: 30px;
            padding: 35px 25px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: all 0.4s ease;
            animation: fadeInUp 0.8s ease-out;
            animation-fill-mode: both;
        }

        .stat-card:nth-child(1) { animation-delay: 0.1s; }
        .stat-card:nth-child(2) { animation-delay: 0.2s; }
        .stat-card:nth-child(3) { animation-delay: 0.3s; }

        @keyframes fadeInUp {
            from {
                transform: translateY(30px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }

        .stat-card:hover {
            transform: translateY(-10px) scale(1.05);
            background: rgba(255, 255, 255, 0.2);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
        }

        .stat-icon {
            font-size: 50px;
            color: white;
            margin-bottom: 20px;
            filter: drop-shadow(0 5px 10px rgba(0, 0, 0, 0.3));
        }

        .stat-number {
            font-size: 44px;
            font-weight: 700;
            color: white;
            margin-bottom: 10px;
            text-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }

        .stat-label {
            font-size: 18px;
            color: rgba(255, 255, 255, 0.9);
            font-weight: 400;
            letter-spacing: 1px;
        }

        /* Features Grid */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 25px;
            margin-bottom: 50px;
        }

        .feature-item {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 25px;
            padding: 25px;
            display: flex;
            align-items: center;
            gap: 20px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
            animation: fadeInRight 0.8s ease-out;
            animation-fill-mode: both;
        }

        .feature-item:nth-child(1) { animation-delay: 0.4s; }
        .feature-item:nth-child(2) { animation-delay: 0.5s; }
        .feature-item:nth-child(3) { animation-delay: 0.6s; }
        .feature-item:nth-child(4) { animation-delay: 0.7s; }

        @keyframes fadeInRight {
            from {
                transform: translateX(30px);
                opacity: 0;
            }
            to {
                transform: translateX(0);
                opacity: 1;
            }
        }

        .feature-item:hover {
            background: rgba(255, 255, 255, 0.15);
            transform: translateX(10px);
            border-color: rgba(255, 255, 255, 0.3);
        }

        .feature-icon {
            width: 70px;
            height: 70px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 32px;
            color: white;
        }

        .feature-text h4 {
            color: white;
            font-size: 20px;
            font-weight: 600;
            margin-bottom: 8px;
        }

        .feature-text p {
            color: rgba(255, 255, 255, 0.8);
            font-size: 16px;
            font-weight: 400;
        }

        /* Info Cards */
        .info-cards {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 25px;
            margin-top: 30px;
        }

        .info-card {
            background: rgba(0, 0, 0, 0.2);
            border-radius: 25px;
            padding: 30px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
            animation: fadeInLeft 0.8s ease-out;
            animation-fill-mode: both;
        }

        .info-card:nth-child(1) { animation-delay: 0.8s; }
        .info-card:nth-child(2) { animation-delay: 0.9s; }

        @keyframes fadeInLeft {
            from {
                transform: translateX(-30px);
                opacity: 0;
            }
            to {
                transform: translateX(0);
                opacity: 1;
            }
        }

        .info-card:hover {
            background: rgba(0, 0, 0, 0.3);
            transform: translateY(-5px);
            border-color: rgba(255, 255, 255, 0.2);
        }

        .info-card h3 {
            color: white;
            font-size: 24px;
            font-weight: 600;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .info-card h3 i {
            color: #667eea;
            font-size: 28px;
        }

        .info-card ul {
            list-style: none;
        }

        .info-card ul li {
            color: rgba(255, 255, 255, 0.9);
            font-size: 18px;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .info-card ul li i {
            color: #28a745;
            font-size: 16px;
        }

        /* Footer */
        .footer {
            text-align: center;
            margin-top: 60px;
            padding-top: 35px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }

        .footer p {
            color: rgba(255, 255, 255, 0.7);
            font-size: 18px;
            font-weight: 400;
        }

        .footer i {
            color: #e73c7e;
            animation: heartbeat 1.5s ease infinite;
        }

        @keyframes heartbeat {
            0%, 100% { transform: scale(1); }
            25% { transform: scale(1.2); }
            50% { transform: scale(1); }
            75% { transform: scale(1.2); }
        }

        .footer-links {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 20px;
        }

        .footer-links a {
            color: rgba(255, 255, 255, 0.6);
            text-decoration: none;
            font-size: 16px;
            transition: color 0.3s ease;
        }

        .footer-links a:hover {
            color: white;
        }

        /* Responsive Design */
        @media (max-width: 992px) {
            .container { padding: 40px; }
            .header h1 { font-size: 52px; }
            .header p { font-size: 20px; }
            .launch-btn { padding: 25px 50px; font-size: 24px; }
            .stat-number { font-size: 36px; }
            .stat-label { font-size: 16px; }
        }

        @media (max-width: 768px) {
            .container { padding: 30px; }
            .header h1 { 
                font-size: 44px;
                white-space: normal;
            }
            .header p { font-size: 18px; }
            .stats-grid { grid-template-columns: 1fr; }
            .features-grid { grid-template-columns: 1fr; }
            .info-cards { grid-template-columns: 1fr; }
            .launch-btn { 
                padding: 20px 40px; 
                font-size: 22px;
                width: 100%;
            }
        }

        @media (max-width: 480px) {
            .header h1 { font-size: 36px; }
            .header p { font-size: 16px; }
            .stat-number { font-size: 32px; }
            .stat-label { font-size: 14px; }
            .feature-text h4 { font-size: 18px; }
            .feature-text p { font-size: 14px; }
            .info-card h3 { font-size: 20px; }
            .info-card ul li { font-size: 16px; }
        }
    </style>
</head>
<body>
    <!-- Animated Background Circles -->
    <ul class="circles">
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
    </ul>

    <!-- Floating Particles -->
    <div class="particles"></div>

    <!-- Main Container -->
    <div class="container">
        <!-- Header -->
        <div class="header">
            <div class="floating-icon">
                <i class="fas fa-vote-yea"></i>
            </div>
            <h1>मतदान केंद्र माहिती प्रणाली</h1>
            <p>सोपी | सुरक्षित | जलद</p>
        </div>

        <!-- Main Button -->
        <div class="button-wrapper">
            <a href="https://script.google.com/macros/s/AKfycbwV--g5jhc4lmgPFoPtrHysjtzNuLajIhgp96yvg6kdiMUnN5xcjYKUoCPmLfA41CO7/exec" 
               class="launch-btn" 
               target="_self">
                <i class="fas fa-rocket"></i>
                प्रणाली सुरू करा
                <i class="fas fa-arrow-right"></i>
                <span class="btn-shine"></span>
            </a>
        </div>

        <!-- Stats Grid -->
        <div class="stats-grid">
            <div class="stat-card">
                <div class="stat-icon">
                    <i class="fas fa-building"></i>
                </div>
                <div class="stat-number">100+</div>
                <div class="stat-label">मतदान केंद्रे</div>
            </div>
            <div class="stat-card">
                <div class="stat-icon">
                    <i class="fas fa-users"></i>
                </div>
                <div class="stat-number">200+</div>
                <div class="stat-label">अधिकारी</div>
            </div>
            <div class="stat-card">
                <div class="stat-icon">
                    <i class="fas fa-clock"></i>
                </div>
                <div class="stat-number">24/7</div>
                <div class="stat-label">उपलब्ध</div>
            </div>
        </div>

        <!-- Features Grid -->
        <div class="features-grid">
            <div class="feature-item">
                <div class="feature-icon">
                    <i class="fas fa-search"></i>
                </div>
                <div class="feature-text">
                    <h4>द्विभाषिक शोध</h4>
                    <p>इंग्रजी / मराठी दोन्हीमध्ये शोधा</p>
                </div>
            </div>
            <div class="feature-item">
                <div class="feature-icon">
                    <i class="fas fa-history"></i>
                </div>
                <div class="feature-text">
                    <h4>बदल इतिहास</h4>
                    <p>सर्व अपडेटची नोंद ठेवली जाते</p>
                </div>
            </div>
            <div class="feature-item">
                <div class="feature-icon">
                    <i class="fas fa-lock"></i>
                </div>
                <div class="feature-text">
                    <h4>पासवर्ड संरक्षण</h4>
                    <p>फक्त अधिकृत व्यक्ती अपडेट करू शकतात</p>
                </div>
            </div>
            <div class="feature-item">
                <div class="feature-icon">
                    <i class="fas fa-mobile-alt"></i>
                </div>
                <div class="feature-text">
                    <h4>मोबाईल फ्रेंडली</h4>
                    <p>कोणत्याही डिव्हाइसवर वापरा</p>
                </div>
            </div>
        </div>

        <!-- Info Cards -->
        <div class="info-cards">
            <div class="info-card">
                <h3><i class="fas fa-star"></i> प्रमुख वैशिष्ट्ये</h3>
                <ul>
                    <li><i class="fas fa-check-circle"></i> केंद्र क्रमांकाने शोधा</li>
                    <li><i class="fas fa-check-circle"></i> नावाने शोधा (इंग्रजी/मराठी)</li>
                    <li><i class="fas fa-check-circle"></i> अधिकारी अपडेट करा</li>
                    <li><i class="fas fa-check-circle"></i> संपूर्ण इतिहास पहा</li>
                    <li><i class="fas fa-check-circle"></i> बॅकअप सिस्टीम</li>
                </ul>
            </div>
            <div class="info-card">
                <h3><i class="fas fa-shield-alt"></i> सुरक्षा वैशिष्ट्ये</h3>
                <ul>
                    <li><i class="fas fa-check-circle"></i> पासवर्ड प्रोटेक्शन</li>
                    <li><i class="fas fa-check-circle"></i> प्रत्येक बदलाची नोंद</li>
                    <li><i class="fas fa-check-circle"></i> कोणी अपडेट केले ते कळेल</li>
                    <li><i class="fas fa-check-circle"></i> डेटा बॅकअप</li>
                    <li><i class="fas fa-check-circle"></i> सुरक्षित प्रवेश</li>
                </ul>
            </div>
        </div>

        <!-- Footer -->
        <div class="footer">
            <p>
                <i class="fas fa-heart"></i> 
                विकसित: मतदान केंद्र माहिती प्रणाली 
                <i class="fas fa-copyright"></i> 2024
            </p>
            <div class="footer-links">
                <a href="#"><i class="fas fa-info-circle"></i> मदत</a>
                <a href="#"><i class="fas fa-lock"></i> गोपनीयता</a>
                <a href="#"><i class="fas fa-envelope"></i> संपर्क</a>
            </div>
        </div>
    </div>
</body>
</html>
