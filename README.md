<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Mi Amor 💖</title>
    <style>
        body { font-family: 'Georgia', serif; background: linear-gradient(to right, #ffe0ec, #fff); text-align: center; margin: 0; padding: 0; }
        .carta { background: white; max-width: 500px; margin: 40px auto; padding: 25px; border-radius: 15px; box-shadow: 0 10px 30px rgba(0,0,0,0.2); }
        h1 { color: #e91e63; font-size: 1.8em; }
        p { font-size: 1.1em; color: #444; line-height: 1.6; }
        .heart { font-size: 60px; animation: latido 1.5s infinite; }
        @keyframes latido { 0% {transform: scale(1);} 50% {transform: scale(1.2);} 100% {transform: scale(1);} }
        /* Contenedor para que el video se vea bien en celular */
        .video-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; margin-top: 20px; border-radius: 10px; }
        .video-container iframe { position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: none; }
        .btn { margin-top: 15px; padding: 12px 25px; background: #e91e63; color: white; border: none; border-radius: 10px; cursor: pointer; font-size: 1em; font-weight: bold; }
    </style>
</head>
<body>

    <div class="carta">
        <h1>Para mi amor eterno 💕</h1>
        <p>
            Mi amor,<br><br>
            Desde que llegaste a mi vida, todo es más bonito, más especial… más tú.
            Gracias por existir y por hacerme tan feliz.<br><br>
            Te amo hoy, mañana y siempre. ❤️
        </p>

        <div class="heart">💖</div>

        <div class="video-container">
            <iframe 
                id="video"
                src="https://www.youtube.com/embed/G5tlJnxFJF8?autoplay=1&mute=1&enablejsapi=1" 
                allow="autoplay; encrypted-media" 
                allowfullscreen>
            </iframe>
        </div>

        <br>
        <button class="btn" onclick="activarSonido()">🔊 Toca para escuchar nuestra canción</button>
    </div>

    <script>
        function activarSonido() {
            var iframe = document.getElementById("video");
            // Al hacer clic, recargamos el video con sonido (mute=0)
            iframe.src = "https://www.youtube.com/embed/G5tlJnxFJF8?autoplay=1&mute=0";
        }
    </script>

</body>
</html>
