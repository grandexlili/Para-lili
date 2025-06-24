# Para Lili:
Página especial para lili

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Lili</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom, #f8baff, #ffe6f7);
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Arial', sans-serif;
            color: #333;
            text-align: center;
        }
        .container {
            position: relative;
            width: 100%;
            max-width: 600px;
        }
        .message {
            font-size: 1.5em;
            margin: 20px;
        }
        .star {
            position: absolute;
            top: 5%;
            right: 10%;
            font-size: 2em;
            color: #fff;
            text-shadow: 0 0 10px #ff9, 0 0 20px #ff6;
        }
        .firefly {
            position: absolute;
            bottom: 10%;
            left: 50%;
            transform: translateX(-50%);
            background: yellow;
            border-radius: 50%;
            width: 20px;
            height: 20px;
            box-shadow: 0 0 10px yellow;
            cursor: pointer;
        }
        .photo {
            display: none;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: rgba(0, 0, 0, 0.8);
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.5);
        }
        .photo img {
            max-width: 100%;
            border-radius: 10px;
        }
        .close {
            position: absolute;
            top: 10px;
            right: 10px;
            font-size: 1.5em;
            color: white;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="star">★</div>
        <p class="message">Lili, me gustas mucho, y no vas a dejar de gustarme ni un poquito.</p>
        <div class="firefly" onclick="showPhoto()"></div>
        <div class="photo" id="photoPopup">
            <span class="close" onclick="closePhoto()">✖</span>
            <img src="photo.jpg" alt="Nosotros">
            <audio controls autoplay loop>
                <source src="amor_de_cine.mp3" type="audio/mpeg">
                Tu navegador no soporta el reproductor de audio.
            </audio>
            <p>Te amo</p>
        </div>
    </div>

    <script>
        function showPhoto() {
            document.getElementById('photoPopup').style.display = 'block';
        }
        function closePhoto() {
            document.getElementById('photoPopup').style.display = 'none';
        }
    </script>
</body>
</html>
