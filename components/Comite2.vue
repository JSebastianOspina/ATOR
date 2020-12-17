<template>
  <div 
  style="background-image:url(fondo.jpg)"
  class="flex flex-col justify-center items-center w-full pb-10">
    <h2 class="text-center text-3xl font-bold my-12 ">
      Estructura organizacional
    </h2> 
    <div
      class="border-double border-4 p-2 border-grey-400 w-full md:w-2/4 mb-6 "
      v-for="(i, key) in data"
      :key="key"
    >
      <h1 class="text-2xl parrafo font-bold text-center">
        {{ i.nombre }}
      </h1>
      <h2 class="text-lg parrafo text-center mb-2">Enero 2020 – Enero 2021</h2>
      <ul class="parrafo ml-2 ">
        <li v-for="(o, llave) in i.miembros" :key="o.Cargo">
          <strong>{{ o.Cargo }}</strong>
          <ul>
            <li v-for="(u, llave2) in o.persona" :key="llave2">
              {{ u }}
            </li>
          </ul>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      data: [
        {
          nombre: "Junta directiva",
          miembros: [
            {
              Cargo: "Presidente",
              persona: ["Jaime Arturo Campo"],
            },
            {
              Cargo: "Vice-presidente",
              persona: ["Carlos Eduardo Beltran "],
            },
            {
              Cargo: "Secretaria",
              persona: ["Luz Patricia Naranjo"],
            },
            {
              Cargo: "Tesorero",
              persona: ["Luis Fernando Arias"],
            },
            {
              Cargo: "Vocal 1",
              persona: ["Cesar Augusto Nuñez"],
            },
            {
              Cargo: "Vocal 2",
              persona: ["Manuel Guillermo Forero"],
            },
            {
              Cargo: "Vocal 3",
              persona: ["Marco Rada"],
            },
            {
              Cargo: "Revisor Fiscal",
              persona: ["Sandra Liliana Riveros"],
            },
            {
              Cargo: "Asesor Jurídico",
              persona: ["Juan Manuel Barrero"],
            },
          ],
        },
        {
          nombre: "Comité Científico",
          miembros: [
            {
              Cargo: "Prof Dr Marco rada ph.D",
              persona: [
                "director comite cientifico",
                "Investigador ATO e Investigador Asociado, Laboratorio de Anfibios",
                "Instituto de Biociências, Universidade de São Paulo (USP), Brasil.",
              ],
            },
            {
              Cargo: "Prof Dr. Luz Patricia Naranjo Ph.D",
              persona: ["G. Naturatu /Fac. de Ciencias Universidad de Ibagué."],
            },
            {
              Cargo: "Prof Dr.Manuel Guillermo Forero .Ph.D",
              persona: [
                "Director de investigacion D + Tec / ",
                "Decano Fac. de Ingeniería Universidad de Ibagué.",
              ],
            },
            {
              Cargo: "Prof/Cand PhD. Miguel Cesar Moreno ",
              persona: [
                "Representate de Naturatu,",
                " Asesor programa Biologia Ambiental (Fac. de Ciencias Unibague).",
              ],
            },
            {
              Cargo: "Prof. Cesar Augusto Nuñez MSc ",
              persona: [
                "Asesor CORTOLIMA ",
                "Asesor línea ambiental Facultad de Ciencias Universidad.de Ibagué",
                "Asesor ATO.",
              ],
            },
          ],
        },

        {
          nombre: "Comité Laboratorios y Biotecnología",
          miembros: [
            {
              Cargo: "Ing Juan Carlos Otavo MSc ",
              persona: ["Coordinador."],
            },
            {
              Cargo: "Yensi Katherine Moreno.",
              persona: [
                "Tec / Asistente laboratorio de Biotecnología e Invitro/ Universidad de Ibagué.",
              ],
            },
          ],
        },
        {
          nombre: "Comité de Eventos",
          miembros: [
            {
              persona: ["La junta Directiva y todos los Asociados de la ATO "]
            },
          ],
        },
      ],
    };
  },
};
</script>

<style>
.parrafo {
  color: #4f4f4f;
  line-height: 1.65em;
}
</style>