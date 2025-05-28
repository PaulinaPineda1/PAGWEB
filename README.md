<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width,initial-scale=1.0">
    <title>REALIDAD VIRTUAL</title>
    <style>
        .title-row {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 1.2rem;
        }
        .title-img {
            width: 48px;
            height: 48px;
            object-fit: contain;
            border-radius: 50%;
            box-shadow: 0 2px 8px #43cea299;
            background: #fff2;
        }
        @media (max-width: 600px) {
            .title-img{
                width: 32px;
                height: 32px;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700;400&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            font-family: 'Montserrat', Arial, sans-serif;
            background: linear-gradient(135deg, #0f0c29 0%, #302b63 50%, #ff0080 100%);
            color: #fff;
            min-height: 100vh;
        }
        
        * {
            box-sizing: border-box;
            transition: all 0.3s ease;
        }
        header {
            text-align: center;
            padding: 2rem 1rem 0.5rem 1rem;
        }
        h1 {
            font-size: 3rem;
            letter-spacing: 2px;
            margin: 0;
            background: linear-gradient(90deg, #a18cd1, #fbc2eb, #43cea2, #185a9d);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        .subtitle {
            font-size: 1.1rem;
            color: #bdbdbd;
            margin-top: 0.5rem;
            letter-spacing: 1px;
        }
        .main-content {
            display: flex;
            justify-content: center;
            align-items: flex-start;
            gap: 2rem;
            padding: 2rem 5vw 1rem 5vw;
            flex-wrap: wrap;
        }
        .info-box {
            background: rgba(40, 20, 60, 0.85);
            border-radius: 1.5rem;
            box-shadow: 0 4px 32px 0 rgba(120,0,120,0.2);
            padding: 2rem;
            max-width: 400px;
            min-width: 280px;
            flex: 1 1 320px;
        }
        .info-box h2 {
            font-size: 1.5rem;
            color: #c471f5;
            margin-bottom: 1rem;
        }
        .info-box p {
            font-size: 1.1rem;
            color: #e0e0e0;
            line-height: 1.6;
        }
        .oculus-image {
            flex: 1 1 320px;
            display: flex;
            align-items: center;
            justify-content: center;
            min-width: 280px;
            position: relative;
        }
        .oculus-image img {
            width: 340px;
            max-width: 100%;
            filter: drop-shadow(0 8px 32px #a18cd1aa);
            border-radius: 2rem;
            animation: float 3s ease-in-out infinite;
            background: linear-gradient(135deg, #a18cd1 0%, #fbc2eb 100%);
            padding: 1rem;
        }
        @keyframes float {
            0%, 100% { transform: translateY(0);}
            50% { transform: translateY(-20px);}
        }
        .collage-section {
            margin: 2rem auto 1rem auto;
            max-width: 900px;
            display: flex;
            gap: 1rem;
            flex-wrap: wrap;
            justify-content: center;
        }
        .collage-section img {
            width: 180px;
            height: 120px;
            object-fit: cover;
            border-radius: 1rem;
            box-shadow: 0 2px 16px #43cea299;
            border: 2px solid #302b63;
            background: #1a1a2e;
        }
        .minigames-section {
            background: rgba(30, 10, 40, 0.7);
            border-radius: 1.5rem;
            margin: 2rem auto 2rem auto;
            max-width: 900px;
            padding: 2rem;
            box-shadow: 0 2px 24px #ff008055;
            text-align: center;
        }
        .minigames-section h3 {
            color: #43cea2;
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }
        .minigames-placeholder {
            color: #bdbdbd;
            font-size: 1rem;
            margin-top: 1rem;
        }
        @media (max-width: 900px) {
            .main-content {
                flex-direction: column;
                align-items: stretch;
            }
            .oculus-image, .info-box {
                max-width: 100%;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>REALIDAD VIRTUAL</h1>
        <div class="subtitle">CECyTECH #11, CIUDAD DEL CONOCIMIENTO</div>
    </header>
    <section class="main-content">
        <div class="info-box">
            <h2>¿Qué es la Realidad Virtual?</h2>
            <p>
                La <strong></strong>Piensa en la realidad virtual como un mundo mágico dentro de una computadora donde puedes jugar, explorar y sentir que estás en otro lugar sin moverte de donde estás. Es como si te pusieras un visor especial y, ¡pum!, de repente estás en una montaña, en el espacio o en un videojuego súper divertido.
            </p>
            <h2>Oculus Quest</h2>
            <p>
                <strong></strong>Los Oculus Quest son unos lentes especiales que te permiten entrar en estos mundos mágicos. Son como unas gafas gigantes con pantallas adentro que te muestran todo a tu alrededor como si estuvieras ahí de verdad. Además, puedes mover tus manos y caminar para interactuar con lo que ves. Es como jugar en un sueño, pero despierto. ¿Te gustaría probarlo?
            </p>
        </div>
        <div class="survey-box" style="background:rgba(60,30,80,0.85); border-radius:1.5rem; box-shadow:0 2px 16px #43cea299; padding:1.5rem; max-width:350px; min-width:220px; margin-top:1.5rem; color:#fff;">
            <form id="stem-survey">
                <h3 style="color:#43cea2; font-size:1.1rem; margin-bottom:1rem;">Encuesta rápida STEM</h3>
                <div style="margin-bottom:1rem;">
                    <label style="font-weight:600;">¿En tu escuela hay actividades STEM?</label><br>
                    <input type="radio" name="q1" value="muchas" required> Sí, muchas.<br>
                    <input type="radio" name="q1" value="pocas"> Sí, pocas.<br>
                    <input type="radio" name="q1" value="no"> No hay.<br>
                    <input type="radio" name="q1" value="nose"> No sé.
                </div>
                <div style="margin-bottom:1rem;">
                    <label style="font-weight:600;">¿Conoces a alguien en STEM en tu familia/comunidad?</label><br>
                    <input type="radio" name="q2" value="varias" required> Sí, varias personas.<br>
                    <input type="radio" name="q2" value="una"> Sí, una persona.<br>
                    <input type="radio" name="q2" value="nadie"> No conozco a nadie.<br>
                    <input type="radio" name="q2" value="nose"> No sé.
                </div>
                <div style="margin-bottom:1rem;">
                    <label style="font-weight:600;">¿Tu familia te anima a aprender STEM?</label><br>
                    <input type="radio" name="q3" value="siempre" required> Sí, siempre.<br>
                    <input type="radio" name="q3" value="aveces"> A veces.<br>
                    <input type="radio" name="q3" value="no"> No.<br>
                    <input type="radio" name="q3" value="nose"> No sé.
                </div>
                <div style="margin-bottom:1rem;">
                    <label style="font-weight:600;">¿Has participado en actividades STEM fuera de la escuela?</label><br>
                    <input type="radio" name="q4" value="varias" required> Sí, varias.<br>
                    <input type="radio" name="q4" value="una"> Sí, una.<br>
                    <input type="radio" name="q4" value="no"> No.<br>
                    <input type="radio" name="q4" value="nose"> No sé.
                </div>
                <div style="margin-bottom:1rem;">
                    <label style="font-weight:600;">¿Crees que las carreras STEM son importantes para el futuro?</label><br>
                    <input type="radio" name="q5" value="muy" required> Sí, muy importantes.<br>
                    <input type="radio" name="q5" value="noestoyseguro"> Sí, pero no estoy seguro.<br>
                    <input type="radio" name="q5" value="noimportan"> No son importantes.<br>
                    <input type="radio" name="q5" value="nose"> No sé.
                </div>
                <button type="submit" style="background:#43cea2; color:#222; border:none; border-radius:0.7rem; padding:0.5rem 1.2rem; font-size:1rem; cursor:pointer; margin-top:0.5rem;">Enviar</button>
                <div id="survey-thanks" style="display:none; color:#43cea2; margin-top:1rem; font-weight:600;">¡Gracias por responder!</div>
            </form>
            <script>
                document.getElementById('stem-survey').addEventListener('submit', function(e){
                    e.preventDefault();
                    document.getElementById('survey-thanks').style.display = 'block';
                });
            </script>
        </div>
        </div>
        <div class="oculus-image">
            <img src="Meta-Quest-3-Gear-Roundup (1).webp" alt="Oculus Quest 3">
        </div>
        </section>
        <section class="photo-library-section" style="margin:2rem auto 1rem auto; max-width:900px; text-align:center;">
            <h3 style="color:#43cea2; margin-bottom:1rem;">NUESTRO APORTE A LA COMUNIDAD</h3>
            <button id="ver-mas-btn" style="background:#43cea2; color:#222; border:none; border-radius:0.7rem; padding:0.5rem 1.2rem; font-size:1rem; cursor:pointer; margin-bottom:1.2rem;">Ver más</button>
            <script>
const imagenesExtra = [
    { src: "WhatsApp Image 2025-05-26 at 1.36.59 PM.jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 1.36.59 PM (7).jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 1.36.59 PM (5).jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 1.36.59 PM (4).jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 1.36.59 PM (3).jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 1.36.59 PM (1).jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 1.33.22 PM.jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 1.33.22 PM (2).jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 1.36.59 PM.jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 10.22.26 PM.jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 10.22.26 PM (1).jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 10.22.25 PM.jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 10.22.25 PM (4).jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 10.22.25 PM (3).jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 10.22.25 PM (2).jpeg", alt: "VR" },
    { src: "WhatsApp Image 2025-05-26 at 10.22.25 PM (1).jpeg", alt: "VR" },
]

            // Script para manejar el botón "Ver más" y cargar imágenes adicionales
                let verMasClickeado = false;
                document.getElementById('ver-mas-btn').addEventListener('click', function() {
                    if (verMasClickeado) return;
                    const contenedor = document.querySelector('.photo-thumbnails');
                    imagenesExtra.forEach(function(imgObj) {
                        const img = document.createElement('img');
                        img.src = imgObj.src;
                        img.alt = imgObj.alt;
                        img.className = "photo-thumb";
                        img.style = "width:120px; height:80px; object-fit:cover; border-radius:0.7rem; cursor:pointer;";
                        img.addEventListener('click', function() {
                            document.getElementById('modal-img').src = this.src;
                            document.getElementById('photo-modal').style.display = 'flex';
                        });
                        contenedor.appendChild(img);
                    });
                    verMasClickeado = true;
                    this.style.display = 'none';
                });
            </script>
            <div class="photo-thumbnails" style="display:flex; flex-wrap:wrap; gap:1rem; justify-content:center;">
                <img src="WhatsApp Image 2025-05-26 at 1.32.20 PM.jpeg" alt="VR" class="photo-thumb" style="width:120px; height:80px; object-fit:cover; border-radius:0.7rem; cursor:pointer;">
                <img src="WhatsApp Image 2025-05-26 at 1.32.19 PM.jpeg" alt="VR" class="photo-thumb" style="width:120px; height:80px; object-fit:cover; border-radius:0.7rem; cursor:pointer;">
                <img src="WhatsApp Image 2025-05-26 at 1.32.19 PM (6).jpeg" alt="VR" class="photo-thumb" style="width:120px; height:80px; object-fit:cover; border-radius:0.7rem; cursor:pointer;">
                <img src="WhatsApp Image 2025-05-26 at 1.32.19 PM (5).jpeg" alt="VR" class="photo-thumb" style="width:120px; height:80px; object-fit:cover; border-radius:0.7rem; cursor:pointer;">
                <img src="WhatsApp Image 2025-05-26 at 1.32.19 PM (4).jpeg" alt="VR" class="photo-thumb" style="width:120px; height:80px; object-fit:cover; border-radius:0.7rem; cursor:pointer;">
                <img src="WhatsApp Image 2025-05-26 at 1.32.19 PM (3).jpeg" alt="VR" class="photo-thumb" style="width:120px; height:80px; object-fit:cover; border-radius:0.7rem; cursor:pointer;">
                <img src="WhatsApp Image 2025-05-26 at 1.32.19 PM (2).jpeg" alt="VR" class="photo-thumb" style="width:120px; height:80px; object-fit:cover; border-radius:0.7rem; cursor:pointer;">
                <img src="WhatsApp Image 2025-05-26 at 1.32.19 PM (1).jpeg" alt="VR" class="photo-thumb" style="width:120px; height:80px; object-fit:cover; border-radius:0.7rem; cursor:pointer;">
            </div>
            <div id="photo-modal" style="display:none; position:fixed; top:0; left:0; width:100vw; height:100vh; background:rgba(0,0,0,0.85); align-items:center; justify-content:center; z-index:1000;">
                <img id="modal-img" src="" alt="Foto VR" style="max-width:90vw; max-height:80vh; border-radius:1rem; box-shadow:0 2px 32px #43cea299;">
            </div>
        </section>
        <script>
            document.querySelectorAll('.photo-thumb').forEach(function(img) {
                img.addEventListener('click', function() {
                    document.getElementById('modal-img').src = this.src;
                    document.getElementById('photo-modal').style.display = 'flex';
                });
            });
            document.getElementById('photo-modal').addEventListener('click', function(e) {
                if (e.target === this) {
                    this.style.display = 'none';
                    document.getElementById('modal-img').src = '';
                }
            });
        </script>
    </section>
    <section class="minigames-section">
        <h3>Minijuegos de Realidad Virtual</h3>
        <div class="minigames-placeholder">
            minijuegos interactivos 
        </div>
        <div class="mascota-container" style="position:fixed; right:0; bottom:0; z-index:1200; pointer-events:none;"></div>
            <img src="ajolote con oculus.png" alt="Mascota VR" class="mascota-img" style="width:110px; height:auto; animation:float-mascota 3s ease-in-out infinite; background:none; margin:0; padding:0; border:none; position:fixed; right:0; bottom:0; z-index:1200; pointer-events:none;">
        </div>
        <style>
            @keyframes float-mascota {
            0%, 100% { transform: translateY(0);}
            50% { transform: translateY(-12px);}
            }
        </style>
        <div style="text-align:center; margin-top:2rem; color:#fff; font-size:1.1rem;">
            La curiosidad construye el futuro: explora, innova y transforma el mundo con ciencia y tecnología.🚀🔬
        </div>
    </div>
     <div style="text-align:center; color:#bdbdbd; margin:2rem 0 1rem 0; font-size:1rem;">
        <p>Desarrollado por el equipo de CECyTECH #11, Ciudad del Conocimiento</p>
        <p>© 2025 Todos los derechos reservados</p>
</body>
</html>
