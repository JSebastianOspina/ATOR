<template>
  <div class="">
    <h2 class="text-3xl text-center mt-12 mb-2">Visitas internacionales</h2>
    <p class="text-justify  md:text-center mx-5 md:mx-0">
      La ATO promueve y programa dos salidas al año , generalmente son eventos
      que invitan al estudio y disfrute de la orquideologia.
    </p>
    <div class="eventos flex flex-col md:flex-row items-start justify-around mt-8 w-100 px-5 md:px-24">
      <div class="w-full md:w-1/4 mb-8" v-for="(i, key) in data" :key="key">
        <img :src="i.img" alt="" class="object-cover w-full h-48" height="500"/>
        <h3 class="text-xl font-medium">{{i.año}}</h3>
        <ul>
            <li v-for="(o,key2) in i.eventos" :key="key2" class="mb-4">
                <a :href="o.url" style="color: #262626">{{o.nombre}}</a>
            </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      data: [
        {
          año: 2019,
          img: "eventos/1.jpg",
          eventos: [
            {
              nombre: "Redland International Orhid Festival - Florida, U.S.A",
              url: "https://www.redlandorchidfest.org/",
            },
            {
              nombre: "VI Exposición Internacional de Orquídeas",
              url: "https://www.redlandorchidfest.org/",
            },
            {
              nombre: "Alexander Von Humboldt – Quito, Ecuador. ",
              url:
                "https://www.udla.edu.ec/2019/10/01/6ta-exposicion-internacional-de-orquideas-alexander-von-humboldt/",
            },
          ],
        },

        {
          año: 2018,
          img: "eventos/2.jpg",

          eventos: [
            {
              nombre:
                "XVIII Conferencia Europea de Orquideologia - Paris,Francia",
              url:
                "https://www.europeanorchidcouncil.eu/dateien/EOCCE%20Report__The%20Orchid%20Review.%20FINAL.%20low%20res.pdf",
            },
            {
              nombre:
                "Visita a la Asociacion Orquideofila de Sao Paulo - Brasil",
              url: "http://www.aosp.com.br/",
            },
          ],
        },

        {
          año: 2017,
          img: "eventos/3.jpg",
          eventos: [
            {
              nombre:
                "Conferencia Mundial de Orquideas XXII WOC - Guayaqui,Ecuador",
              url: "https://www.youtube.com/watch?v=ulw9ahSkuhc",
            },
          ],
        },
      ],
    };
  },
};
</script>

<style>
</style>