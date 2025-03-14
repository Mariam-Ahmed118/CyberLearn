<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CyberLearn</title>
    <style>
        /* General Styles */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            /* Modern font */
            margin: 0;
            padding: 0;
            overflow-x: hidden;
            background-color: #f0f8ff;
            /* Light, calming background */
            background-image: url('bc.JPG');
        }

        /* Home Screen Styles */
        .home-screen {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #1557B0, #29abe2);
            color: white;
            text-align: center;
            padding: 20px;
            overflow: hidden;
            position: relative;
            /* For the animated background */
        }

        #Egypt digital efforts {
            padding: 20px;
            background-color: #f9f9f9;
            border-radius: 8px;
            margin-top: 20px;
        }

        #Egypt digital efforts h2 {
            color: #1557B0;
            font-size: 24px;
            margin-bottom: 15px;
        }

        #Egypt digital efforts h3 {
            color: #29abe2;
            font-size: 20px;
            margin-top: 20px;
            margin-bottom: 10px;
        }

        #Egypt digital efforts p {
            font-size: 16px;
            color: #555;
            line-height: 1.6;
        }

        .video-container {
            margin-top: 20px;
            margin-bottom: 20px;
        }

        /* Animated Background */
        .home-screen::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('path/to/your/cyber-pattern.png');
            /* Replace with a subtle cyber pattern */
            opacity: 0.15;
            animation: moveBackground 40s linear infinite;
            z-index: 0;
        }

        @keyframes moveBackground {
            from {
                background-position: 0 0;
            }

            to {
                background-position: 100% 100%;
            }
        }

        .home-content {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
            /* Ensure content is above the background */
            z-index: 1;
        }

        .home-title {
            font-size: 4rem;
            /* Increased size */
            font-weight: 700;
            /* Stronger weight */
            color: #d6e4ee;
            margin-bottom: 25px;
            animation: fadeInDown 1s ease-out forwards;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
            /* Subtle shadow */
            animation-fill-mode: forwards !important;
            /* Keep the animation result */
            opacity: 1 !important;
            /* Ensure it's visible */
            transform: translateY(0) !important;
            /* Ensure it's in the final position */
        }

        .highlight {
            color: #f6d365;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        .home-subtitle {
            font-size: 1.75rem;
            /* Increased size */
            margin-bottom: 30px;
            /* Reduced margin to bring button closer */
            animation: fadeInUp 1s ease-out 0.5s;
            opacity: 0;
            animation-fill-mode: forwards;
            line-height: 1.6;
            /* Improved readability */
        }

        .home-animation {
            display: flex;
            justify-content: center;
            align-items: center;
            margin-bottom: 30px;
            /* Reduced margin to bring button closer */
        }

        .emoji-animation {
            font-size: 4rem;
            /* Increased size */
            animation: float 3s ease-in-out infinite;
        }

        .cyber-animation {
            display: flex;
            gap: 25px;
            margin-left: 25px;
        }

        .cyber-animation div {
            font-size: 3rem;
            /* Increased size */
            animation: bounce 2s ease-in-out infinite;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.1);
        }

        .cyber-animation div:nth-child(1) {
            animation-delay: 0s;
        }

        .cyber-animation div:nth-child(2) {
            animation-delay: 0.5s;
        }

        .cyber-animation div:nth-child(3) {
            animation-delay: 1s;
        }

        .cta-button {
            background-color: #f6d365;
            color: #1557B0;
            padding: 18px 45px;
            /* Increased padding */
            border: none;
            border-radius: 50px;
            font-size: 1.3rem;
            /* Increased size */
            font-weight: 600;
            /* Slightly lighter weight */
            cursor: pointer;
            transition: all 0.3s ease;
            animation: fadeInUp 1s ease-out 1s;
            opacity: 0;
            animation-fill-mode: forwards;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            /* Added shadow */
        }

        .cta-button:hover {
            background-color: #ffcc00;
            transform: scale(1.07);
            /* Slightly more pronounced scale */
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.3);
            /* Enhanced shadow */
        }

        /* Animations */
        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-60px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(60px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes float {
            0%,
            100% {
                transform: translateY(0);
            }

            50% {
                transform: translateY(-25px);
            }
        }

        @keyframes bounce {
            0%,
            100% {
                transform: translateY(0);
            }

            50% {
                transform: translateY(-20px);
            }
        }

        /* Existing Styles (Moved to bottom for organization) */
        .nav-bar {
            width: 100%;
            background-color: #1557B0;
            padding: 15px 0;
            position: fixed;
            top: 0;
            left: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease-in-out;
            display: none;
            /* Initially hidden */
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 20px;
        }

        .nav-logo {
            color: white;
            font-size: 24px;
            font-weight: bold;
            text-decoration: none;
            margin-right: 50px;
            /* Add margin to push it to the left */
        }

        .nav-menu {
            display: flex;
            gap: 20px;
        }

        .nav-item {
            color: white;
            text-decoration: none;
            padding: 8px 15px;
            border-radius: 5px;
            transition: background-color 0.3s, transform 0.2s ease-in-out;
        }

        .nav-item:hover {
            background-color: rgba(255, 255, 255, 0.1);
            transform: scale(1.05);
        }

        .user-profile {
            display: flex;
            align-items: center;
            gap: 10px;
            color: white;
            cursor: pointer;
            transition: transform 0.2s ease-in-out;
        }

        .user-profile:hover {
            transform: scale(1.05);
        }

        .profile-img {
            width: 35px;
            height: 35px;
            border-radius: 50%;
            background-color: #fff;
            cursor: pointer;
        }

        .dashboard {
            max-width: 800px;
            margin: 100px auto 50px;
            padding: 20px;
            background: #fff;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
            opacity: 0;
            transform: translateY(20px);
            animation: fadeIn 0.5s ease-out forwards 0.2s;
            display: none;
            /* Initially hidden */
        }

        @keyframes fadeIn {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .back-button {
            background-color: #c45637;
            color: white;
            padding: 20px 40px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            font-size: 24px;
            font-weight: bold;
            transition: all 0.3s ease;
            margin-bottom: 50px;
            width: 300px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .back-button:hover {
            background-color: #1557B0;
            transform: scale(1.05);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
        }

        h1 {
            text-align: center;
            color: #1557B0;
            opacity: 0;
            transform: translateY(-10px);
            animation: slideIn 0.5s ease-out forwards 0.3s;
        }

        @keyframes slideIn {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .progress-bar {
            width: 100%;
            background-color: #e0e0e0;
            border-radius: 5px;
            margin-bottom: 20px;
            overflow: hidden;
        }

        .progress {
            height: 20px;
            background-color: #1557B0;
            border-radius: 5px;
            width: 0%;
            transition: width 0.6s ease-in-out;
        }

        .levels .level {
            margin-bottom: 20px;
            padding: 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            background: #f9f9f9;
            transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
        }

        .levels .level:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .levels .level.locked {
            opacity: 0.5;
        }

        .levels .level h2 {
            margin-top: 0;
        }

        .levels .level button {
            padding: 10px 20px;
            background: #007bff;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .levels .level button:hover {
            background-color: #0056b3;
        }

        .levels .level button:disabled {
            background: #ccc;
            cursor: not-allowed;
        }

        .content {
            display: none;
            margin-top: 20px;
        }

        .content.active {
            display: block;
            animation: slideInContent 0.3s ease-out forwards;
        }

        @keyframes slideInContent {
            from {
                opacity: 0;
                transform: translateY(10px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .quiz {
            margin-top: 20px;
        }

        .quiz p {
            font-weight: bold;
        }

        .quiz input[type="radio"] {
            margin-right: 10px;
        }

        .quiz button {
            margin-top: 10px;
            padding: 10px 20px;
            background: #28a745;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .quiz button:hover {
            background-color: #1e7e34;
        }

        .tab-container {
            width: 100%;
            margin-top: 20px;
        }

        .tab-nav {
            display: flex;
            border-bottom: 2px solid #e6e6e6;
            margin-bottom: 20px;
        }

        .tab-button {
            padding: 15px 30px;
            border: none;
            background: none;
            font-size: 16px;
            font-weight: 500;
            color: #666;
            cursor: pointer;
            position: relative;
            transition: all 0.3s ease;
        }

        .tab-button:hover {
            color: #1557B0;
        }

        .tab-button.active {
            color: #1557B0;
        }

        .tab-button.active::after {
            content: '';
            position: absolute;
            bottom: -2px;
            left: 0;
            width: 100%;
            height: 2px;
            background-color: #1557B0;
        }

        .tab-content {
            display: none;
            padding: 20px;
        }

        .tab-content.active {
            display: block;
            animation: fadeIn 0.3s ease-out forwards;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .stat-box {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
        }

        .stat-box:hover {
            transform: scale(1.03);
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        .stat-number {
            font-size: 24px;
            font-weight: bold;
            color: #1557B0;
        }

        .resource-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .resource-card {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
        }

        .resource-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        .resource-link {
            display: inline-block;
            padding: 8px 20px;
            background: #1557B0;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            margin-top: 10px;
            transition: background-color 0.3s ease;
        }

        .resource-link:hover {
            background: #c45637;
        }

        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 1001;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
        }

        .modal-content {
            background-color: #fefefe;
            margin: 15% auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
            max-width: 500px;
            border-radius: 8px;
            position: relative;
            animation: slideInModal 0.4s ease-out forwards;
        }

        @keyframes slideInModal {
            from {
                opacity: 0;
                transform: translateY(-50px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .close {
            position: absolute;
            right: 20px;
            top: 10px;
            color: #aaa;
            font-size: 28px;
            font-weight: bold;
            cursor: pointer;
        }

        .close:hover {
            color: black;
        }

        .form-group {
            margin-bottom: 15px;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
        }

        .form-group input {
            width: 100%;
            padding: 8px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }

        .btn-primary {
            background-color: #1557B0;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            width: 100%;
            margin-top: 10px;
            transition: background-color 0.3s ease;
        }

        .btn-primary:hover {
            background-color: #1246a0;
        }

        /* Dropdown Styles */
        .dropdown {
            display: none;
            position: absolute;
            right: 20px;
            top: 60px;
            background-color: white;
            min-width: 160px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
            border-radius: 4px;
            z-index: 1000;
            animation: slideInDropdown 0.3s ease-out forwards;
        }

        @keyframes slideInDropdown {
            from {
                opacity: 0;
                transform: translateY(-10px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .dropdown-content {
            padding: 10px 0;
        }

        .dropdown-content a {
            color: #333;
            padding: 12px 16px;
            text-decoration: none;
            display: block;
            transition: background-color 0.2s ease;
        }

        .dropdown-content a:hover {
            background-color: #f1f1f1;
        }

        .quiz-result {
            margin-top: 20px;
            font-weight: bold;
            opacity: 0;
            animation: fadeIn 0.5s ease-out forwards;
        }

        /* Congratulations Screen Styles */
        #congratulationsScreen {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.9);
            z-index: 1000;
            overflow: auto;
        }

        #congratulationsScreen>div {
            position: relative;
            background: white;
            max-width: 600px;
            margin: 50px auto;
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            animation: slideInCongratulations 0.5s ease-out forwards;
        }

        @keyframes slideInCongratulations {
            from {
                opacity: 0;
                transform: translateY(-50px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        #certificate {
            display: none;
            border: 5px solid #1557B0;
            margin: 20px auto;
            padding: 40px;
            background: #f9f9f9;
            animation: fadeIn 0.5s ease-out forwards;
        }

        /* New Styles for Progress Tab */
        .progress-tab-content {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .points-display {
            font-size: 2em;
            font-weight: bold;
            color: #28a745;
            margin-bottom: 20px;
        }

        .level-progress-list {
            list-style: none;
            padding: 0;
            width: 100%;
            max-width: 600px;
        }

        .level-progress-item {
            background-color: #f8f9fa;
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 15px;
            margin-bottom: 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .level-name {
            font-weight: bold;
        }

        .level-status {
            color: #555;
        }

        .completed {
            color: green;
        }

        /* Congratulations Animation */
        .congrats-animation {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1001;
        }

        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            background-color: #f06;
            border-radius: 50%;
            animation: confettiFall 2s linear infinite;
            /* Corrected animation */
        }

        @keyframes confettiFall {
            0% {
                transform: translateY(0) rotate(0deg);
                opacity: 1;
            }

            100% {
                transform: translateY(100vh) rotate(360deg);
                opacity: 0;
            }
        }

        /* Download Button Style */
        #downloadCertificateBtn {
            background-color: #28a745;
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 8px;
            font-size: 18px;
            cursor: pointer;
            transition: background-color 0.3s ease;
            margin-top: 20px;
        }

        #downloadCertificateBtn:hover {
            background-color: #1e7e34;
        }

        /* Enhanced Name Input */
        #nameInput {
            margin-bottom: 20px;
        }

        #nameInput label {
            display: block;
            font-size: 18px;
            margin-bottom: 8px;
            color: #333;
        }

        #certificateName {
            width: 100%;
            padding: 12px;
            font-size: 16px;
            border: 2px solid #ddd;
            border-radius: 8px;
            box-sizing: border-box;
            margin-bottom: 15px;
            transition: border-color 0.3s ease;
        }

        #certificateName:focus {
            border-color: #1557B0;
            outline: none;
        }

        /* Improved Certificate Design */
        #certificate {
            display: none;
            border: 5px solid #1557B0;
            margin: 20px auto;
            padding: 40px;
            background: #f9f9f9;
            animation: fadeIn 0.5s ease-out forwards;
            max-width: 800px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        #certificate h2 {
            color: #1557B0;
            font-size: 32px;
            margin-bottom: 20px;
        }

        #certificate p {
            font-size: 18px;
            color: #555;
            margin-bottom: 10px;
        }

        #certificate h3 {
            font-size: 24px;
            color: #333;
            margin-bottom: 15px;
        }

        /* Styles for the certificate */
        .certificate-container {
            width: 750px;
            padding: 40px;
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: 15px;
            box-shadow: 0 0 30px rgba(0, 0, 0, 0.15);
            text-align: center;
            margin: 20px auto;
            /* Center the container */
        }

        .certificate {
            position: relative;
            padding: 50px;
            border: 4px solid #f6d365;
            border-radius: 10px;
            overflow: hidden;
        }

        .certificate h1 {
            color: #e44d26;
            font-size: 2.6em;
            margin-bottom: 15px;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.05);
        }

        .certificate .presented-to {
            font-size: 1.2em;
            color: #555;
            margin-bottom: 8px;
        }

        .certificate h2 {
            font-size: 2em;
            color: #29abe2;
            margin-bottom: 10px;
        }

        .certificate .for-completion {
            font-size: 1.2em;
            color: #555;
            margin-bottom: 8px;
        }

        .certificate .course-name {
            font-size: 1.5em;
            color: #8e44ad;
            margin-bottom: 25px;
            font-weight: bold;
        }

        .certificate .date {
            font-size: 1.1em;
            color: #777;
            margin-top: 20px;
        }
    </style>
    <!-- Include jsPDF library -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
</head>

<body>
    <!-- Home Screen -->
    <section id="home" class="home-screen">
        <div class="home-content">
            <h1 class="home-title">Secure Your Future with <span class="highlight">CyberLearn</span> 🛡️</h1>
            <p class="home-subtitle">Unlock the world of cybersecurity with our comprehensive learning platform. From beginner to expert, we've got you covered! 🚀</p>
            <button class="cta-button" onclick="showDashboard()">Start Learning Now</button>
            <div class="home-animation">
                <div class="emoji-animation">💻🔒🌐</div>
                <div class="cyber-animation">
                    <div class="shield">🛡️</div>
                    <div class="lock">🔒</div>
                    <div class="globe">🌐</div>
                </div>
            </div>
        </div>
    </section>

    <nav class="nav-bar">
        <div class="nav-container">
            <a href="#" class="nav-logo">CyberLearn</a>
            <div class="nav-menu">
                <a href="#" class="nav-item" onclick="goToHome()">Home</a>
                <a href="#" class="nav-item" onclick="openTab('overview')">Dashboard</a>
                <a href="#" class="nav-item" onclick="openTab('learning')">Learning Path</a>
                <a href="#" class="nav-item" onclick="openTab('resources')">Resources</a>

                <a href="#" class="nav-item" onclick="openTab('Egypt digital efforts')">Egypt digital efforts</a>
            </div>
            <div class="user-profile" onclick="toggleDropdown()">
                <div class="profile-img"></div>
                <span>Sign In</span>
            </div>
        </div>
    </nav>

    <!-- Sign In Modal -->
    <div id="signInModal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h2>Sign In</h2>
            <form id="signInForm">
                <div class="form-group">
                    <label for="signInEmail">Email</label>
                    <input type="email" id="signInEmail" required>
                </div>
                <div class="form-group">
                    <label for="signInPassword">Password</label>
                    <input type="password" id="signInPassword" required>
                </div>
                <button type="submit" class="btn-primary">Sign In</button>
            </form>
            <p>Don't have an account? <a href="#" onclick="showSignUpModal()">Sign Up</a></p>
        </div>
    </div>

    <!-- Sign Up Modal -->
    <div id="signUpModal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <h2>Sign Up</h2>
            <form id="signUpForm">
                <div class="form-group">
                    <label for="signUpName">Full Name</label>
                    <input type="text" id="signUpName" required>
                </div>
                <div class="form-group">
                    <label for="signUpEmail">Email</label>
                    <input type="email" id="signUpEmail" required>
                </div>
                <div class="form-group">
                    <label for="signUpPassword">Password</label>
                    <input type="password" id="signUpPassword" required>
                </div>
                <div class="form-group">
                    <label for="confirmPassword">Confirm Password</label>
                    <input type="password" id="confirmPassword" required>
                </div>
                <button type="submit" class="btn-primary">Sign Up</button>
            </form>
            <p>Already have an account? <a href="#" onclick="showSignInModal()">Sign In</a></p>
        </div>
    </div>

    <!-- User Profile Dropdown -->
    <div id="userDropdown" class="dropdown">
        <div class="dropdown-content">
            <a href="#" id="logoutLink" onclick="logout()">Logout</a>
        </div>
    </div>

    <!-- Congratulations Animation Container -->
    <div class="congrats-animation" id="congratsAnimation"></div>

    <div class="dashboard">
        <h1>CyberLearn</h1>
        <!-- Tab Container -->
        <div class="tab-container">
            <div class="tab-nav">
                <button class="tab-button active" onclick="openTab('overview')">Overview</button>
                <button class="tab-button" onclick="openTab('learning')">Learning Path</button>
                <button class="tab-button" onclick="openTab('resources')">Resources</button>


                <button class="tab-button" onclick="openTab('Egypt digital efforts')">Egypt digital efforts</button>
            </div>

            <!-- Overview Tab -->
            <div id="overview" class="tab-content active">
                <h2>Cybersecurity Overview</h2>
                <p>Welcome to your cybersecurity learning journey. This course will guide you through fundamental to advanced security concepts.</p>
                <div class="stats-grid">
                    <div class="stat-box">
                        <h3>Course Progress</h3>
                        <p class="stat-number" id="courseProgress">0%</p>
                    </div>
                    <div class="stat-box">
                        <h3>Completed Levels</h3>
                        <p class="stat-number" id="completedLevels">0/10</p>
                    </div>
                    <div class="stat-box">
                        <h3>Time Spent</h3>
                        <p class="stat-number" id="timeSpent">0h 0m</p>
                    </div>
                    <div class="stat-box">
                        <h3>Points Earned</h3>
                        <p class="stat-number" id="pointsEarned">0</p>
                    </div>
                </div>
            </div>

            <!-- Learning Path Tab -->
            <div id="learning" class="tab-content">
                <div class="progress-bar">
                    <div class="progress" id="progress"></div>
                </div>
                <div class="levels">
                    <!-- Level 1 -->
                    <div class="level" id="level1">
                        <h2>Level 1: Introduction to Cybersecurity</h2>
                        <button onclick="loadLevel('level1')">Start Level 1</button>
                        <div class="content" id="level1Content">
                            <h3>Video</h3>
                            <iframe width="100%" height="400" src="https://www.youtube.com/embed/inWWhr5tnEA"
                                frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe>
                            <h3>Article</h3>
                            <p>Cybersecurity is the practice of protecting systems, networks, and programs from digital
                                attacks...</p>
                            <div class="quiz" id="level1Quiz">
                                <h3>Quiz</h3>
                                <p>1. What is the primary goal of cybersecurity?</p>
                                <input type="radio" name="q1" value="a"> A. Develop software <br>
                                <input type="radio" name="q1" value="b"> B. Increase internet speed<br>
                                <input type="radio" name="q1" value="c"> C. protect data <br>
                                <p>2. Which of the following is a common cyber threat?</p>
                                <input type="radio" name="q2" value="a"> A. Rain <br>
                                <input type="radio" name="q2" value="b"> B. Phishing<br>
                                <input type="radio" name="q2" value="c"> C. Sunshine<br>
                                <p>3. What is malware?</p>
                                <input type="radio" name="q3" value="a"> A. Software designed to harm systems<br>
                                <input type="radio" name="q3" value="b"> B. A type of firewall<br>
                                <input type="radio" name="q3" value="c"> C. A network protocol<br>
                                <p>4. What does VPN stand for?</p>
                                <input type="radio" name="q4" value="a"> A. Virtual Private Network<br>
                                <input type="radio" name="q4" value="b"> B. Very Powerful Network<br>
                                <input type="radio" name="q4" value="c"> C. Visual Protection Node<br>
                                <p>5. What is two-factor authentication (2FA)?</p>
                                <input type="radio" name="q5" value="a"> A. A security method requiring two forms of
                                    verification<br>
                                <input type="radio" name="q5" value="b"> B. A type of malware<br>
                                <input type="radio" name="q5" value="c"> C. A network protocol<br>
                                <button onclick="checkQuiz('level1')">Submit Quiz</button>
                                <div class="quiz-result" id="level1Result"></div>
                            </div>
                        </div>
                    </div>
                    <!-- Level 2 -->
                    <div class="level locked" id="level2">
                        <h2>Level 2: Network Security</h2>
                        <button disabled>Locked</button>
                        <div class="content" id="level2Content">
                            <h3>Video</h3>
                            <iframe width="100%" height="400" src="https://www.youtube.com/embed/--onbg-jHqQ"
                                frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe>
                            <h3>Article</h3>
                            <p>Network security involves implementing measures to protect the integrity, confidentiality,
                                and availability of data as it is transmitted across or accessed through networks.</p>
                            <div class="quiz" id="level2Quiz">
                                <h3>Quiz</h3>
                                <p>1. What is a firewall used for?</p>
                                <input type="radio" name="q1" value="a"> A. Store data <br>
                                <input type="radio" name="q1" value="b"> B. Block unauthorized access <br>
                                <input type="radio" name="q1" value="c"> C. Increase internet speed <br>
                                <p>2. Which protocol is used for secure communication over a network?</p>
                                <input type="radio" name="q2" value="a"> A. HTTPS<br>
                                <input type="radio" name="q2" value="b"> B. HTTP<br>
                                <input type="radio" name="q2" value="c"> C. FTP<br>
                                <p>3. What is an IP address?</p>
                                <input type="radio" name="q3" value="a"> A. A network protocol<br>
                                <input type="radio" name="q3" value="b"> B. A type of malware<br>
                                <input type="radio" name="q3" value="c"> C. A unique identifier for devices on a
                                    network<br>
                                <p>4. What is a DDoS attack?</p>
                                <input type="radio" name="q4" value="a"> A. Overwhelming a network with traffic<br>
                                <input type="radio" name="q4" value="b"> B. Stealing data<br>
                                <input type="radio" name="q4" value="c"> C. Encrypting files<br>
                                <p>5. What is a VPN used for?</p>
                                <input type="radio" name="q5" value="a"> A. Block malware <br>
                                <input type="radio" name="q5" value="b"> B. Increase internet speed<br>
                                <input type="radio" name="q5" value="c"> C. Secure remote access to a network<br>
                                <button onclick="checkQuiz('level2')">Submit Quiz</button>
                                <div class="quiz-result" id="level2Result"></div>
                            </div>
                        </div>
                    </div>
                    <!-- Level 3 -->
                    <div class="level locked" id="level3">
                        <h2>Level 3: Advanced Security</h2>
                        <button disabled>Locked</button>
                        <div class="content" id="level3Content">
                            <h3>Video</h3>
                            <iframe width="100%" height="400" src="https://www.youtube.com/embed/-BIANfzF43k"
                                frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe>
                            <h3>Article</h3>
                            <p>Advanced security involves protecting systems from sophisticated threats such as zero-day
                                exploits, ransomware, and advanced persistent threats (APTs).</p>
                            <div class="quiz" id="level3Quiz">
                                <h3>Quiz</h3>
                                <p>1. What is a zero-day exploit?</p>
                                <input type="radio" name="q1" value="a"> A. A vulnerability unknown to the vendor<br>
                                <input type="radio" name="q1" value="b"> B. A type of malware<br>
                                <input type="radio" name="q1" value="c"> C. A network protocol<br>
                                <p>2. What is ransomware?</p>
                                <input type="radio" name="q2" value="a"> A. Malware that encrypts data<br>
                                <input type="radio" name="q2" value="b"> B. A type of firewall<br>
                                <input type="radio" name="q2" value="c"> C. A network monitoring tool<br>
                                <p>3. What is an APT?</p>
                                <input type="radio" name="q3" value="a"> A. A type of virus<br>
                                <input type="radio" name="q3" value="b"> B. A network protocol<br>
                                <input type="radio" name="q3" value="c"> C. A long-term targeted attack <br>
                                <p>4. What is social engineering?</p>
                                <input type="radio" name="q4" value="a"> A. A type of malware<br>
                                <input type="radio" name="q4" value="b"> B. Manipulating people to gain access to
                                    systems<br>
                                <input type="radio" name="q4" value="c"> C. A network protocol<br>
                                <p>5. What is a honeypot?</p>
                                <input type="radio" name="q5" value="a"> A. A type of firewall <br>
                                <input type="radio" name="q5" value="b"> B. A decoy system to attract attackers<br>
                                <input type="radio" name="q5" value="c"> C. A network protocol<br>
                                <button onclick="checkQuiz('level3')">Submit Quiz</button>
                                <div class="quiz-result" id="level3Result"></div>
                            </div>
                        </div>
                    </div>

                    <!-- Level 4 -->
                    <div class="level locked" id="level4">
                        <h2>Level 4: Cryptography Basics</h2>
                        <button disabled>Locked</button>
                        <div class="content" id="level4Content">
                            <h3>Video</h3>
                            <iframe width="100%" height="400" src=" https://www.youtube.com/embed/https://www.youtube.com/watch?v=InxVxKm4wSQ"
                                title="Cryptography Basics - A Practical Introduction" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                                allowfullscreen></iframe>
                            <h3>Article</h3>
                            <p>Cryptography is the practice and study of techniques for secure communication in the
                                presence of adversaries.</p>
                            <div class="quiz" id="level4Quiz">
                                <h3>Quiz</h3>
                                <p>1. What is encryption?</p>
                                <input type="radio" name="q1" value="a"> A. Hiding data <br>
                                <input type="radio" name="q1" value="b"> B. Converting data into a secure format<br>
                                <input type="radio" name="q1" value="c"> C. Compressing data<br>
                                <p>2. What is a cipher?</p>
                                <input type="radio" name="q2" value="a"> A. A type of firewall<br>
                                <input type="radio" name="q2" value="b"> B. An algorithm for encryption or decryption<br>
                                <input type="radio" name="q2" value="c"> C. A network protocol<br>
                                <p>3. What is a key in cryptography?</p>
                                <input type="radio" name="q3" value="a"> A. A physical lock<br>
                                <input type="radio" name="q3" value="b"> B. A secret value used in encryption and
                                    decryption<br>
                                <input type="radio" name="q3" value="c"> C. A type of malware<br>
                                <p>4. What is hashing?</p>
                                <input type="radio" name="q4" value="a"> A. Encrypting data<br>
                                <input type="radio" name="q4" value="b"> B. Converting data into a fixed-size string<br>
                                <input type="radio" name="q4" value="c"> C. Compressing data<br>
                                <p>5. What is the purpose of digital signatures?</p>
                                <input type="radio" name="q5" value="a"> A. Encrypting emails<br>
                                <input type="radio" name="q5" value="b"> B. Verifying the authenticity and integrity of
                                    a message<br>
                                <input type="radio" name="q5" value="c"> C. Blocking network traffic<br>
                                <button onclick="checkQuiz('level4')">Submit Quiz</button>
                                <div class="quiz-result" id="level4Result"></div>
                            </div>
                        </div>
                    </div>

                    <!-- Level 5 -->
                    <div class="level locked" id="level5">
                        <h2>Level 5: Incident Response</h2>
                        <button disabled>Locked</button>
                        <div class="content" id="level5Content">
                            <h3>Video</h3>
                            <iframe width="100%" height="400" src="https://www.youtube.com/watch?v=9-W55MB-y24"
                                title="Cyber Security Incident Response Process" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                                allowfullscreen></iframe>
                            <h3>Article</h3>
                            <p>Incident response is the process of handling and managing the aftermath of a security
                                breach or cyberattack.</p>
                            <div class="quiz" id="level5Quiz">
                                <h3>Quiz</h3>
                                <p>1. What is the first step in incident response?</p>
                                <input type="radio" name="q1" value="a"> A. Eradication<br>
                                <input type="radio" name="q1" value="b"> B. Identification<br>
                                <input type="radio" name="q1" value="c"> C. Recovery<br>
                                <p>2. What does containment involve?</p>
                                <input type="radio" name="q2" value="a"> A. Identifying the source of the incident<br>
                                <input type="radio" name="q2" value="b"> B. Limiting the scope and impact of the
                                    incident<br>
                                <input type="radio" name="q2" value="c"> C. Restoring systems to normal operation<br>
                                <p>3. What is eradication?</p>
                                <input type="radio" name="q3" value="a"> A. Identifying the attacker<br>
                                <input type="radio" name="q3" value="b"> B. Removing malware and vulnerabilities<br>
                                <input type="radio" name="q3" value="c"> C. Documenting the incident<br>
                                <p>4. What is the purpose of the recovery phase?</p>
                                <input type="radio" name="q4" value="a"> A. Restoring systems to normal operation<br>
                                <input type="radio" name="q4" value="b"> B. Identifying the attacker<br>
                                <input type="radio" name="q4" value="c"> C. Containing the incident<br>
                                <p>5. What is the final step in incident response?</p>
                                <input type="radio" name="q5" value="a"> A. Containment<br>
                                <input type="radio" name="q5" value="b"> B. Lessons learned<br>
                                <input type="radio" name="q5" value="c"> C. Eradication<br>
                                <button onclick="checkQuiz('level5')">Submit Quiz</button>
                                <div class="quiz-result" id="level5Result"></div>
                            </div>
                        </div>
                    </div>

                    <!-- Level 6 -->
                    <div class="level locked" id="level6">
                        <h2>Level 6: Web Application Security</h2>
                        <button disabled>Locked</button>
                        <div class="content" id="level6Content">
                            <h3>Video</h3>
                            <iframe width="100%" height="400" src="https://www.youtube.com/watch?v=spjvU4C5C-Y"
                                title="Web Application Security" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                                allowfullscreen></iframe>
                            <h3>Article</h3>
                            <p>Web application security involves implementing measures to protect web applications from
                                cyber threats.</p>
                            <div class="quiz" id="level6Quiz">
                                <h3>Quiz</h3>
                                <p>1. What is SQL injection?</p>
                                <input type="radio" name="q1" value="a"> A. Injecting HTML code<br>
                                <input type="radio" name="q1" value="b"> B. Injecting SQL code to manipulate a database<br>
                                <input type="radio" name="q1" value="c"> C. Injecting JavaScript code<br>
                                <p>2. What is Cross-Site Scripting (XSS)?</p>
                                <input type="radio" name="q2" value="a"> A. Executing scripts on a server<br>
                                <input type="radio" name="q2" value="b"> B. Injecting malicious scripts into websites<br>
                                <input type="radio" name="q2" value="c"> C. Blocking network traffic<br>
                                <p>3. What is Cross-Site Request Forgery (CSRF)?</p>
                                <input type="radio" name="q3" value="a"> A. Forging network requests<br>
                                <input type="radio" name="q3" value="b"> B. Forcing users to execute unwanted actions<br>
                                <input type="radio" name="q3" value="c"> C. Encrypting web traffic<br>
                                <p>4. What is authentication?</p>
                                <input type="radio" name="q4" value="a"> A. Verifying user identity<br>
                                <input type="radio" name="q4" value="b"> B. Encrypting data<br>
                                <input type="radio" name="q4" value="c"> C. Blocking network traffic<br>
                                <p>5. What is authorization?</p>
                                <input type="radio" name="q5" value="a"> A. Verifying user identity<br>
                                <input type="radio" name="q5" value="b"> B. Granting access to resources based on
                                    permissions<br>
                                <input type="radio" name="q5" value="c"> C. Encrypting data<br>
                                <button onclick="checkQuiz('level6')">Submit Quiz</button>
                                <div class="quiz-result" id="level6Result"></div>
                            </div>
                        </div>
                    </div>

                    <!-- Level 7 -->
                    <div class="level locked" id="level7">
                        <h2>Level 7: Mobile Security</h2>
                        <button disabled>Locked</button>
                        <div class="content" id="level7Content">
                            <h3>Video</h3>
                            <iframe width="100%" height="400" src="https://www.youtube.com/watch?v=4G-LzVd5w9A"
                                title="Mobile Security - What You Need To Know" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                                allowfullscreen></iframe>
                            <h3>Article</h3>
                            <p>Mobile security involves protecting mobile devices and networks from cyber threats.</p>
                            <div class="quiz" id="level7Quiz">
                                <h3>Quiz</h3>
                                <p>1. What is mobile malware?</p>
                                <input type="radio" name="q1" value="a"> A. Software designed to harm mobile devices<br>
                                <input type="radio" name="q1" value="b"> B. A type of firewall<br>
                                <input type="radio" name="q1" value="c"> C. A network protocol<br>
                                <p>2. What is sideloading?</p>
                                <input type="radio" name="q2" value="a"> A. Downloading apps from official app stores<br>
                                <input type="radio" name="q2" value="b"> B. Installing apps from unofficial sources<br>
                                <input type="radio" name="q2" value="c"> C. Encrypting data<br>
                                <p>3. What is jailbreaking/rooting?</p>
                                <input type="radio" name="q3" value="a"> A. Removing security restrictions on mobile
                                    devices<br>
                                <input type="radio" name="q3" value="b"> B. Installing a firewall<br>
                                <input type="radio" name="q3" value="c"> C. Encrypting data<br>
                                <p>4. What is mobile device management (MDM)?</p>
                                <input type="radio" name="q4" value="a"> A. Managing mobile devices remotely<br>
                                <input type="radio" name="q4" value="b"> B. Encrypting data<br>
                                <input type="radio" name="q4" value="c"> C. Blocking network traffic<br>
                                <p>5. What is the importance of app permissions?</p>
                                <input type="radio" name="q5" value="a"> A. They are not important<br>
                                <input type="radio" name="q5" value="b"> B. They control what an app can access on a
                                    device<br>
                                <input type="radio" name="q5" value="c"> C. They encrypt data<br>
                                <button onclick="checkQuiz('level7')">Submit Quiz</button>
                                <div class="quiz-result" id="level7Result"></div>
                            </div>
                        </div>
                    </div>

                    <!-- Level 8 -->
                    <div class="level locked" id="level8">
                        <h2>Level 8: Cloud Security</h2>
                        <button disabled>Locked</button>
                        <div class="content" id="level8Content">
                            <h3>Video</h3>
                            <iframe width="100%" height="400" src="https://www.youtube.com/watch?v=wS-vbsWw-zs"
                                title="Cloud Security Explained" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                                allowfullscreen></iframe>
                            <h3>Article</h3>
                            <p>Cloud security involves protecting cloud-based systems and data from cyber threats.</p>
                            <div class="quiz" id="level8Quiz">
                                <h3>Quiz</h3>
                                <p>1. What is cloud computing?</p>
                                <input type="radio" name="q1" value="a"> A. Storing data on a local device<br>
                                <input type="radio" name="q1" value="b"> B. Delivering computing services over the
                                    internet<br>
                                <input type="radio" name="q1" value="c"> C. Encrypting data<br>
                                <p>2. What is Infrastructure as a Service (IaaS)?</p>
                                <input type="radio" name="q2" value="a"> A. Providing software over the internet<br>
                                <input type="radio" name="q2" value="b"> B. Providing virtualized computing resources<br>
                                <input type="radio" name="q2" value="c"> C. Providing a platform for developing
                                    applications<br>
                                <p>3. What is Platform as a Service (PaaS)?</p>
                                <input type="radio" name="q3" value="a"> A. Providing software over the internet<br>
                                <input type="radio" name="q3" value="b"> B. Providing virtualized computing resources<br>
                                <input type="radio" name="q3" value="c"> C. Providing a platform for developing
                                    applications<br>
                                <p>4. What is Software as a Service (SaaS)?</p>
                                <input type="radio" name="q4" value="a"> A. Providing software over the internet<br>
                                <input type="radio" name="q4" value="b"> B. Providing virtualized computing resources<br>
                                <input type="radio" name="q4" value="c"> C. Providing a platform for developing
                                    applications<br>
                                <p>5. What is the shared responsibility model in cloud security?</p>
                                <input type="radio" name="q5" value="a"> A. The cloud provider is responsible for all
                                    security aspects<br>
                                <input type="radio" name="q5" value="b"> B. The customer is responsible for all security
                                    aspects<br>
                                <input type="radio" name="q5" value="c"> C. The cloud provider and customer share
                                    security responsibilities<br>
                                <button onclick="checkQuiz('level8')">Submit Quiz</button>
                                <div class="quiz-result" id="level8Result"></div>
                            </div>
                        </div>
                    </div>

                    <!-- Level 9 -->
                    <div class="level locked" id="level9">
                        <h2>Level 9: IoT Security</h2>
                        <button disabled>Locked</button>
                        <div class="content" id="level9Content">
                            <h3>Video</h3>
                            <iframe width="100%" height="400" src="https://www.youtube.com/watch?v=j6Ywf-v2Y-o"
                                title="IoT Security Explained" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                                allowfullscreen></iframe>
                            <h3>Article</h3>
                            <p>IoT security involves protecting Internet of Things (IoT) devices and networks from cyber
                                threats.</p>
                            <div class="quiz" id="level9Quiz">
                                <h3>Quiz</h3>
                                <p>1. What is the Internet of Things (IoT)?</p>
                                <input type="radio" name="q1" value="a"> A. A network protocol<br>
                                <input type="radio" name="q1" value="b"> B. A network of interconnected devices<br>
                                <input type="radio" name="q1" value="c"> C. A type of malware<br>
                                <p>2. What are common IoT security risks?</p>
                                <input type="radio" name="q2" value="a"> A. Strong passwords<br>
                                <input type="radio" name="q2" value="b"> B. Weak default passwords and unencrypted
                                    communication<br>
                                <input type="radio" name="q2" value="c"> C. Regular security updates<br>
                                <p>3. What is device authentication?</p>
                                <input type="radio" name="q3" value="a"> A. Verifying device identity<br>
                                <input type="radio" name="q3" value="b"> B. Encrypting data<br>
                                <input type="radio" name="q3" value="c"> C. Blocking network traffic<br>
                                <p>4. What is data encryption?</p>
                                <input type="radio" name="q4" value="a"> A. Hiding data<br>
                                <input type="radio" name="q4" value="b"> B. Converting data into a secure format<br>
                                <input type="radio" name="q4" value="c"> C. Compressing data<br>
                                <p>5. What is the importance of regular security updates for IoT devices?</p>
                                <input type="radio" name="q5" value="a"> A. They are not important<br>
                                <input type="radio" name="q5" value="b"> B. They patch vulnerabilities and improve
                                    security<br>
                                <input type="radio" name="q5" value="c"> C. They encrypt data<br>
                                <button onclick="checkQuiz('level9')">Submit Quiz</button>
                                <div class="quiz-result" id="level9Result"></div>
                            </div>
                        </div>
                    </div>

                    <!-- Level 10 -->
                    <div class="level locked" id="level10">
                        <h2>Level 10: Cybersecurity Compliance</h2>
                        <button disabled>Locked</button>
                        <div class="content" id="level10Content">
                            <h3>Video</h3>
                            <iframe width="100%" height="400" src=" https://www.youtube.com/embed/https://www.youtube.com/watch?v=Vw-l45yK-loh"
                                title="Cybersecurity Compliance Explained" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                                allowfullscreen></iframe>
                            <h3>Article</h3>
                            <p>Cybersecurity compliance involves adhering to regulations and standards to protect
                                sensitive data.</p>
                            <div class="quiz" id="level10Quiz">
                                <h3>Quiz</h3>
                                <p>1. What is GDPR?</p>
                                <input type="radio" name="q1" value="a"> A. A network protocol<br>
                                <input type="radio" name="q1" value="b"> B. A data protection regulation in the
                                    European Union<br>
                                <input type="radio" name="q1" value="c"> C. A type of malware<br>
                                <p>2. What is HIPAA?</p>
                                <input type="radio" name="q2" value="a"> A. A health information regulation in the United
                                    States<br>
                                <input type="radio" name="q2" value="b"> B. A network protocol<br>
                                <input type="radio" name="q2" value="c"> C. A type of firewall<br>
                                <p>3. What is PCI DSS?</p>
                                <input type="radio" name="q3" value="a"> A. A payment card industry standard<br>
                                <input type="radio" name="q3" value="b"> B. A network protocol<br>
                                <input type="radio" name="q3" value="c"> C. A type of malware<br>
                                <p>4. What is compliance?</p>
                                <input type="radio" name="q4" value="a"> A. Adhering to regulations and standards<br>
                                <input type="radio" name="q4" value="b"> B. Encrypting data<br>
                                <input type="radio" name="q4" value="c"> C. Blocking network traffic<br>
                                <p>5. What is the importance of cybersecurity compliance?</p>
                                <input type="radio" name="q5" value="a"> A. It is not important<br>
                                <input type="radio" name="q5" value="b"> B. It protects sensitive data and ensures legal
                                    adherence<br>
                                <input type="radio" name="q5" value="c"> C. It encrypts data<br>
                                <button onclick="checkQuiz('level10')">Submit Quiz</button>
                                <div class="quiz-result" id="level10Result"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <!-- Congratulations Screen -->
            <div id="congratulationsScreen"
                style="display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0, 0, 0, 0.9); z-index: 1000;">
                <div
                    style="position: relative; background: white; max-width: 600px; margin: 50px auto; padding: 30px; border-radius: 15px; text-align: center; animation: slideInCongratulations 0.5s ease-out forwards;">
                    <h2>Congratulations!</h2>
                    <p>You have completed all levels!</p>
                    <div id="nameInput">
                        <label for="certificateName">Enter your name to generate a certificate:</label>
                        <input type="text" id="certificateName" placeholder="Your Name">
                    </div>
                    <button id="generateCertificateBtn" onclick="generateCertificate()"
                        style="background-color: #1557B0; color: white; padding: 15px 30px; border: none; border-radius: 8px; font-size: 18px; cursor: pointer; transition: background-color 0.3s ease;">Generate
                        Certificate</button>
                    <button onclick="backToDashboard()"
                        style="background-color: #c45637; color: white; padding: 15px 30px; border: none; border-radius: 8px; font-size: 18px; cursor: pointer; transition: background-color 0.3s ease;">Back
                        to Dashboard</button>
                    <button id="downloadCertificateBtn" onclick="downloadCertificate()"
                        style="background-color: #28a745; color: white; padding: 15px 30px; border: none; border-radius: 8px; font-size: 18px; cursor: pointer; transition: background-color 0.3s ease; display:none;">Download
                        Certificate</button>
                </div>
            </div>
            <!-- Certificate -->
            <div id="certificate">
                <h2>Certificate of Completion</h2>
                <p>This certificate is awarded to</p>
                <h3 id="certificateNameDisplay"></h3>
                <p>for successfully completing the Cybersecurity Learning Course.</p>
                <p>Date: <span id="certificateDate"></span></p>
            </div>

            <!-- Certificate Container for jsPDF -->
            <div id="certificateContainer" style="display:none;">
                <div class="certificate">
                    <h1>Certificate of Completion</h1>
                    <p class="presented-to">This certificate is presented to</p>
                    <h2 id="certificateNameToDownload"></h2>
                    <p class="for-completion">For successfully completing the course</p>
                    <p class="course-name">Cybersecurity Learning Course</p>
                    <p class="date">Date: <span id="certificateDateToDownload"></span></p>
                </div>
            </div>
        </div>

        <!-- Resources Tab -->
        <div id="resources" class="tab-content">
            <h2>Additional Resources</h2>
            <div class="resource-grid">
                <div class="resource-card">
                    <h3>Documentation</h3>
                    <p>Access comprehensive cybersecurity documentation</p>
                    <a href="https://complianceforge.com/example-cybersecurity-documentation/"
                        class="resource-link">View Docs</a>
                </div>
                <div class="resource-card">
                    <h3>Practice Labs</h3>
                    <p>Hands-on virtual labs for practical experience</p>
                    <a href="https://youtu.be/DY-Eup8My-I?si=0S9hZdA8_txxYeZf" class="resource-link">Start Lab</a>
                </div>
                <div class="resource-card">
                    <h3>Community</h3>
                    <p>Connect with other cybersecurity learners</p>
                    <a href="https://chat.whatsapp.com/BBpbIZe3Tsz4IImCLOH7Jz" class="resource-link">Join Now</a>
                </div>
            </div>
        </div>
        <!-- Egypt digital efforts Tab -->
        <div id="Egypt digital efforts" class="tab-content">
            <h2>Egypt digital efforts</h2>
            <p>In recent years, Egypt has emerged as a regional leader in digital transformation, leveraging technology
                to drive economic growth, improve public services, and enhance its global competitiveness. However,
                with the rapid adoption of digital technologies comes the increasing risk of cyber threats. Recognizing
                this, the Egyptian government has taken proactive steps to strengthen its cybersecurity infrastructure
                and educate its youth on the importance of cybersecurity. These efforts are not only safeguarding the
                nation’s digital assets but also preparing a new generation of tech-savvy professionals to tackle the
                challenges of the digital age.</p>
            <h3>- Awareness Campaign</h3>
            <div class="video-container">
                <iframe width="560" height="315" src="https://www.youtube.com/embed/IJFYi_w6hbk" frameborder="0"
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                    allowfullscreen></iframe>
            </div>
            <h3> - The Road Ahead:</h3>
            <p>As Egypt accelerates its digital transformation, the country has become a target for cybercriminals. From
                ransomware attacks on critical infrastructure to phishing scams targeting individuals, the threat
                landscape is evolving rapidly. According to a 2022 report by the Egyptian Computer Emergency Readiness
                Team (EG-CERT), cyber attacks in Egypt increased by 30% compared to the previous year. These attacks
                have targeted government institutions, financial systems, and private businesses, highlighting the
                urgent need for robust cybersecurity measures. In response, the Egyptian government has made
                cybersecurity a top priority, integrating it into its national development strategy. The country’s
                Vision 2030 plan emphasizes the importance of building a secure digital ecosystem to support economic
                growth and protect citizens’ data.</p>
            <h3> - Launching the National Cybersecurity Strategy:</h3>
            <p>The Supreme Council for Cybersecurity, affiliated to the Presidency of the Council of Ministers, chaired
                by the Minister of Communications and Information Technology, launched the National Cybersecurity
                Strategy (2017-2021), which aims to secure the communications and information infrastructure in an
                integrated manner to provide a secure environment for various sectors to provide integrated electronic
                services, within the framework of the state's efforts to support national security and the development
                of the Egyptian society</p>
            <h3> - Formation of the Supreme Council for Cybersecurity in Egypt 2014:</h3>
            <p>The Supreme Council for Cybersecurity in Egypt was formed by a decision of former Prime Minister Eng.
                Ibrahim Mahlab in December 2014, and aims to protect the information and data of the authorities with
                attention to the information and communication departments in the ministries and various entities, and
                to ensure the availability of the necessary funding to ensure the implementation of the cybersecurity
                system, with the need for clarity of its legislative framework, and its formation includes the Minister
                of Communications and Information Technology as Chairman of the Council, and the membership of
                representatives of the ministries: Defense, Foreign Affairs, Interior, Petroleum and Mineral Resources,
                Electricity, Health, Water Resources and Irrigation, Supply, Communications, General Intelligence
                Service, Central Bank, and 3 experienced members.</p>


            <!-- Progress Tab -->

            <div id="progress" class="tab-content">
                <div class="progress-tab-content">
                    <div class="points-display" id="totalPoints">Points: 0</div>
                    <ul class="level-progress-list" id="levelProgressList">
                        <li class="level-progress-item">
                            <span class="level-name">Level 1: Introduction to Cybersecurity</span>
                            <span class="level-status" id="level1Status">Incomplete</span>
                        </li>
                        <li class="level-progress-item">
                            <span class="level-name">Level 2: Network Security</span>
                            <span class="level-status" id="level2Status">Locked</span>
                        </li>
                        <li class="level-progress-item">
                            <span class="level-name">Level 3: Advanced Security</span>
                            <span class="level-status" id="level3Status">Locked</span>
                        </li>
                        <li class="level-progress-item">
                            <span class="level-name">Level 4: Cryptography Basics</span>
                            <span class="level-status" id="level4Status">Locked</span>
                        </li>
                        <li class="level-progress-item">
                            <span class="level-name">Level 5: Incident Response</span>
                            <span class="level-status" id="level5Status">Locked</span>
                        </li>
                        <li class="level-progress-item">
                            <span class="level-name">Level 6: Web Application Security</span>
                            <span class="level-status" id="level6Status">Locked</span>
                        </li>
                        <li class="level-progress-item">
                            <span class="level-name">Level 7: Mobile Security</span>
                            <span class="level-status" id="level7Status">Locked</span>
                        </li>
                        <li class="level-progress-item">
                            <span class="level-name">Level 8: Cloud Security</span>
                            <span class="level-status" id="level8Status">Locked</span>
                        </li>
                        <li class="level-progress-item">
                            <span class="level-name">Level 9: IoT Security</span>
                            <span class="level-status" id="level9Status">Locked</span>
                        </li>
                        <li class="level-progress-item">
                            <span class="level-name">Level 10: Cybersecurity Compliance</span>
                            <span class="level-status" id="level10Status">Locked</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>

        <script>
         
    // Global variables for tracking progress
    let timeSpent = 0;
    let completedLevels = 0;
    let courseProgress = 0;
    let timerInterval;
    let currentUser = null; // Track the current user
    let totalPoints = 0; // Track total points
    const totalLevels = 10; // Define the total number of levels

    // Initialize progress tracking function
    function initializeProgress() {
        // Load saved progress if user is logged in
        loadProgress();
        // Start timer
        startTimer();
        // Initial stats update
        updateStats();
    }

    // Timer function
    function startTimer() {
        // Clear any existing timer
        if (timerInterval) {
            clearInterval(timerInterval);
        }
        timerInterval = setInterval(() => {
            timeSpent++;
            updateTimeDisplay();
        }, 1000); // Update every second
    }

    // Update time display function
    function updateTimeDisplay() {
        const hours = Math.floor(timeSpent / 3600);
        const minutes = Math.floor((timeSpent % 3600) / 60);
        const timeDisplay = `${hours}h ${minutes}m`;
        document.getElementById('timeSpent').textContent = timeDisplay;
    }


    function updateStats() {
        // Calculate progress percentage
        courseProgress = Math.round((completedLevels / totalLevels) * 100);

        // Update stats display
        document.getElementById('courseProgress').textContent = `${courseProgress}%`;
        document.getElementById('completedLevels').textContent = `${completedLevels}/${totalLevels}`;
        document.getElementById('timeSpent').textContent = `${Math.floor(timeSpent / 3600)}h ${Math.floor((timeSpent % 3600) / 60)}m`;
        document.getElementById('pointsEarned').textContent = totalPoints;
        document.getElementById('totalPoints').textContent = `Points: ${totalPoints}`;

        // Update progress bar
        document.getElementById('progress').style.width = `${courseProgress}%`;

        // Update level progress list
        updateLevelProgressList();

        // Save progress if user is logged in
        if (currentUser) {
            saveProgress();
        }
    }

    function updateLevelProgressList() {
        const levelProgressList = document.getElementById('levelProgressList');
        const levels = ['level1', 'level2', 'level3', 'level4', 'level5', 'level6', 'level7', 'level8', 'level9', 'level10'];
        levels.forEach(levelId => {
            const levelStatusElement = document.getElementById(`${levelId}Status`);
            const levelElement = document.getElementById(levelId);

            if (levelElement && levelElement.classList.contains('completed')) { // Check for "completed" class
                levelStatusElement.textContent = 'Completed';
                levelStatusElement.classList.add('completed');
            } else if (!levelElement.classList.contains('locked')) {
                levelStatusElement.textContent = 'Unlocked';
                levelStatusElement.classList.remove('completed');
            } else {
                levelStatusElement.textContent = 'Locked';
                levelStatusElement.classList.remove('completed');
            }
        });
    }


    function goToSeQuize() {
        try {
            window.location.href = 'SeQuize.html';
        } catch (error) {
            console.error('Error navigating to SeQuize:', error);
            alert('Unable to navigate to SeQuize. Please try again.');
        }
    }

    function loadLevel(levelId) {
        document.querySelectorAll('.content').forEach(content => {
            content.classList.remove('active');
        });
        const levelContent = document.getElementById(`${levelId}Content`);
        if (levelContent) {
            levelContent.classList.add('active');
        } else {
            console.error(`Content for ${levelId} not found.`);
        }
    }

    function completeAllLevels() {
        // Update progress to 100%
        completedLevels = totalLevels; // All levels are completed
        courseProgress = 100; // Progress is 100%
        updateStats(); // Update the UI

        // Show the congratulations screen
        setTimeout(() => {
            showCongratulationsScreen();
        }, 1000); // Show after 1 second
    }

    function checkQuiz(levelId) {
        const quiz = document.getElementById(`${levelId}Quiz`);
        const resultDiv = document.getElementById(`${levelId}Result`);
        const answers = {
            level1: { q1: 'c', q2: 'b', q3: 'a', q4: 'a', q5: 'a' },
            level2: { q1: 'b', q2: 'a', q3: 'c', q4: 'a', q5: 'c' },
            level3: { q1: 'a', q2: 'a', q3: 'c', q4: 'b', q5: 'b' },
            level4: { q1: 'b', q2: 'b', q3: 'b', q4: 'b', q5: 'b' },
            level5: { q1: 'b', q2: 'b', q3: 'b', q4: 'a', q5: 'b' },
            level6: { q1: 'b', q2: 'b', q3: 'b', q4: 'a', q5: 'b' },
            level7: { q1: 'a', q2: 'b', q3: 'a', q4: 'a', q5: 'b' },
            level8: { q1: 'b', q2: 'b', q3: 'c', q4: 'a', q5: 'c' },
            level9: { q1: 'b', q2: 'b', q3: 'a', q4: 'b', q5: 'b' },
            level10: { q1: 'b', q2: 'a', q3: 'a', q4: 'a', q5: 'b' }
        };
        let score = 0;
        for (let i = 1; i <= 5; i++) {
            const userAnswer = quiz.querySelector(`input[name="q${i}"]:checked`)?.value;
            if (userAnswer === answers[levelId][`q${i}`]) {
                score++;
            }
        }

        if (score >= 4) {
            resultDiv.textContent = `You passed! Score: ${score}/5`;
            resultDiv.style.color = 'green';
            totalPoints += 100; // Award 100 points for passing

            // Increment completedLevels if the level is not already completed
            const levelElement = document.getElementById(levelId);
            if (levelElement && !levelElement.classList.contains('completed')) {
                completedLevels++; // Increment completed levels
                levelElement.classList.add('completed'); // Mark the level as completed
            }

            updateStats(); // Update stats
            showCongratsAnimation(); // Show congratulations animation

            if (levelId === 'level10') {
                // Call the new function for Level 10
                completeAllLevels();
            } else {
                // Unlock the next level
                unlockNextLevel(levelId);
            }
        } else {
            resultDiv.textContent = `You failed. Score: ${score}/5. Try again!`;
            resultDiv.style.color = 'red';
        }
    }


    function unlockNextLevel(levelId) {
        const currentLevel = document.getElementById(levelId);
        const nextLevel = currentLevel.nextElementSibling;
        if (nextLevel && nextLevel.classList.contains('locked')) {
            nextLevel.classList.remove('locked');
            const button = nextLevel.querySelector('button');
            button.disabled = false;
            const nextLevelId = nextLevel.id;
            button.textContent = `Start ${nextLevel.querySelector('h2').textContent.split(':')[0]}`;
            button.setAttribute('onclick', `loadLevel('${nextLevelId}')`);
        }
    }

    function showCongratulationsScreen() {
        document.getElementById('congratulationsScreen').style.display = 'block';
    }

    function generateCertificate() {
        const name = document.getElementById('certificateName').value.trim();
        if (!name) {
            alert('Please enter your name');
            return;
        }
        document.getElementById('certificate').style.display = 'block';
        document.getElementById('certificateNameDisplay').textContent = name;
        document.getElementById('certificateDate').textContent = new Date().toLocaleDateString();

        // Set values for jsPDF certificate
        document.getElementById('certificateNameToDownload').textContent = name;
        document.getElementById('certificateDateToDownload').textContent = new Date().toLocaleDateString();

        document.getElementById('nameInput').style.display = 'none';
        document.getElementById('generateCertificateBtn').style.display = 'none';
        document.getElementById('downloadCertificateBtn').style.display = 'inline-block'; // Show the download button
    }

    function backToDashboard() {
        document.getElementById('congratulationsScreen').style.display = 'none';
        document.getElementById('certificate').style.display = 'none';
        document.getElementById('nameInput').style.display = 'block';
        document.getElementById('generateCertificateBtn').style.display = 'inline-block';
        document.getElementById('downloadCertificateBtn').style.display = 'none';
        document.getElementById('certificateName').value = '';
        document.querySelectorAll('.content').forEach(content => {
            content.classList.remove('active');
        });
    }

    function openTab(tabName) {
        // Hide all tab content
        const tabContents = document.getElementsByClassName('tab-content');
        for (let content of tabContents) {
            content.classList.remove('active');
        }

        // Remove active class from all buttons
        const tabButtons = document.getElementsByClassName('tab-button');
        for (let button of tabButtons) {
            button.classList.remove('active');
        }

        // Show the selected tab content and activate the button
        document.getElementById(tabName).classList.add('active');

        // Find the button that corresponds to the tabName and add the active class
        const tabButton = document.querySelector(`.tab-button[onclick="openTab('${tabName}')"]`);
        if (tabButton) {
            tabButton.classList.add('active');
        }

        // Only show levels in learning tab
        const levelsSection = document.querySelector('.levels');
        if (tabName === 'learning') {
            levelsSection.style.display = 'block';
        } else {
            levelsSection.style.display = 'none';
        }
    }

    // User Authentication Functions
    function showSignInModal() {
        document.getElementById('signUpModal').style.display = 'none';
        document.getElementById('signInModal').style.display = 'block';
    }

    function showSignUpModal() {
        document.getElementById('signInModal').style.display = 'none';
        document.getElementById('signUpModal').style.display = 'block';
    }

    function closeModals() {
        document.getElementById('signInModal').style.display = 'none';
        document.getElementById('signUpModal').style.display = 'none';
    }

    function toggleDropdown() {
        const dropdown = document.getElementById('userDropdown');
        dropdown.style.display = dropdown.style.display === 'block' ? 'none' : 'block';
    }

    function logout() {
        currentUser = null;
        clearInterval(timerInterval); // Stop the timer
        timeSpent = 0;
        completedLevels = 0;
        courseProgress = 0;
        totalPoints = 0;
        updateStats();
        localStorage.removeItem('userProgress');
        updateUserInterface();

        // Reset levels to locked state
        document.querySelectorAll('.level').forEach((level, index) => {
            if (index > 0) { // Skip first level
                level.classList.add('locked');
                const button = level.querySelector('button');
                button.disabled = true;
                button.textContent = 'Locked';
            }
        });
        // Ensure level 1 is unlocked after logout
        const level1 = document.getElementById('level1');
        level1.classList.remove('locked');
        const button1 = level1.querySelector('button');
        button1.disabled = false;
        button1.textContent = 'Start Level 1';
    }

    function updateUserInterface() {
        const userProfile = document.querySelector('.user-profile span');
        if (currentUser) {
            userProfile.textContent = currentUser.name;
            // Save progress to localStorage
            saveProgress();
        } else {
            userProfile.textContent = 'Sign In';
            // Clear saved progress
            localStorage.removeItem('userProgress');
        }
    }

    function saveProgress() {
        if (currentUser) {
            const progress = {
                completedLevels,
                courseProgress,
                timeSpent,
                totalPoints,
                email: currentUser.email
            };
            localStorage.setItem('userProgress', JSON.stringify(progress));
        }
    }

    function loadProgress() {
        if (currentUser) {
            const savedProgress = localStorage.getItem('userProgress');
            if (savedProgress) {
                const progress = JSON.parse(savedProgress);
                if (progress.email === currentUser.email) {
                    completedLevels = progress.completedLevels;
                    courseProgress = progress.courseProgress;
                    timeSpent = progress.timeSpent;
                    totalPoints = progress.totalPoints;

                    // Unlock appropriate levels based on progress
                    for (let i = 1; i <= completedLevels; i++) {
                        const levelId = `level${i}`;
                        const levelElement = document.getElementById(levelId);
                        if (levelElement) {
                            levelElement.classList.remove('locked');
                            const button = levelElement.querySelector('button');
                            if (button) {
                                button.disabled = false;
                                button.textContent = `Start ${levelElement.querySelector('h2').textContent.split(':')[0]}`;
                                button.setAttribute('onclick', `loadLevel('${levelId}')`);
                            }
                        }
                    }
                    if (completedLevels < totalLevels) {
                        unlockNextLevel(`level${completedLevels}`);
                    }
                    updateStats();
                }
            }
        }
    }

    // Function to trigger the congratulations animation
    function showCongratsAnimation() {
        const animationContainer = document.getElementById('congratsAnimation');
        animationContainer.innerHTML = ''; // Clear existing confetti

        const numberOfConfetti = 100;
        for (let i = 0; i < numberOfConfetti; i++) {
            const confetti = document.createElement('div');
            confetti.classList.add('confetti');
            confetti.style.left = `${Math.random() * 100}%`;
            confetti.style.animationDelay = `${Math.random() * 2}s`;
            confetti.style.backgroundColor = getRandomColor(); // Random confetti color
            animationContainer.appendChild(confetti);
        }

        // Remove the animation after it completes
        setTimeout(() => {
            animationContainer.innerHTML = '';
        }, 4000); // Remove after 4 seconds
    }

    // Function to generate a random color for confetti
    function getRandomColor() {
        const letters = '0123456789ABCDEF';
        let color = '#';
        for (let i = 0; i < 6; i++) {
            color += letters[Math.floor(Math.random() * 16)];
        }
        return color;
    }

    function downloadCertificate() {
        const name = document.getElementById('certificateNameToDownload').textContent;
        const date = document.getElementById('certificateDateToDownload').textContent;
        const { jsPDF } = window.jspdf;
        const doc = new jsPDF();

        const pageWidth = doc.internal.pageSize.getWidth();
        const pageHeight = doc.internal.pageSize.getHeight();

        // Border
        doc.setLineWidth(1); // Reduced border thickness
        doc.setDrawColor('#f6d365'); // Solid color border
        doc.rect(15, 15, pageWidth - 30, pageHeight - 30, 'D'); // 'D' for draw (outline)

        // Title
        doc.setFontSize(26);
        doc.setTextColor('#e44d26'); // Orange-red
        doc.setFont('Arial', 'bold');
        const titleText = "Certificate of Completion";
        const titleWidth = doc.getTextWidth(titleText);
        const titleX = (pageWidth - titleWidth) / 2;
        doc.text(titleText, titleX, 40);

        // Presented To
        doc.setFontSize(14);
        doc.setTextColor('#555');
        doc.setFont('Arial', 'italic');
        const presentedText = "This certificate is presented to";
        const presentedWidth = doc.getTextWidth(presentedText);
        const presentedX = (pageWidth - presentedWidth) / 2;
        doc.text(presentedText, presentedX, 60);

        // Name
        doc.setFontSize(20);
        doc.setTextColor('#29abe2'); // Light blue
        doc.setFont('Arial', 'normal');
        const nameText = name;
        const nameWidth = doc.getTextWidth(nameText);
        const nameX = (pageWidth - nameWidth) / 2;
        doc.text(nameText, nameX, 75);

        // For Completion
        doc.setFontSize(14);
        doc.setTextColor('#555');
        doc.setFont('Arial', 'italic');
        const completionText = "For successfully completing the course";
        const completionWidth = doc.getTextWidth(completionText);
        const presentedX2 = (pageWidth - completionWidth) / 2;
        doc.text(completionText, presentedX2, 90);

        // Course Name
        doc.setFontSize(16);
        doc.setTextColor('#8e44ad'); // Purple
        doc.setFont('Arial', 'bold');
        const courseText = "Cybersecurity Learning Course";
        const courseWidth = doc.getTextWidth(courseText);
        const courseX = (pageWidth - courseWidth) / 2;
        doc.text(courseText, courseX, 105);

        // Date
        doc.setFontSize(12);
        doc.setTextColor('#777');
        doc.setFont('Arial', 'normal');
        const dateText = `Date: ${date}`;
        const dateWidth = doc.getTextWidth(dateText);
        const dateX = (pageWidth - dateWidth) / 2;
        doc.text(dateText, dateX, 120);

        doc.save(`Certificate-${name}.pdf`);
    }

    // Function to hide the dashboard and show the home screen
    function goToHome() {
        document.getElementById('home').style.display = 'flex';
        document.querySelector('.nav-bar').style.display = 'none';
        document.querySelector('.dashboard').style.display = 'none';
    }

    // Function to hide the home screen and show the dashboard
    function showDashboard() {
        document.getElementById('home').style.display = 'none';
        document.querySelector('.nav-bar').style.display = 'flex';
        document.querySelector('.dashboard').style.display = 'block';
        openTab('overview'); // Open the overview tab by default
    }

    // Initialize when page loads
    document.addEventListener('DOMContentLoaded', () => {
        // Initially hide the navigation bar and dashboard
        document.querySelector('.nav-bar').style.display = 'none';
        document.querySelector('.dashboard').style.display = 'none';

        initializeProgress();

        // Initially hide levels
        document.querySelector('.levels').style.display = 'none';

        // Add event listener for visibility change
        document.addEventListener('visibilitychange', () => {
            if (document.hidden) {
                // Clear timer when page is hidden
                clearInterval(timerInterval);
            } else {
                // Restart timer when page is visible
                startTimer();
            }
        });

        // Close modals when clicking outside
        window.onclick = (event) => {
            if (event.target.classList.contains('modal')) {
                closeModals();
            }
        };

        // Close button functionality
        document.querySelectorAll('.close').forEach(closeBtn => {
            closeBtn.onclick = closeModals;
        });

        // Sign In Form Submit
        document.getElementById('signInForm').addEventListener('submit', (e) => {
            e.preventDefault();
            const email = document.getElementById('signInEmail').value;
            const password = document.getElementById('signInPassword').value;

            // Here you would typically validate against a backend
            // For demo, we'll just simulate a successful login
            currentUser = { email: email, name: 'User Name' };
            updateUserInterface();
            closeModals();

            // Load progress after successful sign-in
            loadProgress(); // <--- THIS IS THE CRITICAL LINE
        });

        // Sign Up Form Submit
        document.getElementById('signUpForm').addEventListener('submit', (e) => {
            e.preventDefault();
            const name = document.getElementById('signUpName').value;
            const email = document.getElementById('signUpEmail').value;
            const password = document.getElementById('signUpPassword').value;
            const confirmPassword = document.getElementById('confirmPassword').value;

            if (password !== confirmPassword) {
                alert('Passwords do not match!');
                return;
            }

            // Here you would typically send this to a backend
            // For demo, we'll just simulate a successful registration
            currentUser = { name: name, email: email };
            updateUserInterface();
            closeModals();
        });

        // Logout functionality
        document.getElementById('logoutLink').addEventListener('click', (e) => {
            e.preventDefault();
            logout();
        });

        // User profile click handler
        document.querySelector('.user-profile').addEventListener('click', () => {
            if (currentUser) {
                toggleDropdown();
            } else {
                showSignInModal();
            }
        });

        // Close dropdown when clicking outside
        document.addEventListener('click', (e) => {
            if (!e.target.closest('.user-profile') && !e.target.closest('#userDropdown')) {
                document.getElementById('userDropdown').style.display = 'none';
            }
        });

        // Open the overview tab by default
        openTab('overview');
    });

</script>

    
</body>

</html>


