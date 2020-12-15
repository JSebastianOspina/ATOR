<template>
  <splide :options="options">
    <splide-slide>
      <img src="images01.jpeg">
    </splide-slide>
    <splide-slide>
      <img src="images02.jpeg">
    </splide-slide>
    <splide-slide>
      <img src="images01.jpeg">
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
          gap    : '1rem',
        },
      };
    },
  }
</script>