<template>
<div class="card p-4 mb-3" style="width: 80rem; text-align: center;">
      <div class="card-body">
        <!-- Primera fila con 2 tarjetas -->
        <div class="row row-cols-1 row-cols-md-2 g-3 mb-3">
          <div class="col" v-for="(image, index) in images.slice(0, 2)" :key="index">
            <div class="card h-100">
              <div class="card-header text-white" style="background-color: rgb(0, 136, 143);">
                <h6 class="text-center">CARDS</h6>
              </div>
              <div class="card-body text-center">
                <img :src="image.src" class="card-img-top rounded-circle mx-auto mt-3" style="width: 150px; height: 150px;" alt="Imagen">
                <p style="font-style:italic;">{{ image.text }}</p>
                <a href="#" class="btn btn-primary">Botón</a>
              </div>
            </div>
          </div>
        </div>
        <!-- Segunda fila con 3 tarjetas -->
        <div class="row row-cols-1 row-cols-md-3 g-3">
          <div class="col" v-for="(image, index) in images.slice(2, 5)" :key="index">
            <div class="card h-100">
              <div class="card-header text-white" style="background-color: rgb(0, 136, 143);">
                <h6 class="text-center">CARDS</h6>
              </div>
              <div class="card-body text-center">
                <img :src="image.src" class="card-img-top rounded-circle mx-auto mt-3" style="width: 150px; height: 150px;" alt="Imagen">
                <p style="font-style:italic;">{{ image.text }}</p>
                <a href="#" class="btn btn-primary">Botón</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
</template>


<script>
export default {
  data() {
    return {
      images: [
        { src: "https://cdn-5.motorsport.com/images/amp/6O1dL7N2/s6/start-action.jpg", text: "UNA DE LAS CARRERAS DE LA TRIPLE CORONA" },
        { src: "https://www.lemans.org/media/cache/api_news_large/assets/fileuploads/60/09/60093cbfb88f1.jpg", text: "UNA CARRERA DE 24 HORAS" },
        { src: "https://img.speedweek.com/i/6/6b51815fa1464dfb9c10bc3577b0df15.jpg?preset=i750", text: "FERRARI UN EQUIPO QUE PARTICIPA EN LA CARRERA" },
        { src: "https://toyotagazooracing.com/-/media/TMC/tgr/global/contents/wec/images/cars/2021/ogp.jpg?la=ja-JP&rev=8b92dacd1b9447d19fb8179dd142a7a3", text: "TOYOTA, UN EQUIPO QUE PARTICIPA EN LA CARRERA" },
        { src: "https://cdn-8.motorsport.com/images/amp/Yv8qd1x0/s1000/race-winner-50-ferrari-af-cors.jpg", text: "GANADORES DE LA ULTIMA CARRERA DE LMANS" }
      ]
    };
  }
};
</script>
