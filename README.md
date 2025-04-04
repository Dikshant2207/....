<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Anniversary, My Love 💖</title>
    
    <!-- Google Fonts: Poppins & Dancing Script -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Dancing+Script:wght@700&display=swap" rel="stylesheet">

    <style>
        /* Animated Gradient Background */
        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        body {
            font-family: 'Poppins', sans-serif;
            text-align: center;
            background: linear-gradient(45deg, #ff758c, #ff7eb3, #ff758c);
            background-size: 300% 300%;
            animation: gradientBG 6s infinite alternate ease-in-out;
            color: white;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        /* Title Animation */
        @keyframes fadeInScale {
            0% { opacity: 0; transform: scale(0.8); }
            100% { opacity: 1; transform: scale(1); }
        }

        h1 {
            font-size: 2em;
            font-weight: 800;
            text-shadow: 2px 2px 10px rgba(255, 255, 255, 0.6);
            animation: fadeInScale 1.5s ease-in-out;
        }

        .container, #password-container {
            display: none;
            width: 90%;
            max-width: 400px;
            padding: 15px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 15px;
            box-shadow: 0px 0px 10px rgba(255, 255, 255, 0.4);
            text-align: center;
        }

        /* Readable Message Font */
        .message {
            font-size: 1.2em;
            line-height: 1.6;
            padding: 15px;
            border-radius: 10px;
            text-align: center;
            font-family: 'Poppins', sans-serif;
            background: rgba(255, 255, 255, 0.3);
            box-shadow: 0px 0px 8px rgba(255, 255, 255, 0.4);
        }

        /* Button Styling */
        .button {
            background: #ff4081;
            color: white;
            font-size: 1em;
            padding: 10px 18px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            margin-top: 15px;
            transition: 0.3s;
            box-shadow: 0px 4px 10px rgba(255, 64, 129, 0.6);
        }

        /* Button Hover Effect */
        .button:hover {
            background: #d63384;
            transform: scale(1.05);
        }

        /* Secret Letter - Now Opens Instantly */
        .hidden-message {
            display: none;
            font-size: 1.2em; /* Matched font size */
            margin-top: 15px;
            padding: 10px;
            border-radius: 8px;
            background: rgba(255, 255, 255, 0.3);
            box-shadow: 0px 0px 8px rgba(255, 255, 255, 0.4);
            text-align: center;
            font-family: 'Poppins', sans-serif;
        }

        /* Password Input Styling */
        .password-input {
            font-size: 1em;
            padding: 8px;
            border-radius: 5px;
            border: none;
            text-align: center;
            width: 80%;
        }
    </style>
</head>
<body>

    <!-- Password Input -->
    <div id="password-container">
        <h1>Enter Password to Unlock 💖</h1>
        <input type="password" id="password" class="password-input" placeholder="Enter Password">
        <button class="button" onclick="checkPassword()">Unlock</button>
        <p id="error-message" style="color: yellow; display: none;">Wrong Password! Try Again. 🔐</p>
    </div>

    <!-- First Open Button (Hidden Initially) -->
    <button id="open-button" class="button" style="display: none;" onclick="openSurprise()">🌹 This Is For You 💖</button>

    <div id="content" class="container">
        <h1>Happy Anniversary, My Love! 💖</h1>

        <div class="message">
            😊❤ It's been 1 year, and I promise I will always be yours.  
            I love you, my love. You are my happiness, my dream.  
            My goal is to make you my wife. 💍  
            Your smile is my power, and your eyes never lie to me.  
            You make my life magical and full of love.  
            🦋🐼 Thank you for coming into my life. 🐼🦋  
            I promise to always stay loyal to you. 💖  
            I LOVE YOU SO MUCH, MY DEAR BUTTERFLY, MERI PYAARI JALEBI! 😊💖  
        </div>

        <!-- Secret Love Letter Button -->
        <button class="button" onclick="showLoveLetter()">💌 Tap for a Secret Love Letter</button>

        <!-- Hidden Love Letter (Now Appears Instantly) -->
        <div id="love-letter" class="hidden-message">
            Happy anniversary, Shraddhuuu!  
            Mi nehmi tuzya sobt rahil. Ata ek varsha zaly ahe, ani pudhe pan rahaycha!  
            Hasn, radn, sagl je kahi asel, tuzya sobt jagaycha!  
            Bala, tuzya vr ata jase prem karto, tya peksha jast prem karycha!  
            Life madhe je kahi chadh-utaar astil, te tuzya sobt jagayche!  
            Tuzya peksha changla koni shodhnyachi garaj nahi, tuzya peksha ajun mala koni nakoy.  
            I really love you so much, my future wife. 💖  
        </div>
    </div>

    <script>
        document.getElementById('password-container').style.display = 'block';

        function checkPassword() {
            let inputPassword = document.getElementById('password').value;
            if (inputPassword === "12062207") {
                document.getElementById('password-container').style.display = 'none';
                document.getElementById('open-button').style.display = 'block';
            } else {
                document.getElementById('error-message').style.display = 'block';
            }
        }

        function openSurprise() {
            document.getElementById('content').style.display = 'block';
            document.getElementById('open-button').style.display = 'none';
        }

        function showLoveLetter() {
            document.getElementById('love-letter').style.display = 'block';
        }
    </script>

</body>
</html>
