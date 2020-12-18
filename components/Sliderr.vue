<template>
  <slider animation="fade" class="mt-8" height="70vh" :interval="4000" :speed="1000">
    <slider-item v-for="(i, index) in list" :key="index">
      <div
        class="flex flex-col justify-center items-center h-full w-full bg-cover bg-center"
        :style="'background-image: url('+i.src+')'"
      >
        <h1 class="text-5xl text-gray-200 mb-6">{{i.encabezado}}</h1>
        <h2 class="text-2xl text-gray-200 text-center">{{i.subtitulo}}</h2>
      </div>
    </slider-item>
  </slider>
</template>

<script>
export default {
  data() {
    return {
      list: [
        {
          src: "slider/1.jpg",
          alt: "Cattleya forbesii",
          encabezado: 'ATO',
          subtitulo:'Página web oficial de la asociación tolimense de orquidelogía'
        },
        {
           src: "slider/2.jpg",
          alt: "Ocidium cebolleta",
          encabezado: 'Conócenos',
          subtitulo:'Estamos ubicados en Ibagué tolima'
        },
        {
          
          src: "slider/3.jpg",
          alt: "Cattleya mendelli",
          encabezado: '¿Alguna duda?',
          subtitulo:'Contáctanos!'
        },
      ],
    };
  },
};
</script>