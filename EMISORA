<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fuxion Stereo</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #121212;
            color: white;
        }
        #player-container {
            margin-top: 50px;
        }
        .social-links a {
            margin: 10px;
            color: white;
            text-decoration: none;
        }
    </style>
</head>
<body>
    <h1>Bienvenidos a Fuxion Stereo</h1>
    <div id="player-container">
        <audio id="radio" autoplay controls>
            <source src="https://stream-169.zeno.fm/vz19v9fwdzzuv?zt=eyJhbGciOiJIUzI1NiJ9.eyJzdHJlYW0iOiJ2ejE5djlmd2R6enV2IiwiaG9zdCI6InN0cmVhbS0xNjkuemVuby5mbSIsInJ0dGwiOjUsImp0aSI6IlFiRmhRaUJpUVJXbFdEZVNZck9FY3ciLCJpYXQiOjE3NDM0NjcxMzQsImV4cCI6MTc0MzQ2NzE5NH0.61EH5SmB2aiooxYX3cXcf_DLS3yQZdeFSTmEHrm9s4U&adtonosListenerId=01JQ2DP4HBNAWP1853EZ07NTM4" type="audio/mpeg">
            Tu navegador no soporta el audio en streaming.
        </audio>
    </div>
    <h2>Desde dónde nos escuchan:</h2>
    <p id="location">Cargando...</p>
    <div class="social-links">
        <a href="https://facebook.com" target="_blank">Facebook</a>
        <a href="https://instagram.com" target="_blank">Instagram</a>
        <a href="https://twitter.com" target="_blank">Twitter</a>
    </div>
    <script>
        async function getLocation() {
            try {
                let response = await fetch('https://ipapi.co/json/');
                let data = await response.json();
                document.getElementById("location").innerText = `Escuchando desde: ${data.city}, ${data.country_name}`;
            } catch (error) {
                document.getElementById("location").innerText = "No se pudo obtener la ubicación";
            }
        }
        getLocation();
    </script>
</body>
</html>
