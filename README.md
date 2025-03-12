# mi-proyecto-web
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SABANAS S Y E</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="./CSS/STYLE.CSS">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css"> 
    <link rel="shortcut icon" href="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS85iESdFjbexkVxurYxsP4Wyyu1Yr_cVPBAQ&s" type="image/x-icon">
</head>
<body>

    <!-- Barra de navegación -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <div class="container">
            <a href=""><img src="https://png.pngtree.com/png-clipart/20230926/original/pngtree-vector-icon-of-neatly-folded-linens-and-pillows-vector-png-image_12785105.png" alt="" width="100" height="100"></a>
            <h1>SABANAS S & E</h1>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="index.html">Inicio</a></li>
                    <li class="nav-item"><a class="nav-link" href="productos.html">Productos</a></li>
                    <li class="nav-item"><a class="nav-link" href="nosotros.html">Nosotros</a></li>
                    <li class="nav-item"><a class="nav-link" href="contacto.html">Contacto</a></li>
                </ul>
            </div>
            <div class="buscarbox">
                <i class="fa-solid fa-magnifying-glass"></i>
                <input type="text" placeholder="Buscar acá...">
            </div>
            <!-- Botón de usuario que abre el modal -->
            <div id="reguser">
                <a href="#" onclick="mostrarModal()"><i class="fa-solid fa-user"></i></a>
            </div>
        </div>
    </nav>

    <!-- Modal de inicio de sesión -->
    <div id="loginModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="cerrarModal()">&times;</span>
            <h2>Iniciar Sesión</h2>
            <form action="bienvenida.html">
                <input type="text" placeholder="Usuario" required>
                <input type="password" placeholder="Contraseña" required>
                <button type="submit">Ingresar</button>
            </form>
            <p>¿No tienes cuenta? <a href="registro.html">Regístrate aquí</a></p>
        </div>
    </div>

    <!-- Scripts -->
    <script>
        function mostrarModal() {
            document.getElementById("loginModal").style.display = "block";
        }

        function cerrarModal() {
            document.getElementById("loginModal").style.display = "none";
        }

        // Cierra el modal si el usuario hace clic fuera de él
        window.onclick = function(event) {
            var modal = document.getElementById("loginModal");
            if (event.target == modal) {
                modal.style.display = "none";
            }
        }
    </script>


    <!-- Slider de imágenes -->
    <div id="carouselExample" class="carousel slide" data-bs-ride="carousel">
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
        </button>
    </div>

    <!-- Contenido principal -->
    <div class="container mt-5">
        <h2 class="text-center">Bienvenidos a SABANAS S Y E</h2>
        <p class="text-center">
            Tu descanso merece lo mejor, y en SABANAS S Y E estamos aquí para ofrecerte sábanas y cubrelechos de alta calidad con un diseño moderno y elegante. 
            Cada uno de nuestros productos está pensado para brindarte comodidad, estilo y la mejor experiencia de descanso. Explora nuestra colección y descubre cómo transformar tu habitación en un espacio único y acogedor.
        </p>
        <p class="text-center">¡Gracias por visitarnos y ser parte de nuestra comunidad!</p>
    </div>
    <br><br>
    <!-- Seccion de Video -->
    <div class="video-container">
    <h2>Videos de Interes</h2>
    <br><br>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/bhPwYlV0L8k?si=RGS76gCnk8yb7Oic" title="YouTube video player" frameborder="5" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>
    <br><br>
    </aside>
    <!-- Pie de página -->
    <footer id="footer">
        <div class="container text-center">
            <div id="redes">
                <a href="https://www.instagram.com/house.stilo_0814/" target="_blank">
                    <i class="fab fa-instagram"></i>
                </a>
                <a href="https://www.facebook.com/house.stilo/" target="_blank">
                    <i class="fab fa-facebook"></i>
                </a>
                <a href="https://web.whatsapp.com/"><i class="fa-brands fa-whatsapp"></i>
                </a>
                <a href="https://tiktok.com"><i class="fa-brands fa-tiktok"></i>
                </a>
                <a href="https://x.com/?lang=es"><i class="fa-brands fa-x-twitter"></i>
                </a>
            </div>
            <h6>Todos los derechos reservados &copy; 2025 Sara Jiménez</h6>
        </div>
    </footer>

</body>
</html>
