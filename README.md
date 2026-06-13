<!DOCTYPE html>
<html lang="mr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no, viewport-fit=cover">
    <title>२६८ - कणकवली विधानसभा संघ | मतदान केंद्रस्तरीय अधिकारी माहिती</title>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <!-- Google Fonts for modern typography -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html, body {
            height: 100%;
            overflow: hidden;
        }

        body {
            font-family: 'Inter', 'Nirmala UI', 'Segoe UI', sans-serif;
            background: #0a0a2a;
            height: 100vh;
            width: 100vw;
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
            overflow: hidden;
        }

        /* Dynamic Gradient Background */
        body::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: radial-gradient(circle at 20% 50%, rgba(102, 126, 234, 0.4), transparent 50%),
                        radial-gradient(circle at 80% 80%, rgba(118, 75, 162, 0.4), transparent 50%),
                        linear-gradient(135deg, #0f0c29 0%, #302b63 50%, #24243e 100%);
            z-index: -2;
        }

        /* Animated Mesh Gradient */
        .mesh-gradient {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at 50% 50%, rgba(255, 255, 255, 0.05) 0%, transparent 60%);
            z-index: -1;
            animation: meshMove 20s ease-in-out infinite alternate;
        }

        @keyframes meshMove {
            0% {
                transform: scale(1) translate(0, 0);
                opacity: 0.3;
            }
            100% {
                transform: scale(1.5) translate(5%, 5%);
                opacity: 0.6;
            }
        }

        /* Floating Particles */
        .particles {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            overflow: hidden;
        }

        .particle {
            position: absolute;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            animation: floatParticle linear infinite;
        }

        @keyframes floatParticle {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 0.5;
            }
            90% {
                opacity: 0.5;
            }
            100% {
                transform: translateY(-100vh) rotate(360deg);
                opacity: 0;
            }
        }

        /* Main Container - Glass Morphism */
        .container {
            position: relative;
            z-index: 2;
            width: 92%;
            max-width: 1350px;
            height: 92vh;
            max-height: 900px;
            background: rgba(15, 12, 41, 0.4);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border-radius: 48px;
            padding: 25px 35px;
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.3),
                        0 0 0 1px rgba(255, 255, 255, 0.15) inset;
            border: 1px solid rgba(255, 255, 255, 0.2);
            animation: containerGlow 4s ease-in-out infinite alternate;
            transition: all 0.3s ease;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        @keyframes containerGlow {
            0% {
                box-shadow: 0 25px 50px rgba(0, 0, 0, 0.3), 0 0 0 1px rgba(255, 255, 255, 0.1) inset;
                border-color: rgba(255, 255, 255, 0.15);
            }
            100% {
                box-shadow: 0 30px 60px rgba(102, 126, 234, 0.2), 0 0 0 2px rgba(255, 255, 255, 0.25) inset;
                border-color: rgba(255, 255, 255, 0.3);
            }
        }

        /* Animated Border */
        .container::before {
            content: '';
            position: absolute;
            top: -2px;
            left: -2px;
            right: -2px;
            bottom: -2px;
            background: linear-gradient(45deg, #667eea, #764ba2, #f093fb, #4facfe);
            border-radius: 50px;
            z-index: -1;
            opacity: 0;
            transition: opacity 0.5s ease;
        }

        .container:hover::before {
            opacity: 0.15;
        }

        /* Header Section */
        .header {
            text-align: center;
            margin-bottom: 12px;
        }

        .floating-icon {
            font-size: 65px;
            color: white;
            margin-bottom: 8px;
            filter: drop-shadow(0 10px 25px rgba(0, 0, 0, 0.4));
            animation: floatIcon 4s ease-in-out infinite;
            display: inline-block;
        }

        @keyframes floatIcon {
            0%, 100% { transform: translateY(0) rotate(0deg); }
            50% { transform: translateY(-12px) rotate(5deg); }
        }

        .header h1 {
            font-size: 44px;
            font-weight: 800;
            background: linear-gradient(135deg, #fff, #c3b8ff, #a8b8ff, #e0c3ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 6px;
            letter-spacing: -0.5px;
            white-space: nowrap;
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
        }

        .header p {
            font-size: 18px;
            color: rgba(255, 255, 255, 0.85);
            font-weight: 500;
            letter-spacing: 3px;
            word-spacing: 8px;
        }

        /* Button Wrapper - Two Buttons Side by Side */
        .button-wrapper {
            display: flex;
            justify-content: center;
            gap: 25px;
            margin: 15px 0 20px 0;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
            padding: 16px 38px;
            border-radius: 60px;
            font-size: 18px;
            font-weight: 600;
            cursor: pointer;
            text-decoration: none;
            position: relative;
            overflow: hidden;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            border: none;
            font-family: inherit;
        }

        .btn-primary {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            box-shadow: 0 10px 25px rgba(102, 126, 234, 0.4);
        }

        .btn-primary:hover {
            transform: translateY(-4px) scale(1.02);
            box-shadow: 0 20px 35px rgba(102, 126, 234, 0.5);
        }

        .btn-secondary {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            box-shadow: 0 10px 25px rgba(240, 147, 251, 0.3);
        }

        .btn-secondary:hover {
            transform: translateY(-4px) scale(1.02);
            box-shadow: 0 20px 35px rgba(240, 147, 251, 0.4);
        }

        .btn i {
            font-size: 20px;
            transition: transform 0.3s ease;
        }

        .btn:hover i {
            transform: translateX(5px);
        }

        .btn-primary:hover i {
            transform: translateX(5px) rotate(360deg);
        }

        .btn-secondary:hover i {
            transform: translateX(-5px) rotate(-360deg);
        }

        .btn-shine {
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
            animation: btnShine 3s infinite;
        }

        @keyframes btnShine {
            to {
                left: 100%;
            }
        }

        /* Stats Grid - Enhanced */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 18px;
            margin-bottom: 18px;
        }

        .stat-card {
            background: rgba(255, 255, 255, 0.08);
            backdrop-filter: blur(10px);
            border-radius: 28px;
            padding: 18px 12px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.15);
            transition: all 0.4s ease;
            animation: fadeInUp 0.6s ease-out both;
            position: relative;
            overflow: hidden;
        }

        .stat-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.1), transparent);
            transition: left 0.5s ease;
        }

        .stat-card:hover::before {
            left: 100%;
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
            transform: translateY(-6px) scale(1.02);
            background: rgba(255, 255, 255, 0.15);
            border-color: rgba(255, 255, 255, 0.3);
        }

        .stat-icon {
            font-size: 38px;
            color: white;
            margin-bottom: 8px;
        }

        .stat-number {
            font-size: 34px;
            font-weight: 800;
            background: linear-gradient(135deg, #fff, #e0c3ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 4px;
        }

        .stat-label {
            font-size: 14px;
            color: rgba(255, 255, 255, 0.9);
            font-weight: 500;
        }

        /* Features Grid */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 14px;
            margin-bottom: 18px;
        }

        .feature-item {
            background: rgba(255, 255, 255, 0.06);
            border-radius: 22px;
            padding: 14px 12px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
            animation: fadeInRight 0.6s ease-out both;
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
            background: linear-gradient(135deg, rgba(102,126,234,0.2), rgba(118,75,162,0.2));
            transform: translateY(-4px);
            border-color: rgba(255,255,255,0.25);
        }

        .feature-icon {
            width: 48px;
            height: 48px;
            background: linear-gradient(135deg, rgba(255,255,255,0.15), rgba(255,255,255,0.05));
            border-radius: 16px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            color: white;
            margin: 0 auto 10px;
            transition: all 0.3s ease;
        }

        .feature-item:hover .feature-icon {
            transform: scale(1.05) rotate(5deg);
            background: linear-gradient(135deg, #667eea, #764ba2);
        }

        .feature-text h4 {
            color: white;
            font-size: 15px;
            font-weight: 600;
            margin-bottom: 4px;
        }

        .feature-text p {
            color: rgba(255, 255, 255, 0.75);
            font-size: 11px;
            font-weight: 400;
        }

        /* Info Cards */
        .info-cards {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 18px;
            margin-bottom: 14px;
        }

        .info-card {
            background: rgba(0, 0, 0, 0.3);
            border-radius: 24px;
            padding: 16px 20px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
            animation: fadeInLeft 0.6s ease-out both;
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
            background: rgba(0, 0, 0, 0.45);
            transform: translateY(-3px);
            border-color: rgba(255,255,255,0.2);
        }

        .info-card h3 {
            color: white;
            font-size: 17px;
            font-weight: 700;
            margin-bottom: 12px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .info-card h3 i {
            font-size: 20px;
            background: linear-gradient(135deg, #667eea, #f093fb);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        .info-card ul {
            list-style: none;
        }

        .info-card ul li {
            color: rgba(255, 255, 255, 0.85);
            font-size: 13px;
            margin-bottom: 8px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .info-card ul li i {
            color: #4facfe;
            font-size: 12px;
        }

        /* Footer */
        .footer {
            text-align: center;
            padding-top: 12px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }

        .footer p {
            color: rgba(255, 255, 255, 0.65);
            font-size: 13px;
            font-weight: 500;
        }

        .footer i.fa-heart {
            color: #ff6b6b;
            animation: heartbeat 1.4s ease infinite;
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
            gap: 20px;
            margin-top: 8px;
        }

        .footer-links a {
            color: rgba(255, 255, 255, 0.55);
            text-decoration: none;
            font-size: 12px;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
            gap: 5px;
        }

        .footer-links a:hover {
            color: white;
            transform: translateY(-2px);
        }

        /* Responsive */
        @media (max-width: 1100px) {
            .container { padding: 20px 25px; }
            .header h1 { font-size: 36px; white-space: normal; line-height: 1.2; }
            .stat-number { font-size: 28px; }
            .btn { padding: 14px 28px; font-size: 16px; }
        }

        @media (max-height: 800px) {
            .container { padding: 18px 25px; }
            .floating-icon { font-size: 50px; }
            .header h1 { font-size: 34px; }
            .stat-card { padding: 12px; }
            .stat-icon { font-size: 30px; }
            .stat-number { font-size: 26px; }
            .feature-item { padding: 10px; }
            .info-card { padding: 12px 16px; }
        }

        /* Landscape orientation warning for mobile */
        @media (orientation: portrait) and (max-width: 768px) {
            .container {
                display: none;
            }
            body::after {
                content: "📱 कृपया फोन आडवा (Landscape mode) करा | Please rotate your phone to landscape";
                position: fixed;
                top: 0;
                left: 0;
                width: 100%;
                height: 100%;
                background: linear-gradient(135deg, #0f0c29, #302b63);
                color: white;
                display: flex;
                align-items: center;
                justify-content: center;
                font-size: 20px;
                text-align: center;
                padding: 30px;
                z-index: 9999;
                font-family: 'Inter', sans-serif;
                font-weight: 500;
            }
        }

        /* Loading animation for buttons */
        .btn.loading {
            pointer-events: none;
            opacity: 0.7;
        }

        .btn.loading i.fa-spinner {
            animation: spin 1s linear infinite;
        }

        @keyframes spin {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
    </style>
</head>
<body>
    <div class="mesh-gradient"></div>
    <div class="particles" id="particles"></div>

    <div class="container">
        <!-- Header -->
        <div class="header">
            <div class="floating-icon">
                <i class="fas fa-vote-yea"></i>
            </div>
            <h1>२६८ - कणकवली विधानसभा संघ</h1>
            <p>मतदान केंद्रस्तरीय अधिकारी माहिती | देवगड • कणकवली • वैभववाडी</p>
        </div>

        <!-- Two Buttons Side by Side - BOTH have SAME LINK now -->
        <div class="button-wrapper">
            <a href="https://script.google.com/macros/s/AKfycbwV--g5jhc4lmgPFoPtrHysjtzNuLajIhgp96yvg6kdiMUnN5xcjYKUoCPmLfA41CO7/exec" 
               class="btn btn-primary" 
               target="_self"
               id="bloBtn">
                <i class="fas fa-users"></i>
                BLO यादी पहा
                <i class="fas fa-arrow-right"></i>
                <span class="btn-shine"></span>
            </a>
            <a href="https://script.google.com/macros/s/AKfycbxZmK6dtzixWpb7Qqh6n5byXFDxWuVVcWEmLmEIo_BS91ntuECGTvLWY-2cEf6d3enC/exec" 
               class="btn btn-secondary" 
               target="_self"
               id="newBtn">
                <i class="fas fa-chart-line"></i>
                2.0
                <i class="fas fa-chart-simple"></i>
                <span class="btn-shine"></span>
            </a>
        </div>

        <!-- Stats Grid -->
        <div class="stats-grid">
            <div class="stat-card">
                <div class="stat-icon"><i class="fas fa-map-marker-alt"></i></div>
                <div class="stat-number">१००+</div>
                <div class="stat-label">मतदान केंद्रे</div>
            </div>
            <div class="stat-card">
                <div class="stat-icon"><i class="fas fa-user-tie"></i></div>
                <div class="stat-number">२००+</div>
                <div class="stat-label">अधिकारी</div>
            </div>
            <div class="stat-card">
                <div class="stat-icon"><i class="fas fa-charging-station"></i></div>
                <div class="stat-number">२४/७</div>
                <div class="stat-label">उपलब्धता</div>
            </div>
        </div>

        <!-- Features Grid -->
        <div class="features-grid">
            <div class="feature-item">
                <div class="feature-icon"><i class="fas fa-language"></i></div>
                <div class="feature-text">
                    <h4>द्विभाषिक शोध</h4>
                    <p>इंग्रजी / मराठी</p>
                </div>
            </div>
            <div class="feature-item">
                <div class="feature-icon"><i class="fas fa-history"></i></div>
                <div class="feature-text">
                    <h4>बदल इतिहास</h4>
                    <p>सर्व अपडेटची नोंद</p>
                </div>
            </div>
            <div class="feature-item">
                <div class="feature-icon"><i class="fas fa-shield-alt"></i></div>
                <div class="feature-text">
                    <h4>पासवर्ड संरक्षण</h4>
                    <p>सुरक्षित अपडेट</p>
                </div>
            </div>
            <div class="feature-item">
                <div class="feature-icon"><i class="fas fa-mobile-alt"></i></div>
                <div class="feature-text">
                    <h4>मोबाईल फ्रेंडली</h4>
                    <p>सर्व डिव्हाइसवर</p>
                </div>
            </div>
        </div>

        <!-- Info Cards -->
        <div class="info-cards">
            <div class="info-card">
                <h3><i class="fas fa-star-of-life"></i> प्रमुख वैशिष्ट्ये</h3>
                <ul>
                    <li><i class="fas fa-check-circle"></i> केंद्र क्रमांकाने / नावाने शोधा</li>
                    <li><i class="fas fa-check-circle"></i> अधिकारी माहिती त्वरित अपडेट</li>
                    <li><i class="fas fa-check-circle"></i> संपूर्ण बदल इतिहास</li>
                    <li><i class="fas fa-check-circle"></i> स्वयंचलित बॅकअप प्रणाली</li>
                </ul>
            </div>
            <div class="info-card">
                <h3><i class="fas fa-shield-virus"></i> सुरक्षा वैशिष्ट्ये</h3>
                <ul>
                    <li><i class="fas fa-lock"></i> पासवर्ड प्रोटेक्शन</li>
                    <li><i class="fas fa-user-check"></i> कोणी केले अपडेट ओळखा</li>
                    <li><i class="fas fa-database"></i> एन्क्रिप्टेड डेटा</li>
                    <li><i class="fas fa-clock"></i> टाइमस्टॅम्पसह लॉग</li>
                </ul>
            </div>
        </div>

        <!-- Footer -->
        <div class="footer">
            <p>
                <i class="fas fa-heart"></i> 
                विकसित: मतदान केंद्र माहिती प्रणाली 
                <i class="fas fa-copyright"></i> 2025
            </p>
            <div class="footer-links">
                <a href="#"><i class="fas fa-info-circle"></i> मदत</a>
                <a href="#"><i class="fas fa-user-shield"></i> गोपनीयता</a>
                <a href="#"><i class="fas fa-headset"></i> संपर्क</a>
            </div>
        </div>
    </div>

    <script>
        // Generate floating particles
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 50;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                const size = Math.random() * 8 + 2;
                particle.style.width = size + 'px';
                particle.style.height = size + 'px';
                particle.style.left = Math.random() * 100 + '%';
                particle.style.animationDuration = Math.random() * 15 + 8 + 's';
                particle.style.animationDelay = Math.random() * 10 + 's';
                particle.style.opacity = Math.random() * 0.4 + 0.1;
                particlesContainer.appendChild(particle);
            }
        }
        
        createParticles();

        // Add loading effect to both buttons
        const bloBtn = document.getElementById('bloBtn');
        const newBtn = document.getElementById('newBtn');

        function addLoadingEffect(btn) {
            btn.addEventListener('click', function(e) {
                if (this.classList.contains('loading')) return;
                this.classList.add('loading');
                const originalText = this.innerHTML;
                this.innerHTML = '<i class="fas fa-spinner fa-spin"></i> लोड करत आहे... <i class="fas fa-hourglass-half"></i>';
                
                setTimeout(() => {
                    // Don't remove loading - let the page navigate
                    // The page will navigate to the link
                }, 500);
            });
        }

        addLoadingEffect(bloBtn);
        addLoadingEffect(newBtn);
    </script>
</body>
</html>
