<!DOCTYPE html>
<html>
<head>
    <title>Happy Valentine's Day My Love ❤️</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(to right, #ff758c, #ff7eb3);
            font-family: 'Segoe UI', sans-serif;
            text-align: center;
            color: white;
        }

        .container {
            padding: 30px;
        }

        h1 {
            font-size: 45px;
            margin-top: 40px;
            animation: glow 2s infinite alternate;
        }

        p {
            font-size: 20px;
            max-width: 900px;
            margin: auto;
            line-height: 1.6;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin-top: 40px;
            padding: 20px;
        }

        .gallery img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.3);
            transition: transform 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.05);
        }

        .btn {
            margin-top: 20px;
            padding: 15px 30px;
            font-size: 18px;
            border: none;
            border-radius: 30px;
            background-color: white;
            color: #ff4b7d;
            cursor: pointer;
            transition: 0.3s;
        }

        .btn:hover {
            background-color: #ffe6f0;
        }

        .hidden-message {
            display: none;
            margin-top: 30px;
            font-size: 24px;
            animation: fadeIn 2s forwards;
        }

        @keyframes glow {
            from { text-shadow: 0 0 10px white; }
            to { text-shadow: 0 0 20px #ffdde1; }
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
    </style>
</head>
<body>

<div class="container">
    <h1>Happy Valentine's Day My Love ❤️</h1>

    <p>
        To my beautiful wife,<br><br>
        Every moment with you is a blessing.  
        These 20 beautiful memories of us will always stay in my heart.
    </p>

    <!-- 20 Photo Gallery -->
    <div class="gallery">
        <img src="1.jpeg" alt="Memory 1">
        <img src="2.jpeg" alt="Memory 2">
        <img src="3.jpeg" alt="Memory 3">
        <img src="4.jpeg" alt="Memory 4">
        <img src="5.jpeg" alt="Memory 5">
        <img src="6.jpeg" alt="Memory 6">
        <img src="7.jpeg" alt="Memory 7">
        <img src="8.jpeg" alt="Memory 8">
        <img src="9.jpeg" alt="Memory 9">
        <img src="10.jpeg" alt="Memory 10">
        <img src="11.jpeg" alt="Memory 11">
        <img src="12.jpeg" alt="Memory 12">
        <img src="13.jpeg" alt="Memory 13">
        <img src="14.jpeg" alt="Memory 14">
        <img src="15.jpeg" alt="Memory 15">
        <img src="16.jpeg" alt="Memory 16">
        <img src="17.jpeg" alt="Memory 17">
        <img src="18.jpeg" alt="Memory 18">
        <img src="19.jpeg" alt="Memory 19">
        <img src="20.jpeg" alt="Memory 20">
    </div>

    <!-- Background Music -->
    <audio id="bgMusic" autoplay loop>
        <source src="love_song.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>

    <!-- Music Control Button -->
    <button class="btn" onclick="toggleMusic()">🎵 Play/Pause Music</button>

    <!-- Surprise Button -->
    <button class="btn" onclick="showMessage()">Click for Surprise 🎁</button>

    <div class="hidden-message" id="surprise">
        I will love you today, tomorrow, and forever.<br><br>
        Forever Yours,<br>
        <strong>My Dear ❤️</strong>
    </div>
</div>

<script>
    // Show hidden surprise message
    function showMessage() {
        document.getElementById("surprise").style.display = "block";
    }

    // Play/Pause background music
    function toggleMusic() {
        var music = document.getElementById("bgMusic");
        if (music.paused) {
            music.play();
        } else {
            music.pause();
        }
    }
</script>

</body>
</html>
