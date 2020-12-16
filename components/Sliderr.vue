<template>
  <slider animation="fade" class="mt-8" height="80vh" :interval="4000" :speed="1000">
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
          src: "images01.jpeg",
          alt: "Descripcion imagen 1",
          encabezado: 'ATOR',
          subtitulo:'Página web oficial de la asociación tolimense de orquidelogía'
        },
        {
           src: "images02.jpeg",
          alt: "Descripcion imagen 1",
          encabezado: 'Conócenos',
          subtitulo:'Estamos ubicados en Ibagué tolima'
        },
        {
          
          src: "images01.jpeg",
          alt: "Descripcion imagen 3",
            encabezado: '¿Alguna duda?',
          subtitulo:'Contáctanos!'
        },
      ],
    };
  },
};
</script>