<template>
    <div>
      <!-- Creado por Kimberly -->
      <!-- Mejorado por Arcangel -->
      <!-- Navbar -->
      <div class="container-fluid bg-primary">
        <div class="container">
          <nav class="navbar navbar-expand-lg navbar-dark">
            <div class="container-fluid">
              <a class="navbar-brand" href="#">Inteligencia Artificial</a>
              <button
                class="navbar-toggler"
                type="button"
                data-bs-toggle="collapse"
                data-bs-target="#navbarSupportedContent"
                aria-controls="navbarSupportedContent"
                aria-expanded="false"
                aria-label="Toggle navigation"
              >
                <span class="navbar-toggler-icon"></span>
              </button>
              <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
                  <li class="nav-item">
                    <a class="nav-link active" aria-current="page" href="#">Kimberly</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link" href="#">Angel</a>
                  </li>
                  <li class="nav-item dropdown">
                    <a
                      class="nav-link dropdown-toggle"
                      href="#"
                      id="navbarDropdown"
                      role="button"
                      data-bs-toggle="dropdown"
                      aria-expanded="false"
                    >
                      Antonia
                    </a>
                    <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                      <li><a class="dropdown-item" href="#">ChatGPT</a></li>
                      <li><a class="dropdown-item" href="#">Siri</a></li>
                      <li><a class="dropdown-item" href="#">Meta IA</a></li>
                    </ul>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link btn btn-warning" href="#" tabindex="-1">Arcángel</a>
                  </li>
                </ul>
              </div>
            </div>
          </nav>
        </div>
      </div>
    </div>
    <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-indicators">
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active"
                aria-current="true" aria-label="Slide 1"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1"
                aria-label="Slide 2"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2"
                aria-label="Slide 3"></button>
        </div>
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img src="https://oaxaca.media/wp-content/uploads/2023/04/notaweb_720x332_fotoslimpias_2_1.jpg"
                    class="d-block w-100" alt="Detener a las IA'S">
                <div class="carousel-caption d-none d-md-block">
                    <h5>Detengan a las IA'S</h5>
                    <p>En definitiva, ¡pongamos manos a la obra! Trabajemos juntos para asegurarnos de que las
                        inteligencias artificiales sean nuestras aliadas en lugar de nuestras enemigas.</p>
                </div>
            </div>
            <div class="carousel-item">
                <img src="https://forbes.es/wp-content/uploads/2023/07/robor-ordenador-inteligencia-artificial.jpg"
                    class="d-block w-100" alt="Riesgos de las IA'S">
                <div class="carousel-caption d-none d-md-block">
                    <h5>Riesgos de las IA'S</h5>
                    <p>Es fundamental que la sociedad en su conjunto tome conciencia de la importancia de regular y
                        supervisar el desarrollo de las IA’s, sin caer en el pánico o la paranoia.</p>
                </div>
            </div>
            <div class="carousel-item">
                <img src="https://static.euronews.com/articles/stories/09/00/90/24/1200x675_cmsv2_9db6dfd4-701a-5bb0-9291-d12401e215d9-9009024.jpg"
                    class="d-block w-100" alt="IA DeepSeek">
                <div class="carousel-caption d-none d-md-block">
                    <h5>IA DeepSeek</h5>
                </div>
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions"
            data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Anterior</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions"
            data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Siguiente</span>
        </button>
    </div>
    <div class="container mt-5">
        <div class="row justify-content-center">
            <div class="col-12 col-md-8">
                <h1 class="text-white fw-bold">Conviértete en un experto en programación web sin pasar miles de horas de
                    investigación</h1>
                <ul class="list-group">
                    <li class="list-group-item">Aprende las bases de la programación web</li>
                    <li class="list-group-item">Domina HTML, CSS y JavaScript</li>
                    <li class="list-group-item">Explora frameworks como Bootstrap</li>
                    <li class="list-group-item">Desarrolla proyectos reales</li>
                    <li class="list-group-item">Accede a recursos exclusivos</li>
                </ul>
            </div>
        </div>
    </div>
    <div class="row mt-5 justify-content-center">
        <div class="col-10 col-md-3 mb-4"> <!-- Ajusté el ancho de las columnas -->
            <div class="card text-center text-warning h-100"> <!-- Añadí h-100 para que todas tengan la misma altura -->
                <img class="card-img-top"
                    src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSmtZLqj3PpQtZeNkewOYEtphPdLtDly7PqoQ&s"
                    alt="ChatGPT">
                <div class="card-body d-flex flex-column"> <!-- Flexbox para alinear el contenido -->
                    <h5 class="card-title">ChatGPT</h5>
                    <p class="card-text flex-grow-1"> <!-- Flex-grow para que el texto ocupe el espacio disponible -->
                        Chat GPT es un chatbot basado en el sistema GPT y entrenado para reconocer y mantener
                        conversaciones con las personas. Su función como herramienta basada en inteligencia artificial
                        es interpretar las preguntas que los usuarios le hacen y ofrecer respuestas coherentes y rápidas
                        a cambio.
                    </p>
                    <a href="#" class="btn btn-outline-info mt-auto">Más Información 🔍</a>
                    <!-- mt-auto para alinear el botón abajo -->
                </div>
            </div>
        </div>
        <div class="col-10 col-md-3 mb-4">
            <div class="card text-center text-warning h-100">
                <img class="card-img-top" src="https://electronicaonline.net/wp-content/uploads/2023/05/Siri.webp"
                    alt="Siri">
                <div class="card-body d-flex flex-column">
                    <h5 class="card-title">Siri</h5>
                    <p class="card-text flex-grow-1">
                        Siri es un asistente de voz de Apple que utiliza inteligencia artificial (IA) para interactuar
                        con los usuarios. Siri se basa en tecnologías como el reconocimiento de voz, el procesamiento
                        del lenguaje natural y el aprendizaje automático.
                    </p>
                    <a href="#" class="btn btn-outline-info mt-auto">Más Información 🔍</a>
                </div>
            </div>
        </div>
        <div class="col-10 col-md-3 mb-4">
            <div class="card text-center text-warning h-100">
                <img class="card-img-top"
                    src="https://pollingersocial.co.uk/wp-content/uploads/2024/04/LLaMA-meta-ai-model-jpeg.webp"
                    alt="Meta IA">
                <div class="card-body d-flex flex-column">
                    <h5 class="card-title">Meta IA</h5>
                    <p class="card-text flex-grow-1">
                        Meta AI es un laboratorio de investigación que desarrolla inteligencia artificial (IA) y
                        realidad aumentada y artificial. Su objetivo es generar conocimiento para la comunidad de IA.
                    </p>
                    <a href="#" class="btn btn-outline-info mt-auto">Más Información 🔍</a>
                </div>
            </div>
        </div>
    </div>
    <div class="row mt-5 justify-content-center"> <!-- Centrar horizontalmente -->
        <div class="col-12 col-md-8 text-center"> <!-- Centrar el contenido y ajustar el ancho -->
            <h2 class="fw-bold" style="color: #ffffffe8;">Explicación sobre las IA’S</h2>
            <!-- Título centrado y en negritas -->
            <p class="text-white"> <!-- Texto centrado y color blanco -->
                <strong>La inteligencia artificial ha revolucionado la manera en que interactuamos con la
                    tecnología.</strong> Desde asistentes virtuales hasta sistemas de recomendación y automatización,
                las IA están presentes en múltiples sectores como la salud, la educación y el entretenimiento. Conoce
                cómo funcionan y su impacto en nuestra vida cotidiana.
            </p>
            <p class="text-white"> <!-- Texto centrado y color blanco -->
                <strong>¿Estamos listos para vivir en un mundo donde la inteligencia artificial tome decisiones por
                    nosotros?</strong> Descubre su impacto y forma parte del futuro tecnológico.
            </p>
            <div class="mt-4"> <!-- Centrar los botones y añadir margen superior -->
                <button type="button" class="btn btn-primary">Más info</button>
            </div>
        </div>
    </div>


    <!-- Creado por Antonia Maria -->
     <!-- Actualizado por Arcangel y agregación de botones -->
    <!-- Incluir Bootstrap Icons en el <head> -->
    <!-- Formulario de Contacto con Iconos -->
    <div class="row justify-content-center mt-5 pb-5">
        <div class="col-12 col-md-7">
            <h2 class="fw-bold text-white">Envíanos un mensaje</h2> <!-- Título en negritas y color blanco -->
            <form>
                <!-- Campo de Nombre con Icono -->
                <div class="mb-3 input-group">
                    <span class="input-group-text">
                        <i class="bi bi-person-fill"></i> <!-- Icono de persona -->
                    </span>
                    <input type="text" class="form-control" placeholder="Nombre">
                </div>

                <!-- Campo de Correo Electrónico con Icono -->
                <div class="mb-3 input-group">
                    <span class="input-group-text">
                        <i class="bi bi-envelope-fill"></i> <!-- Icono de correo -->
                    </span>
                    <input type="email" class="form-control" placeholder="Correo electrónico">
                </div>

                <!-- Campo de Mensaje con Icono -->
                <div class="mb-3 input-group">
                    <span class="input-group-text">
                        <i class="bi bi-chat-left-text-fill"></i> <!-- Icono de mensaje -->
                    </span>
                    <textarea class="form-control" rows="5" placeholder="Mensaje"></textarea>
                </div>

                <!-- Botón de Enviar con Icono -->
                <div class="d-grid">
                    <button type="submit" class="btn btn-primary">
                        <i class="bi bi-send-fill me-2"></i> <!-- Icono de enviar -->
                        Enviar
                    </button>
                </div>
            </form>
        </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "NavbarComponent",
  };
  </script>
  
  <style scoped>
  /* Puedes agregar estilos personalizados aquí */
  </style>
  <style>
  body {
      background: linear-gradient(135deg, #052f47 0%, #0e0e0e 100%);
      background-attachment: fixed;
      background-size: cover;
  }

  .carousel-item img {
      height: 600px;
      object-fit: cover;
  }

  .card {
      height: 500px;
      background-color: #0A1F44;
  }

  .card-img-top {
      height: 200px;
      object-fit: cover;
  }

  .list-group-item:hover {
      background-color: #007bff;
      color: white;
      transform: scale(1.05);
      transition: all 0.3s ease;
      cursor: pointer;
  }
</style>