<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>I'm Sorry, My Pookiee Wookiee Bear</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #ffebee;
            font-family: Arial, sans-serif;
            text-align: center;
            overflow: hidden;
            flex-direction: column;
        }
        .message {
            background: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            animation: fadeIn 2s ease-in-out;
        }
        h1 {
            color: #e53935;
            animation: pulse 1.5s infinite alternate;
        }
        p {
            font-size: 18px;
            color: #333;
        }
        .button {
            display: inline-block;
            margin: 15px 10px;
            padding: 10px 20px;
            background: #e53935;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            transition: 0.3s;
            cursor: pointer;
            animation: bounce 1.5s infinite;
        }
        .button:hover {
            background: #d32f2f;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes pulse {
            from { transform: scale(1); }
            to { transform: scale(1.1); }
        }
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-5px); }
        }
        #photo {
            display: none;
            margin-top: 20px;
            width: 300px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            animation: fadeIn 1s ease-in-out;
        }
    </style>
    <script>
        function showPhoto() {
            document.getElementById('photo').style.display = 'block';
        }
        function showMessage() {
            alert("You are my everything, my Pookiee Wookiee Bear! ❤️");
        }
        function showExtraMessage1() {
            alert("Every second with you is a blessing, and I never want to lose you. 💖");
        }
        function showExtraMessage2() {
            alert("You are my heart, my love, my forever. I cherish you more than words can say. 💕");
        }
        function showExtraMessage3() {
            alert("No matter what happens, I choose you, over and over again. ❤️");
        }
        function surpriseEffect() {
            document.body.style.backgroundColor = "#ffcccb";
        }
        function playMusic() {
            let audio = new Audio('https://www.dropbox.com/scl/fi/your_audio_file.mp3?rlkey=your_key&raw=1'); // Replace with actual link to "Aya" by Earl Agustin
            audio.play();
        }
        function showHearts() {
            let heart = document.createElement('div');
            heart.innerHTML = "❤️";
            heart.style.position = 'absolute';
            heart.style.left = Math.random() * window.innerWidth + 'px';
            heart.style.top = Math.random() * window.innerHeight + 'px';
            heart.style.fontSize = '30px';
            document.body.appendChild(heart);
            setTimeout(() => heart.remove(), 2000);
        }
        function startHeartAnimation() {
            setInterval(showHearts, 500);
        }
    </script>
</head>
<body>
    <div class="message">
        <h1>I'm Sorry, My Pookiee Wookiee Bear ❤️</h1>
        <p>Last night may have been tough, but it only made me realize how much I truly love you. Every moment with you is precious, and I never want to take you for granted. You are my sunshine, my safe place, my heart's home. I promise to love you endlessly, to cherish you always, and to fight for us no matter what. I am never tired of you, and I never will be. You mean the world to me, my Pookiee Wookiee Bear. ❤️</p>
        <button class="button" onclick="showPhoto()">Stay With Me</button>
        <button class="button" onclick="showMessage()">Special Message</button>
        <button class="button" onclick="showExtraMessage1()">More Love</button>
        <button class="button" onclick="showExtraMessage2()">Forever Us</button>
        <button class="button" onclick="showExtraMessage3()">Always Yours</button>
        <button class="button" onclick="surpriseEffect()">Surprise Me</button>
        <button class="button" onclick="playMusic()">Play Romantic Music</button>
        <button class="button" onclick="startHeartAnimation()">Shower with Hearts</button>
    </div>
    <img id="photo" src="image.png" alt="Us Together">
</body>
</html>
