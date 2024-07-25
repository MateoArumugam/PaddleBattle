<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>|Mario's Paddle Battle||Mateo Arumugam|</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="video-background">
        <video autoplay muted loop poster="your-background.jpg" id="bgvid">
            <source src="background.mp4" type="video/mp4">
        </video>
    </div>

    <audio id="bgAudio" loop>
        <source src="background.mp3" type="audio/mp3">
        Your browser does not support the audio element.
    </audio>

    <audio id="ballHitAudio">
        <source src="ballhit.mp3" type="audio/mp3">
        Your browser does not support the audio element.
    </audio>
    
    <audio id="scoreAudio">
        <source src="score.mp3" type="audio/mp3">
        Your browser does not support the audio element.
    </audio>
    
    <audio id="lostAudio">
        <source src="lost.mp3" type="audio/mp3">
        Your browser does not support the audio element.
    </audio>
    
    <audio id="winAudio">
        <source src="win.mp3" type="audio/mp3">
        Your browser does not support the audio element.
    </audio>
    

    <div class="game-container">
        <h1 class="mario-title">Mario's Paddle Battle</h1>
        <canvas id="gameCanvas"></canvas>
        <p>Control the left player by using up and down arrow keys</p>
    </div>
    
    <script>
        document.addEventListener('click', function() {
            const audio = document.getElementById('bgAudio');
            audio.play().catch(error => {
                console.log('Playback prevented: ' + error);
            });
        }, { once: true }); // Ensures the event listener is called only once
    </script>
    <script src="script.js"></script>
</body>
</html>



