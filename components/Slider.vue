<template>
  <splide :options="options">
    <splide-slide >
      <img src="images01.jpeg" class="object-cover">
    </splide-slide>
    <splide-slide>
      <img src="images02.jpeg" class="object-cover">
    </splide-slide>
    <splide-slide>
      <img src="images01.jpeg" class="object-cover">
    </splide-slide>
  </splide>
</template>

<script>
import '@splidejs/splide/dist/css/themes/splide-sea-green.min.css';

  export default { 
    data() {
      return {
        options: {
          rewind : true,
          autoWidth : true,
          height: '70vh',
          gap    : '1rem',
        },
      };
    },
  }
</script>