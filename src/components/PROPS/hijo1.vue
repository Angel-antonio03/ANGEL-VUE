<script setup>
import { ref } from 'vue';

defineProps({
    edad: String
})
</script>


<template>
   <h6>
    <div class="col-md-6">
    <div class="card">   
    <div class="card-body ">
    <img src="https://img.freepik.com/vector-premium/nino-escuela-10-anos_635702-851.jpg" alt="Imagen representativa" class="" style="width: 200px; height: 150px;"/>
    Soy elcomponente hijo 1
    <p>{{ edad }}</p>
    </div>
                 

    </div>
    </div>
                          
   </h6>
</template>
<style scopedyle></style>