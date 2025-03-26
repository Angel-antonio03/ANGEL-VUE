<script setup>
import { ref } from 'vue';


defineProps({
    edad: String
})
</script>


<template>
   <h6 >
    <div class="col-md-6 ">
    <div class="card" >   
    <div class="card-body">
    <img src="https://img.freepik.com/vector-premium/nino-lindo-ropa-azul-esta-pie-suelo-cara-sonriente_1302918-88641.jpg" alt="Imagen representativa" class="" style="width: 200px; height: 150px;"/>
    Soy elcomponente hijo2 
    <p>{{ edad }}</p>

</div>
</div>
</div>
   </h6>


</template>
<style scopedyle></style>